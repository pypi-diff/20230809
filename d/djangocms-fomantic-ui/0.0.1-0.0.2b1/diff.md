# Comparing `tmp/djangocms_fomantic_ui-0.0.1.tar.gz` & `tmp/djangocms_fomantic_ui-0.0.2b1.tar.gz`

## Comparing `djangocms_fomantic_ui-0.0.1.tar` & `djangocms_fomantic_ui-0.0.2b1.tar`

### file list

```diff
@@ -1,48 +1,46 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/README.md
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/admin.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/apps.py
--rw-r--r--   0        0        0    12577 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/cms_plugins.py
--rw-r--r--   0        0        0    38115 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/tests.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/views.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    18592 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/migrations/0001_initial.py
--rw-r--r--   0        0        0    62179 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/migrations/0001_squashed_0052_delete_event.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/migrations/0053_alter_accordionsection_title_and_more.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/migrations/__init__.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion_section.html
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/buttons.html
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/card.html
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/cards.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/column.html
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div_container.html
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/generic_plugin.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/row.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/segment.html
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/site_icons.html
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/statistic.html
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/step.html
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tab.html
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templatetags/djangocms_fomantic_ui.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/LICENSE.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/README.md
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/README.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/admin.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/apps.py
+-rw-r--r--   0        0        0    10984 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/cms_plugins.py
+-rw-r--r--   0        0        0    36760 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/tests.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/views.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    32755 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/migrations/__init__.py
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion_section.html
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/buttons.html
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/card.html
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/cards.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/column.html
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div_container.html
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/generic_plugin.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/row.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/segment.html
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/site_icons.html
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/statistic.html
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/step.html
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tab.html
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templatetags/djangocms_fomantic_ui.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/tests/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/LICENSE.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/README.md
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/PKG-INFO
```

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/admin.py` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/cms_plugins.py` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/cms_plugins.py`

 * *Files 18% similar despite different names*

```diff
@@ -359,53 +359,7 @@
     render_template = 'djangocms_fomantic_ui/generic_plugin.html'
     allow_children = True
     child_classes = ['StatisticPublisher']
 
     def render(self, context, instance, placeholder):
         context.update({'instance': instance})
         return context
-
-
-# @plugin_pool.register_plugin
-# class StaffPublisher(CMSPluginBase):
-#     module = _('Fomantic UI')
-#     name = _('Staff')
-#     render_template = 'djangocms_fomantic_ui/staff.html'
-#
-#     def render(self, context, instance, placeholder):
-#         staff_members = StaffMember.objects.filter(
-#             publish=True
-#         ).order_by('order', 'last_name', 'first_name')
-#         context.update({'staff_members': staff_members})
-#         return context
-#
-#
-# @plugin_pool.register_plugin
-# class StaffPublisherShape(StaffPublisher):
-#     module = _('Fomantic UI')
-#     render_template = 'djangocms_fomantic_ui/staff_shape.html'
-#     name = _('Staff Shape')
-
-
-# @plugin_pool.register_plugin
-# class PretixWidgetPublisher(CMSPluginBase):
-#     model: CMSPlugin = Event
-#     module: str = _('Fomantic UI')
-#     name: str = _('Pretix Widget')
-#     render_template: str = 'djangocms_fomantic_ui/pretix_widget.html'
-#
-#     def render(self, context: dict, instance, placeholder):
-#         context: dict = super(PretixWidgetPublisher,
-#                               self).render(context, instance, placeholder)
-#         language_code: str = get_language()
-#         if language_code not in ['en', 'de', 'zh-hans']:  # TODO: settings
-#             language_code = 'en'
-#         js_url: str = settings.PRETIX_WIDGET_JS_URL.format(
-#             language_code=language_code
-#         )
-#         context.update(
-#             {
-#                 'base_url': settings.PRETIX_WIDGET_BASE_URL,
-#                 'js_url': js_url
-#             }
-#         )
-#         return context
```

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/models.py` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1203,52 +1203,7 @@
 
     def get_classes(self):
         classes = ['ui']
         if self.horizontal:
             classes.append('horizontal')
         classes.append('statistics')
         return ' '.join(classes)
-
-
-# class StaffMember(TranslatableModel):
-#     title = models.CharField(max_length=20, blank=True, verbose_name=_('title'))
-#     first_name = models.CharField(
-#         max_length=50, blank=True, verbose_name=_('first name')
-#     )
-#     last_name = models.CharField(
-#         max_length=50,
-#         verbose_name=_('last name'),
-#         help_text=_('This is used for sorting')
-#     )
-#     order = models.SmallIntegerField(
-#         null=True,
-#         blank=True,
-#         verbose_name=_('order'),
-#         help_text=_('This takes precedence over sorting by last name.')
-#     )
-#     picture = FilerImageField(
-#         null=True,
-#         blank=True,
-#         verbose_name=_('picture'),
-#         on_delete=models.CASCADE
-#     )
-#     translations = TranslatedFields(
-#         info_text=HTMLField(blank=True, verbose_name=_('info text'))
-#     )
-#     publish = models.BooleanField(default=True, verbose_name=_('publish'))
-#
-#     class Meta:
-#         ordering = ['last_name', 'first_name']
-#
-#     def __str__(self):
-#         return f'{self.first_name} {self.last_name}'
-
-
-# class Event(CMSPlugin):
-#     slug = models.CharField(
-#         max_length=20,
-#         verbose_name=_('Short name'),
-#         help_text=_('Short name of the event, like defined in Pretix')
-#     )
-#
-#     def __str__(self):
-#         return self.slug
```

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html` & `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/LICENSE.txt` & `djangocms_fomantic_ui-0.0.2b1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/README.md` & `djangocms_fomantic_ui-0.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/pyproject.toml` & `djangocms_fomantic_ui-0.0.2b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.1/PKG-INFO` & `djangocms_fomantic_ui-0.0.2b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-fomantic-ui
-Version: 0.0.1
+Version: 0.0.2b1
 Project-URL: Documentation, https://github.com/MacLake/djangocms-fomantic-ui#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-fomantic-ui/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-fomantic-ui
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

