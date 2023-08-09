# Comparing `tmp/app_ordering-1.1.tar.gz` & `tmp/app_ordering-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "app_ordering-1.1.tar", last modified: Mon Aug  7 04:33:11 2023, max compression
+gzip compressed data, was "app_ordering-1.2.tar", last modified: Wed Aug  9 03:03:52 2023, max compression
```

## Comparing `app_ordering-1.1.tar` & `app_ordering-1.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.046950 app_ordering-1.1/
--rw-r--r--   0 geek      (1000) geek      (1000)     1064 2023-08-07 04:12:21.000000 app_ordering-1.1/LICENSE.txt
--rw-rw-r--   0 geek      (1000) geek      (1000)     1750 2023-08-07 04:33:11.046950 app_ordering-1.1/PKG-INFO
--rw-rw-r--   0 geek      (1000) geek      (1000)     1393 2023-08-07 04:32:35.000000 app_ordering-1.1/README.md
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/
--rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-14 10:01:01.000000 app_ordering-1.1/app_ordering/__init__.py
--rw-rw-r--   0 geek      (1000) geek      (1000)     2698 2023-08-03 02:27:34.000000 app_ordering-1.1/app_ordering/admin.py
--rw-rw-r--   0 geek      (1000) geek      (1000)     4231 2023-08-03 02:39:37.000000 app_ordering-1.1/app_ordering/apps.py
--rw-r--r--   0 geek      (1000) geek      (1000)      327 2023-08-03 03:09:49.000000 app_ordering-1.1/app_ordering/helpers.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/management/
--rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 07:08:54.000000 app_ordering-1.1/app_ordering/management/__init__.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/management/commands/
--rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 07:14:27.000000 app_ordering-1.1/app_ordering/management/commands/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)      319 2023-07-17 09:17:30.000000 app_ordering-1.1/app_ordering/management/commands/sync_admin_apps.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/migrations/
--rw-rw-r--   0 geek      (1000) geek      (1000)     5397 2023-07-17 10:52:21.000000 app_ordering-1.1/app_ordering/migrations/0001_initial.py
--rw-rw-r--   0 geek      (1000) geek      (1000)     1021 2023-07-17 11:08:54.000000 app_ordering-1.1/app_ordering/migrations/0002_alter_profile_groups_alter_profile_users.py
--rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-14 10:01:01.000000 app_ordering-1.1/app_ordering/migrations/__init__.py
--rw-rw-r--   0 geek      (1000) geek      (1000)     2702 2023-07-17 11:08:47.000000 app_ordering-1.1/app_ordering/models.py
--rw-r--r--   0 geek      (1000) geek      (1000)     2747 2023-08-03 02:21:20.000000 app_ordering-1.1/app_ordering/services.py
--rw-r--r--   0 geek      (1000) geek      (1000)      365 2023-08-03 02:39:01.000000 app_ordering-1.1/app_ordering/signals.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/templates/
--rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-17 13:47:46.000000 app_ordering-1.1/app_ordering/templates/__init__.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering/templates/admin/
--rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-17 13:47:46.000000 app_ordering-1.1/app_ordering/templates/admin/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)     2509 2023-07-17 08:53:15.000000 app_ordering-1.1/app_ordering/templates/admin/app_list.html
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.046950 app_ordering-1.1/app_ordering/templates/admin/app_ordering/
--rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 14:16:40.000000 app_ordering-1.1/app_ordering/templates/admin/app_ordering/__init__.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.046950 app_ordering-1.1/app_ordering/templates/admin/app_ordering/profile/
--rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 14:16:49.000000 app_ordering-1.1/app_ordering/templates/admin/app_ordering/profile/__init__.py
--rw-r--r--   0 geek      (1000) geek      (1000)      713 2023-07-17 07:11:00.000000 app_ordering-1.1/app_ordering/templates/admin/app_ordering/profile/change_list.html
--rw-rw-r--   0 geek      (1000) geek      (1000)       60 2023-07-14 10:01:01.000000 app_ordering-1.1/app_ordering/tests.py
--rw-rw-r--   0 geek      (1000) geek      (1000)       63 2023-07-14 10:01:01.000000 app_ordering-1.1/app_ordering/views.py
-drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-07 04:33:11.042950 app_ordering-1.1/app_ordering.egg-info/
--rw-rw-r--   0 geek      (1000) geek      (1000)     1750 2023-08-07 04:33:11.000000 app_ordering-1.1/app_ordering.egg-info/PKG-INFO
--rw-rw-r--   0 geek      (1000) geek      (1000)     1046 2023-08-07 04:33:11.000000 app_ordering-1.1/app_ordering.egg-info/SOURCES.txt
--rw-rw-r--   0 geek      (1000) geek      (1000)        1 2023-08-07 04:33:11.000000 app_ordering-1.1/app_ordering.egg-info/dependency_links.txt
--rw-rw-r--   0 geek      (1000) geek      (1000)        1 2023-08-07 04:05:49.000000 app_ordering-1.1/app_ordering.egg-info/not-zip-safe
--rw-rw-r--   0 geek      (1000) geek      (1000)       42 2023-08-07 04:33:11.000000 app_ordering-1.1/app_ordering.egg-info/requires.txt
--rw-rw-r--   0 geek      (1000) geek      (1000)       13 2023-08-07 04:33:11.000000 app_ordering-1.1/app_ordering.egg-info/top_level.txt
--rw-r--r--   0 geek      (1000) geek      (1000)       79 2023-08-07 04:33:11.046950 app_ordering-1.1/setup.cfg
--rw-rw-r--   0 geek      (1000) geek      (1000)     1046 2023-08-07 04:32:44.000000 app_ordering-1.1/setup.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/
+-rw-r--r--   0 geek      (1000) geek      (1000)     1064 2023-08-07 04:12:21.000000 app_ordering-1.2/LICENSE.txt
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1750 2023-08-09 03:03:52.669835 app_ordering-1.2/PKG-INFO
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1393 2023-08-07 04:32:35.000000 app_ordering-1.2/README.md
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/
+-rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-14 10:01:01.000000 app_ordering-1.2/app_ordering/__init__.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)     2849 2023-08-09 02:55:01.000000 app_ordering-1.2/app_ordering/admin.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)     4231 2023-08-03 02:39:37.000000 app_ordering-1.2/app_ordering/apps.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      327 2023-08-03 03:09:49.000000 app_ordering-1.2/app_ordering/helpers.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/management/
+-rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 07:08:54.000000 app_ordering-1.2/app_ordering/management/__init__.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/management/commands/
+-rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 07:14:27.000000 app_ordering-1.2/app_ordering/management/commands/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      319 2023-07-17 09:17:30.000000 app_ordering-1.2/app_ordering/management/commands/sync_admin_apps.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/migrations/
+-rw-rw-r--   0 geek      (1000) geek      (1000)     5397 2023-07-17 10:52:21.000000 app_ordering-1.2/app_ordering/migrations/0001_initial.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1021 2023-07-17 11:08:54.000000 app_ordering-1.2/app_ordering/migrations/0002_alter_profile_groups_alter_profile_users.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-14 10:01:01.000000 app_ordering-1.2/app_ordering/migrations/__init__.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)     2702 2023-07-17 11:08:47.000000 app_ordering-1.2/app_ordering/models.py
+-rw-r--r--   0 geek      (1000) geek      (1000)     2950 2023-08-09 02:53:59.000000 app_ordering-1.2/app_ordering/services.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      365 2023-08-03 02:39:01.000000 app_ordering-1.2/app_ordering/signals.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/templates/
+-rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-17 13:47:46.000000 app_ordering-1.2/app_ordering/templates/__init__.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/templates/admin/
+-rw-rw-r--   0 geek      (1000) geek      (1000)        0 2023-07-17 13:47:46.000000 app_ordering-1.2/app_ordering/templates/admin/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)     2509 2023-07-17 08:53:15.000000 app_ordering-1.2/app_ordering/templates/admin/app_list.html
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/templates/admin/app_ordering/
+-rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 14:16:40.000000 app_ordering-1.2/app_ordering/templates/admin/app_ordering/__init__.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering/templates/admin/app_ordering/profile/
+-rw-r--r--   0 geek      (1000) geek      (1000)        0 2023-07-17 14:16:49.000000 app_ordering-1.2/app_ordering/templates/admin/app_ordering/profile/__init__.py
+-rw-r--r--   0 geek      (1000) geek      (1000)      713 2023-07-17 07:11:00.000000 app_ordering-1.2/app_ordering/templates/admin/app_ordering/profile/change_list.html
+-rw-rw-r--   0 geek      (1000) geek      (1000)       60 2023-07-14 10:01:01.000000 app_ordering-1.2/app_ordering/tests.py
+-rw-rw-r--   0 geek      (1000) geek      (1000)       63 2023-07-14 10:01:01.000000 app_ordering-1.2/app_ordering/views.py
+drwxrwxr-x   0 geek      (1000) geek      (1000)        0 2023-08-09 03:03:52.669835 app_ordering-1.2/app_ordering.egg-info/
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1750 2023-08-09 03:03:52.000000 app_ordering-1.2/app_ordering.egg-info/PKG-INFO
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1046 2023-08-09 03:03:52.000000 app_ordering-1.2/app_ordering.egg-info/SOURCES.txt
+-rw-rw-r--   0 geek      (1000) geek      (1000)        1 2023-08-09 03:03:52.000000 app_ordering-1.2/app_ordering.egg-info/dependency_links.txt
+-rw-rw-r--   0 geek      (1000) geek      (1000)        1 2023-08-07 04:05:49.000000 app_ordering-1.2/app_ordering.egg-info/not-zip-safe
+-rw-rw-r--   0 geek      (1000) geek      (1000)       42 2023-08-09 03:03:52.000000 app_ordering-1.2/app_ordering.egg-info/requires.txt
+-rw-rw-r--   0 geek      (1000) geek      (1000)       13 2023-08-09 03:03:52.000000 app_ordering-1.2/app_ordering.egg-info/top_level.txt
+-rw-r--r--   0 geek      (1000) geek      (1000)       79 2023-08-09 03:03:52.669835 app_ordering-1.2/setup.cfg
+-rw-rw-r--   0 geek      (1000) geek      (1000)     1046 2023-08-09 02:55:38.000000 app_ordering-1.2/setup.py
```

### Comparing `app_ordering-1.1/LICENSE.txt` & `app_ordering-1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/PKG-INFO` & `app_ordering-1.2/app_ordering.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: app_ordering
-Version: 1.1
+Name: app-ordering
+Version: 1.2
 Summary: Sorting and toggle visible for Django admin apps
 Home-page: https://github.com/kajalagroup/django-admin-app-ordering
 Author: Tuan Bach Van
 Author-email: tuan@kajala.com
 License: MIT licence, see LICENCE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `app_ordering-1.1/README.md` & `app_ordering-1.2/README.md`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/admin.py` & `app_ordering-1.2/app_ordering/admin.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,13 +77,15 @@
     inlines = [
         AdminModelInlineAdmin,
     ]
 
     def has_add_permission(self, request: HttpRequest) -> bool:
         return False
 
-    def has_delete_permission(self, request: HttpRequest, obj: Any | None = ...) -> bool:
-        return False
+    def changeform_view(self, request, object_id=None, form_url='', extra_context=None):
+        extra_context = extra_context or {}
+        extra_context['show_delete'] = False
+        return super().changeform_view(request, object_id, form_url, extra_context)
 
 
 admin.site.register(Profile, ProfileAdmin)
 admin.site.register(AdminApp, AdminAppAdmin)
```

### Comparing `app_ordering-1.1/app_ordering/apps.py` & `app_ordering-1.2/app_ordering/apps.py`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/migrations/0001_initial.py` & `app_ordering-1.2/app_ordering/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/migrations/0002_alter_profile_groups_alter_profile_users.py` & `app_ordering-1.2/app_ordering/migrations/0002_alter_profile_groups_alter_profile_users.py`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/models.py` & `app_ordering-1.2/app_ordering/models.py`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/services.py` & `app_ordering-1.2/app_ordering/services.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,22 +27,30 @@
     if len(inactive_admin_model_ids) > 0:
         AdminModel.objects.filter(pk__in=inactive_admin_model_ids).delete()
 
 
 def sync_apps(profile_id: Optional[int] = None):
     models = apps.get_models()
     map_app = {}
+    all_apps = []
     for model in models:
         if model in admin.site._registry:  # pylint: disable=protected-access
             app_label = model._meta.app_label
             object_name = model._meta.object_name
             if app_label not in map_app:
                 map_app[app_label] = []
+                all_apps.append(app_label)
             if object_name not in map_app[app_label]:
                 map_app[app_label].append(object_name)
+                
+    all_apps = sorted(all_apps)
+    
+    for app_label in map_app:
+        map_app[app_label] = sorted(map_app[app_label])
+
     profile_qs = Profile.objects.prefetch_related("admin_apps__admin_models")
     if profile_id:
         profile_qs.filter(pk=profile_id)
 
     for profile in profile_qs.all():
         active_app_labels = []
         inactive_app_ids = []
@@ -50,15 +58,15 @@
             assert isinstance(admin_app, AdminApp)
             if admin_app.app_label not in map_app:
                 inactive_app_ids.append(admin_app.pk)
             else:
                 active_app_labels.append(admin_app.app_label)
                 sync_models(admin_app, map_app[admin_app.app_label])
         next_order = profile.next_app_order
-        for app_label in map_app:
+        for app_label in all_apps:
             if app_label not in active_app_labels:
                 admin_app = AdminApp(profile=profile, app_label=app_label, order=next_order)
                 admin_app.save()
                 next_order += 1
                 sync_models(admin_app, map_app[admin_app.app_label])
                 logger.info('new app %s', admin_app)
         if len(inactive_app_ids) > 0:
```

### Comparing `app_ordering-1.1/app_ordering/templates/admin/app_list.html` & `app_ordering-1.2/app_ordering/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering/templates/admin/app_ordering/profile/change_list.html` & `app_ordering-1.2/app_ordering/templates/admin/app_ordering/profile/change_list.html`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/app_ordering.egg-info/PKG-INFO` & `app_ordering-1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: app-ordering
-Version: 1.1
+Name: app_ordering
+Version: 1.2
 Summary: Sorting and toggle visible for Django admin apps
 Home-page: https://github.com/kajalagroup/django-admin-app-ordering
 Author: Tuan Bach Van
 Author-email: tuan@kajala.com
 License: MIT licence, see LICENCE.txt
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `app_ordering-1.1/app_ordering.egg-info/SOURCES.txt` & `app_ordering-1.2/app_ordering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `app_ordering-1.1/setup.py` & `app_ordering-1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 install_requires = parse_requirements("requirements.txt", session=False)
 
 setup(
     name="app_ordering",
-    version="1.1",
+    version="1.2",
     author=u"Tuan Bach Van",
     author_email="tuan@kajala.com",
     packages=find_packages(exclude=["project", "venv"]),
     package_data={'app_ordering.templates.admin': ['*', '*/*', '*/*/*']},
     include_package_data=True,
     url="https://github.com/kajalagroup/django-admin-app-ordering",
     license="MIT licence, see LICENCE.txt",
```

