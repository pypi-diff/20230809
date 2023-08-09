# Comparing `tmp/pyimporters-json-0.4.6.tar.gz` & `tmp/pyimporters-json-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimporters-json-0.4.6.tar", last modified: Wed Jan 26 15:49:46 2022, max compression
+gzip compressed data, was "pyimporters-json-0.4.9.tar", last modified: Thu Feb 24 20:17:07 2022, max compression
```

## Comparing `pyimporters-json-0.4.6.tar` & `pyimporters-json-0.4.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       97 2022-01-26 15:24:28.506488 pyimporters-json-0.4.6/.dockerignore
--rw-r--r--   0        0        0      147 2022-01-26 15:24:28.506488 pyimporters-json-0.4.6/.gitignore
--rw-r--r--   0        0        0      466 2022-01-26 15:24:28.506488 pyimporters-json-0.4.6/Dockerfile
--rw-r--r--   0        0        0     8270 2022-01-26 15:46:48.510852 pyimporters-json-0.4.6/Jenkinsfile
--rw-r--r--   0        0        0      149 2022-01-26 15:46:48.511852 pyimporters-json-0.4.6/README.md
--rw-r--r--   0        0        0       60 2022-01-26 15:49:43.499467 pyimporters-json-0.4.6/pyimporters_json/__init__.py
--rw-r--r--   0        0        0     1244 2022-01-26 15:46:48.511852 pyimporters-json-0.4.6/pyimporters_json/json.py
--rw-r--r--   0        0        0     2068 2022-01-26 15:46:48.512853 pyimporters-json-0.4.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-01-26 15:24:28.506488 pyimporters-json-0.4.6/tests/__init__.py
--rwxr-xr-x   0        0        0   225891 2022-01-26 15:46:48.513852 pyimporters-json-0.4.6/tests/data/organization_en.json
--rw-r--r--   0        0        0      695 2022-01-26 15:46:48.514852 pyimporters-json-0.4.6/tests/test_json.py
--rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 pyimporters-json-0.4.6/setup.py
--rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 pyimporters-json-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0       97 2022-01-26 15:24:28.506488 pyimporters-json-0.4.9/.dockerignore
+-rw-r--r--   0        0        0      147 2022-01-26 15:24:28.506488 pyimporters-json-0.4.9/.gitignore
+-rw-r--r--   0        0        0      466 2022-01-26 15:24:28.506488 pyimporters-json-0.4.9/Dockerfile
+-rw-r--r--   0        0        0    10232 2022-02-24 20:16:20.410290 pyimporters-json-0.4.9/Jenkinsfile
+-rw-r--r--   0        0        0      149 2022-01-26 15:46:48.511852 pyimporters-json-0.4.9/README.md
+-rw-r--r--   0        0        0       60 2022-02-24 20:17:06.312478 pyimporters-json-0.4.9/pyimporters_json/__init__.py
+-rw-r--r--   0        0        0     1244 2022-01-26 15:46:48.511852 pyimporters-json-0.4.9/pyimporters_json/json.py
+-rw-r--r--   0        0        0     2068 2022-01-26 15:46:48.512853 pyimporters-json-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-01-26 15:24:28.506488 pyimporters-json-0.4.9/tests/__init__.py
+-rwxr-xr-x   0        0        0   225891 2022-01-26 15:46:48.513852 pyimporters-json-0.4.9/tests/data/organization_en.json
+-rw-r--r--   0        0        0      695 2022-01-26 15:46:48.514852 pyimporters-json-0.4.9/tests/test_json.py
+-rw-r--r--   0        0        0      795 1970-01-01 00:00:00.000000 pyimporters-json-0.4.9/setup.py
+-rw-r--r--   0        0        0     1591 1970-01-01 00:00:00.000000 pyimporters-json-0.4.9/PKG-INFO
```

### Comparing `pyimporters-json-0.4.6/Jenkinsfile` & `pyimporters-json-0.4.9/Jenkinsfile`

 * *Files 15% similar despite different names*

```diff
@@ -19,18 +19,28 @@
 
   parameters {
       booleanParam(defaultValue: false, description: 'if set to true (ticked), it will not skip on CI commit', name: 'forcePublishing')
   }
 
   stages {
 
-    stage('Abort when upstream') {
-      steps {
-        script {
-          abortBuild()
+    stage('Catch build termination') {
+      agent {
+        node {
+          label 'built-in'
+          customWorkspace "/home/jenkins/${env.JOB_NAME}"
+        }
+      }
+      stages {
+        stage('Abort if upstream or CI_commit') {
+          steps {
+            script {
+              abortBuild()
+            }
+          }
         }
       }
     }
 
     stage('Generate new version') {
       agent {
         node {
@@ -173,21 +183,41 @@
 
     }
 
   }
 
   post {
     // only triggered when blue or green sign
-    //success {
-    //}
+    success {
+      // node is specified here to get an agent
+      node('built-in') {
+        // keep using customWorkspace to store Junit report
+        ws("/home/jenkins/${env.JOB_NAME}") {
+          script {
+            try {
+              sh "rm -f results.xml"
+              sh "cp /tmp/_${env.JOB_NAME}/test-reports/results.xml results.xml"
+            } catch (Exception e) {
+              echo 'Exception occurred: ' + e.toString()
+            }
+            try {
+              junit 'results.xml'
+            } catch (Exception e) {
+              echo 'Exception occurred: ' + e.toString()
+            }
+            println "sending Systematic Build notification"
+            emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
+                    replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
+                    to: '${DEFAULT_RECIPIENTS}')
+          }
+        }
+      }
+    }
     // triggered when red sign
-    //failure {
-    //}
-    // trigger every-works
-    always {
+    failure {
       // node is specified here to get an agent
       node('built-in') {
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${env.JOB_NAME}") {
           script {
             try {
               sh "rm -f results.xml"
@@ -204,14 +234,17 @@
             emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
                     replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
                     to: '${DEFAULT_RECIPIENTS}')
           }
         }
       }
     }
+    // trigger every-works
+    //always {
+    //}
   }
 
 }
 
 // return FLIT_USERNAME from given file
 def getUserName(path) {
   USERNAME = sh(
@@ -254,16 +287,37 @@
           if ( isRunning ) {
             upstream_running = true
           }
         }
       }
     }
   }
+  // Abort build when upstream detected
   if (upstream_running != null) {
     println 'Aborting build because upstream job detected (' + jobName + ')'
     currentBuild.result = 'ABORTED'
     currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
     sleep(1)   // Interrupt is not blocking and does not take effect immediately.
-
-    //error('Aborting build because upstream job detected (' + jobName + ')')
+  }
+  // Abort build when last commit is CI commit
+  // returnStatus = 1 when string not found -> Team commit
+  // returnStatus = 0 when string is found  -> CI commit
+  def last_commit_is_team = sh(
+    script: 'git log -1 | grep "\\[Jenkins CI\\]"',
+    returnStatus: true
+  )
+  if (params.forcePublishing) {
+    println "Try to publish, proceeding"
+    last_commit_is_team = 1
+  }
+  def isStartedByUser = currentBuild.rawBuild.getCause(hudson.model.Cause$UserIdCause) != null
+  if (isStartedByUser) {
+    println "Job started by User, proceeding"
+    last_commit_is_team = 1
+  }
+  if (last_commit_is_team == 0) {
+    println 'Aborting build because last commit has been done by CI'
+    currentBuild.result = 'ABORTED'
+    currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
+    sleep(1)   // Interrupt is not blocking and does not take effect immediately.
   }
 }
```

### Comparing `pyimporters-json-0.4.6/pyimporters_json/json.py` & `pyimporters-json-0.4.9/pyimporters_json/json.py`

 * *Files identical despite different names*

### Comparing `pyimporters-json-0.4.6/pyproject.toml` & `pyimporters-json-0.4.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyimporters-json-0.4.6/tests/data/organization_en.json` & `pyimporters-json-0.4.9/tests/data/organization_en.json`

 * *Files identical despite different names*

### Comparing `pyimporters-json-0.4.6/tests/test_json.py` & `pyimporters-json-0.4.9/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `pyimporters-json-0.4.6/setup.py` & `pyimporters-json-0.4.9/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'xlrd',
  'openpyxl']
 
 entry_points = \
 {'pyimporters.plugins': ['json = pyimporters_json.json:JSONKnowledgeParser']}
 
 setup(name='pyimporters-json',
-      version='0.4.6',
+      version='0.4.9',
       description='Sherpa knowledge import plugins',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyimporters-json-0.4.6/PKG-INFO` & `pyimporters-json-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimporters-json
-Version: 0.4.6
+Version: 0.4.9
 Summary: Sherpa knowledge import plugins
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

