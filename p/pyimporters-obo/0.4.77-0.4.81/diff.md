# Comparing `tmp/pyimporters-obo-0.4.77.tar.gz` & `tmp/pyimporters_obo-0.4.81.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyimporters-obo-0.4.77.tar", last modified: Thu Dec 15 17:29:05 2022, max compression
+gzip compressed data, was "pyimporters_obo-0.4.81.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyimporters-obo-0.4.77.tar` & `pyimporters_obo-0.4.81.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       97 2022-12-15 17:27:54.901248 pyimporters-obo-0.4.77/.dockerignore
--rw-r--r--   0        0        0      147 2022-12-15 17:27:54.901248 pyimporters-obo-0.4.77/.gitignore
--rw-r--r--   0        0        0      448 2022-12-15 17:27:54.902248 pyimporters-obo-0.4.77/Dockerfile
--rw-r--r--   0        0        0    10580 2022-12-15 17:27:54.902248 pyimporters-obo-0.4.77/Jenkinsfile
--rw-r--r--   0        0        0      147 2022-12-15 17:27:54.902248 pyimporters-obo-0.4.77/README.md
--rw-r--r--   0        0        0       61 2022-12-15 17:29:04.002050 pyimporters-obo-0.4.77/pyimporters_obo/__init__.py
--rw-r--r--   0        0        0     2796 2022-12-15 17:27:54.904248 pyimporters-obo-0.4.77/pyimporters_obo/obo.py
--rw-r--r--   0        0        0     1977 2022-12-15 17:27:54.904248 pyimporters-obo-0.4.77/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-15 17:27:54.904248 pyimporters-obo-0.4.77/tests/__init__.py
--rw-r--r--   0        0        0     5734 2022-12-15 17:27:54.906248 pyimporters-obo-0.4.77/tests/data/small.obo
--rw-r--r--   0        0        0     2234 2022-12-15 17:27:54.906248 pyimporters-obo-0.4.77/tests/data/small.zip
--rw-r--r--   0        0        0     2081 2022-12-15 17:27:54.907248 pyimporters-obo-0.4.77/tests/test_obo.py
--rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 pyimporters-obo-0.4.77/setup.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pyimporters-obo-0.4.77/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-08-09 05:37:25.311532 pyimporters_obo-0.4.81/.dockerignore
+-rw-r--r--   0        0        0      178 2023-08-09 05:37:25.311532 pyimporters_obo-0.4.81/.gitignore
+-rw-r--r--   0        0        0      448 2023-08-09 05:37:25.312532 pyimporters_obo-0.4.81/Dockerfile
+-rw-r--r--   0        0        0    12845 2023-08-09 05:37:25.312532 pyimporters_obo-0.4.81/Jenkinsfile
+-rw-r--r--   0        0        0      147 2023-08-09 05:37:25.314532 pyimporters_obo-0.4.81/README.md
+-rw-r--r--   0        0        0       61 2023-08-09 05:38:01.710513 pyimporters_obo-0.4.81/pyimporters_obo/__init__.py
+-rw-r--r--   0        0        0     2796 2023-08-09 05:37:25.318532 pyimporters_obo-0.4.81/pyimporters_obo/obo.py
+-rw-r--r--   0        0        0     1977 2023-08-09 05:37:25.318532 pyimporters_obo-0.4.81/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-09 05:37:25.319532 pyimporters_obo-0.4.81/tests/__init__.py
+-rw-r--r--   0        0        0     5734 2023-08-09 05:37:25.321532 pyimporters_obo-0.4.81/tests/data/small.obo
+-rw-r--r--   0        0        0     2234 2023-08-09 05:37:25.322532 pyimporters_obo-0.4.81/tests/data/small.zip
+-rw-r--r--   0        0        0     2081 2023-08-09 05:37:25.324532 pyimporters_obo-0.4.81/tests/test_obo.py
+-rw-r--r--   0        0        0      770 1970-01-01 00:00:00.000000 pyimporters_obo-0.4.81/setup.py
+-rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 pyimporters_obo-0.4.81/PKG-INFO
```

### Comparing `pyimporters-obo-0.4.77/Jenkinsfile` & `pyimporters_obo-0.4.81/Jenkinsfile`

 * *Files 26% similar despite different names*

```diff
@@ -1,116 +1,88 @@
 pipeline {
-
   environment {
-    PATH_HOME = "/home/jenkins"
-    PYTHONDONTWRITEBYTECODE = "1"
-    PYTHONPYCACHEPREFIX = "/tmp/.pytest_cache"
-    TEST_REPORT_DIR="/root/test-reports"
-    MAJOR_VERSION = "0"
-    MINOR_VERSION = "4"
+    PATH_HOME = '/home/jenkins'
+    TEST_REPORT_DIR = '/root/test-reports'
+    PYTHONPYCACHEPREFIX = '/tmp/.pytest_cache'
+    PYTHONDONTWRITEBYTECODE = '1'
     GIT_AUTH = credentials('bitbucket-user')
+
+    MAJOR_VERSION = '0'
+    MINOR_VERSION = '4'
   }
 
   agent none
 
   triggers {
-    upstream(upstreamProjects: "pyimporters_plugins/" + env.BRANCH_NAME.replaceAll("/", "%2F"),\
+    upstream(upstreamProjects: 'pyimporters_plugins/' + env.BRANCH_NAME.replaceAll('/', '%2F'),\
                                 threshold: hudson.model.Result.SUCCESS)
   }
 
-  parameters {
-      booleanParam(defaultValue: false, description: 'if set to true (ticked), it will not skip on CI commit', name: 'forcePublishing')
-  }
-
   stages {
-
     stage('Catch build termination') {
       agent {
         node {
           label 'built-in'
           customWorkspace "/home/jenkins/${env.JOB_NAME}"
         }
       }
       stages {
-        stage('Abort if upstream or CI_commit') {
+        stage('Analyse build cause') {
           steps {
             script {
-              abortBuild()
+              analyseBuildCause()
             }
           }
         }
       }
     }
 
     stage('Generate new version') {
+      when {
+        environment name: 'SKIP_JOB', value: '0'
+      }
+
       agent {
         node {
           label 'built-in'
           customWorkspace "/home/jenkins/${env.JOB_NAME}"
         }
       }
 
       stages {
-
         stage('Add credentials') {
           steps {
             script {
               // Add password file for flit publishing
               sh "cp ${env.PATH_HOME}/.passwd-pypi .env"
             }
           }
         }
 
-        stage('Skip on CI commit') {
-          steps {
-            script {
-              // returnStatus = 1 when string not found -> Team commit
-              // returnStatus = 0 when string is found  -> CI commit
-              env.LAST_COMMIT_IS_TEAM = sh(
-                      script: 'git log -1 | grep "\\[Jenkins CI\\]"',
-                      returnStatus: true
-              )
-              if (LAST_COMMIT_IS_TEAM == '0') {
-                println "Last commit has been done by CI, skipping next steps"
-              } else {
-                println "Last commit has been done by Team, processing"
-              }
-              if (params.forcePublishing) {
-                println "Try to publish, considering last commit has been done by Team"
-                env.LAST_COMMIT_IS_TEAM = "1"
-              }
-            }
-          }
-        }
-
         stage('Commit new version') {
-          when {
-            environment name: "LAST_COMMIT_IS_TEAM", value: "1"
-          }
           steps {
             script {
               println("attempt to publish ${env.JOB_NAME} with version: ${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}")
 
               // push updates of file __init__.py
               withCredentials([gitUsernamePassword(credentialsId: 'bitbucket-user', gitToolName: 'git-tool')]) {
                 sh "echo '\"\"\"Sherpa knowledge import plugins\"\"\"' > pyimporters_obo/__init__.py"
                 sh "echo '__version__ = \"${MAJOR_VERSION}.${MINOR_VERSION}.${env.BUILD_ID}\"' >> pyimporters_obo/__init__.py"
                 sh 'git commit pyimporters_obo/__init__.py -m "[Jenkins CI] Commit on version files" || echo "No changes to commit"'
                 sh 'git push'
               }
             }
           }
         }
-
       }
     }
 
     stage('Build, test and publish') {
       when {
-        environment name: "LAST_COMMIT_IS_TEAM", value: "1"
+        environment name: 'SKIP_JOB', value: '0'
       }
 
       agent {
         // dockerfile agent
         // Mounted volume for Junit reports
         //   - docker: /root/test-reports
         //   - host  : /tmp/_${env.JOB_NAME}/test-reports
@@ -119,15 +91,14 @@
           customWorkspace "/home/jenkins/${env.JOB_NAME}"
           filename 'Dockerfile'
           args "-u root --privileged -v /tmp/_${env.JOB_NAME}/test-reports:${TEST_REPORT_DIR}"
         }
       }
 
       stages {
-
         stage('Install flit & flake8') {
           steps {
             sh 'python -m pip install pip==22.0.3'
             sh 'pip install --no-cache-dir flit==3.2.0 flake8==3.9.2 flakehell'
             sh 'flit install'
           }
         }
@@ -148,16 +119,16 @@
             // purge python cache
             sh "rm -rf ${PYTHONPYCACHEPREFIX}"
           }
         }
 
         stage('Publish on PyPI') {
           environment {
-            FLIT_USERNAME = getUserName ".env"
-            FLIT_PASSWORD = getUserPass ".env"
+            FLIT_USERNAME = getUserName '.env'
+            FLIT_PASSWORD = getUserPass '.env'
           }
           steps {
             // remove any previous folder dist
             sh 'rm -rf dist'
             // create (as root) folder dist
             sh 'mkdir dist'
             // pull recent updates of file __init__.py
@@ -176,79 +147,94 @@
             sh 'rm -rf dist'
             // remove current folder .hypothesis
             sh 'rm -rf .hypothesis'
             // remove current folder .tox
             sh 'rm -rf .tox'
           }
         }
-
       }
-
     }
-
   }
 
   post {
     // only triggered when blue or green sign
     success {
       // node is specified here to get an agent
       node('built-in') {
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${env.JOB_NAME}") {
           script {
             try {
-              sh "rm -f results.xml"
+              sh 'rm -f results.xml'
               sh "cp /tmp/_${env.JOB_NAME}/test-reports/results.xml results.xml"
             } catch (Exception e) {
               echo 'Exception occurred: ' + e.toString()
             }
             try {
               junit 'results.xml'
             } catch (Exception e) {
               echo 'Exception occurred: ' + e.toString()
             }
-            println "sending Systematic Build notification"
-            emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
-                    replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
-                    to: '${DEFAULT_RECIPIENTS}')
+            if (sendEmailNotif("/home/jenkins/${env.JOB_NAME}", "${env.BUILD_NUMBER}")) {
+              println 'sending Success Build notification'
+              CUSTOM_SUBJECT = '[CI - Jenkinzz SUCCESS] ' + env.CUSTOM_SUBJECT
+              emailext(
+                  mimeType: 'text/html',
+                  subject: CUSTOM_SUBJECT,
+                  body: '${DEFAULT_CONTENT}',
+                  replyTo: '${DEFAULT_REPLYTO}',
+                  to: '${ADMIN_RECIPIENTS}' + ',' + CUSTOM_RECIPIENTS
+              )
+              switchEmailNotif(false, env.BUILD_NUMBER)
+            } else {
+              println 'preventing Success Build notification'
+            }
           }
         }
       }
     }
     // triggered when red sign
     failure {
       // node is specified here to get an agent
       node('built-in') {
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${env.JOB_NAME}") {
           script {
             try {
-              sh "rm -f results.xml"
+              sh 'rm -f results.xml'
               sh "cp /tmp/_${env.JOB_NAME}/test-reports/results.xml results.xml"
             } catch (Exception e) {
               echo 'Exception occurred: ' + e.toString()
             }
             try {
               junit 'results.xml'
             } catch (Exception e) {
               echo 'Exception occurred: ' + e.toString()
             }
-            println "sending Systematic Build notification"
-            emailext(body: '${DEFAULT_CONTENT}', mimeType: 'text/html',
-                    replyTo: '${DEFAULT_REPLYTO}', subject: '${DEFAULT_SUBJECT}',
-                    to: '${DEFAULT_RECIPIENTS}')
+            println 'sending Failure Build notification'
+            CUSTOM_SUBJECT = '[CI - Jenkinzz FAILURE] ' + env.CUSTOM_SUBJECT
+            emailext(
+                mimeType: 'text/html',
+                subject: CUSTOM_SUBJECT,
+                body: '${DEFAULT_CONTENT}',
+                replyTo: '${DEFAULT_REPLYTO}',
+                to: '${ADMIN_RECIPIENTS}' + ',' + CUSTOM_RECIPIENTS
+            )
           }
         }
       }
     }
+    // triggered when black sign
+    aborted {
+      println 'post-declarative message: abort job'
+    }
     // trigger every-works
     //always {
     //}
   }
-
 }
 
 // return FLIT_USERNAME from given file
 def getUserName(path) {
   USERNAME = sh(
                  script: "grep FLIT_USERNAME ${path}|cut -d '=' -f2",
                  returnStdout: true
@@ -261,70 +247,134 @@
   USERPASS = sh(
                  script: "grep FLIT_PASSWORD ${path}|cut -d '=' -f2",
                  returnStdout: true
                ).trim()
   return USERPASS
 }
 
-def abortBuild() {
-  def upstream_projects = ["pyimporters_plugins"]
-  def upstream_running = null
-  def jobName
-  // iterate over upstream_projects
-  for (upstream_project in upstream_projects) {
-    Jenkins.instance.getItemByFullName(upstream_project).getItems().each { repository ->
-      def isRunning = false
+// create/remove emailNotif file to trigger email notification
+def switchEmailNotif(toggle, build) {
+  if (toggle) {
+    sh 'echo ' + build + ' > .emailNotif'
+  } else {
+    if (build == env.BUILD_NUMBER) {
+      sh 'rm -f .emailNotif'
+    }
+  }
+}
+
+// return true if emailNotif file present
+boolean sendEmailNotif(path, build) {
+  emailNotif = sh(
+                 script: "find ${path} -name '.emailNotif'|wc -l",
+                 returnStdout: true
+               ).trim()
+  emailContent = ''
+  if (emailNotif == '1') {
+    emailContent = sh(
+                     script: "cat ${path}/.emailNotif",
+                     returnStdout: true
+                   ).trim()
+  }
+  return (emailContent == build)
+}
+
+def analyseBuildCause() {
+  upstreamProjects = ['pyimporters_plugins']
+  boolean upstreamRunning = false
+  String jobName
+  // iterate over upstreamProjects
+  for (upstream_project in upstreamProjects) {
+    Jenkins.instance.getItemByFullName(upstream_project).items.each { repository ->
+      boolean isRunning = false
       //repository.parent.name: project
       //repository.name: branch
       if ( repository.name == env.BRANCH_NAME ) {
         // iterate over all jobs of current repository
-        repository.getAllJobs().each { job ->
+        repository.allJobs.each { job ->
           // iterate over all builds of current job
           job.builds.each { build ->
             // determine if a build is running or not
-            if ( build.getResult().equals(null) ) {
+            if ( build.result == (null) ) {
               jobName = build.parent.parent.name
               isRunning = true
             }
           }
           if ( isRunning ) {
-            upstream_running = true
+            upstreamRunning = true
           }
         }
       }
     }
   }
-  // Abort build when upstream detected
-  if (upstream_running != null) {
-    println 'Aborting build because upstream job detected (' + jobName + ')'
-    currentBuild.result = 'ABORTED'
-    currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
-    sleep(1)   // Interrupt is not blocking and does not take effect immediately.
-  }
-  // Abort build when last commit is CI commit
-  // returnStatus = 1 when string not found -> Team commit
-  // returnStatus = 0 when string is found  -> CI commit
-  def last_commit_is_team = sh(
+
+  // Catch if build has been triggered by CI Commit
+  // returnStatus = true  when string not found -> Team commit
+  // returnStatus = false when string is found  -> CI commit
+  boolean lastCommitIsTeam = sh(
     script: 'git log -1 | grep "\\[Jenkins CI\\]"',
     returnStatus: true
   )
-  if (params.forcePublishing) {
-    println "Try to publish, proceeding"
-    last_commit_is_team = 1
-  }
-  def isStartedByUser = currentBuild.rawBuild.getCause(hudson.model.Cause$UserIdCause) != null
-  if (isStartedByUser) {
-    println "Job started by User, proceeding"
-    last_commit_is_team = 1
-  }
-  def isStartedByUpstream = currentBuild.rawBuild.getCause(hudson.model.Cause$UpstreamCause) != null
-  if (isStartedByUpstream) {
-    println "Job started by Upstream, proceeding"
-    last_commit_is_team = 1
-  }
-  if (last_commit_is_team == 0) {
-    println 'Aborting build because last commit has been done by CI'
-    currentBuild.result = 'ABORTED'
-    currentBuild.getRawBuild().getExecutor().interrupt(Result.ABORTED)
-    sleep(1)   // Interrupt is not blocking and does not take effect immediately.
+
+  // Skip build when upstream detected
+  if (upstreamRunning) {
+    println 'Skipping build because upstream job detected (' + jobName + ')'
+    env.SKIP_JOB = '1'
+    switchEmailNotif(false, 0)
+  }
+
+  // Catch if build has been triggered by User
+  boolean isStartedByUser = currentBuild.rawBuild.getCause(hudson.model.Cause$UserIdCause) != null
+  if (isStartedByUser && !upstreamRunning) {
+    env.SKIP_JOB = '0'
+    env.CUSTOM_SUBJECT = env.JOB_NAME + ' - Manual Build #' + env.BUILD_NUMBER
+    env.CUSTOM_RECIPIENTS = emailextrecipients([[$class: 'RequesterRecipientProvider']])
+    switchEmailNotif(true, env.BUILD_NUMBER)
+    println 'Job started by User, proceeding'
+  }
+
+  // Catch if build has been triggered by Upstream
+  boolean isStartedByUpstream = currentBuild.rawBuild.getCause(hudson.model.Cause$UpstreamCause) != null
+  if (isStartedByUpstream && !upstreamRunning) {
+    env.SKIP_JOB = '0'
+    env.CUSTOM_SUBJECT = env.JOB_NAME + ' - Upstream Build #' + env.BUILD_NUMBER
+    env.CUSTOM_RECIPIENTS = emailextrecipients([[$class:'UpstreamComitterRecipientProvider']])
+    switchEmailNotif(true, env.BUILD_NUMBER)
+    println 'Job started by Upstream, proceeding'
+  }
+
+  // Catch if build has been triggered by User Commit
+  boolean isStartedByCommit = currentBuild.rawBuild.getCause(jenkins.branch.BranchEventCause) != null
+  if (isStartedByCommit && lastCommitIsTeam && !upstreamRunning) {
+    env.SKIP_JOB = '0'
+    env.CUSTOM_SUBJECT = env.JOB_NAME + ' - SCM Build #' + env.BUILD_NUMBER
+    env.CUSTOM_RECIPIENTS = emailextrecipients([[$class: 'DevelopersRecipientProvider'], [$class:'CulpritsRecipientProvider']])
+    switchEmailNotif(true, env.BUILD_NUMBER)
+    println 'Job started by User Commit, proceeding'
+  }
+
+  // Catch if build has been triggered by cron
+  boolean isStartedByCron = currentBuild.rawBuild.getCause(hudson.triggers.TimerTrigger$TimerTriggerCause) != null
+  if (isStartedByCron && lastCommitIsTeam && !upstreamRunning) {
+    env.SKIP_JOB = '0'
+    env.CUSTOM_SUBJECT = env.JOB_NAME + ' - CRON Build #' + env.BUILD_NUMBER
+    env.CUSTOM_RECIPIENTS = emailextrecipients([[$class: 'DevelopersRecipientProvider'], [$class:'CulpritsRecipientProvider']])
+    switchEmailNotif(true, env.BUILD_NUMBER)
+    println 'Job started by Cron, proceeding'
+  }
+
+  // Catch if build has been triggered by branch discovery
+  boolean isStartedByBranchDiscovery = currentBuild.rawBuild.getCause(jenkins.branch.BranchIndexingCause) != null
+  if (isStartedByBranchDiscovery && lastCommitIsTeam && !upstreamRunning) {
+    env.SKIP_JOB = '0'
+    env.CUSTOM_SUBJECT = env.JOB_NAME + ' - BranchDiscovery Build #' + env.BUILD_NUMBER
+    env.CUSTOM_RECIPIENTS = emailextrecipients([[$class: 'DevelopersRecipientProvider'], [$class:'CulpritsRecipientProvider']])
+    switchEmailNotif(true, env.BUILD_NUMBER)
+    println 'Job started by Branch Discovery, proceeding'
+  }
+
+  if (!lastCommitIsTeam && !upstreamRunning && !isStartedByUser && !isStartedByUpstream) {
+    println 'Skipping build because last commit has been done by CI'
+    env.SKIP_JOB = '1'
+    switchEmailNotif(false, 0)
   }
 }
```

### Comparing `pyimporters-obo-0.4.77/pyimporters_obo/obo.py` & `pyimporters_obo-0.4.81/pyimporters_obo/obo.py`

 * *Files identical despite different names*

### Comparing `pyimporters-obo-0.4.77/pyproject.toml` & `pyimporters_obo-0.4.81/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyimporters-obo-0.4.77/tests/data/small.obo` & `pyimporters_obo-0.4.81/tests/data/small.obo`

 * *Files identical despite different names*

### Comparing `pyimporters-obo-0.4.77/tests/data/small.zip` & `pyimporters_obo-0.4.81/tests/data/small.zip`

 * *Files identical despite different names*

### Comparing `pyimporters-obo-0.4.77/tests/test_obo.py` & `pyimporters_obo-0.4.81/tests/test_obo.py`

 * *Files identical despite different names*

### Comparing `pyimporters-obo-0.4.77/setup.py` & `pyimporters_obo-0.4.81/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 install_requires = \
 ['pyimporters_plugins>=0.4.0,<0.5.0', 'collections-extended', 'obonet']
 
 entry_points = \
 {'pyimporters.plugins': ['obo = pyimporters_obo.obo:OBOKnowledgeParser']}
 
 setup(name='pyimporters-obo',
-      version='0.4.77',
+      version='0.4.81',
       description='Sherpa knowledge import plugins',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyimporters-obo-0.4.77/PKG-INFO` & `pyimporters_obo-0.4.81/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyimporters-obo
-Version: 0.4.77
+Version: 0.4.81
 Summary: Sherpa knowledge import plugins
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

