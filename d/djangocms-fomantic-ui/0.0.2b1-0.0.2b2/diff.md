# Comparing `tmp/djangocms_fomantic_ui-0.0.2b1.tar.gz` & `tmp/djangocms_fomantic_ui-0.0.2b2.tar.gz`

## Comparing `djangocms_fomantic_ui-0.0.2b1.tar` & `djangocms_fomantic_ui-0.0.2b2.tar`

### file list

```diff
@@ -1,46 +1,75 @@
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/README.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/__about__.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/__init__.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/admin.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/apps.py
--rw-r--r--   0        0        0    10984 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/cms_plugins.py
--rw-r--r--   0        0        0    36760 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/models.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/tests.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/views.py
--rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    32755 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/migrations/__init__.py
--rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion_section.html
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/buttons.html
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/card.html
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/cards.html
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/column.html
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div.html
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div_container.html
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/generic_plugin.html
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/row.html
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/segment.html
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/site_icons.html
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/statistic.html
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/step.html
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tab.html
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templatetags/djangocms_fomantic_ui.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/tests/__init__.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/.gitignore
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/LICENSE.txt
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/README.md
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/pyproject.toml
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b1/PKG-INFO
+-rw-r--r--   0        0        0   359731 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/package-lock.json
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/package.json
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/webpack.config.js
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/assets/src/index.js
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/README.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/__about__.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/__init__.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/admin.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/apps.py
+-rw-r--r--   0        0        0    10984 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/cms_plugins.py
+-rw-r--r--   0        0        0    36760 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/models.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/tests.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/views.py
+-rw-r--r--   0        0        0     5041 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17016 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    32755 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/migrations/__init__.py
+-rw-r--r--   0        0        0    78268 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/1551f4f60c37af51121f.woff2
+-rw-r--r--   0        0        0    89988 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/2285773e6b4b172f07d9.woff
+-rw-r--r--   0        0        0   303376 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/2e72ab08f6b108d7eef4.woff
+-rw-r--r--   0        0        0   290956 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/2fee7146711cc5c3dd41.woff
+-rw-r--r--   0        0        0   188332 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/330c031b5bb2b88046da.woff2
+-rw-r--r--   0        0        0   178044 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/43bc627160e4b7a28fbc.woff2
+-rw-r--r--   0        0        0   291164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/497f04acb55a3d00dfa3.woff
+-rw-r--r--   0        0        0    45632 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/4a38ade2ce0988376595.woff
+-rw-r--r--   0        0        0    33616 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/710a16565cff7fb7bf78.woff2
+-rw-r--r--   0        0        0    46980 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/720116e2e1990835048b.woff
+-rw-r--r--   0        0        0    13224 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/7a3337626410ca2f4071.woff2
+-rw-r--r--   0        0        0    45416 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/8525916133d63443ee21.woff
+-rw-r--r--   0        0        0   190608 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/978bab8c991c4aab7d12.woff2
+-rw-r--r--   0        0        0    46468 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/9bcbc975bb95fcc7bdbb.woff
+-rw-r--r--   0        0        0    33828 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/b0a598e91a6ca2310dc9.woff2
+-rw-r--r--   0        0        0    16276 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/bb932b70aeb593860dfe.woff2
+-rw-r--r--   0        0        0    76736 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/d878b0a6a1144760244f.woff2
+-rw-r--r--   0        0        0   308540 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/e67e575e2b5ee2fe795c.woff
+-rw-r--r--   0        0        0    34752 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/e83aa39dd6147ef2b674.woff2
+-rw-r--r--   0        0        0   101648 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0        0        0   178868 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/f846fe49520f593c671e.woff2
+-rw-r--r--   0        0        0  2074862 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/index.bundle.js
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/djangocms_fomantic_ui/webpack/index.bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0    11469 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion_section.html
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/buttons.html
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/card.html
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/cards.html
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/column.html
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div.html
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/div_container.html
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/fomantic-ui.html
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/generic_plugin.html
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/row.html
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/segment.html
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/site_icons.html
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/statistic.html
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/step.html
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tab.html
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templatetags/djangocms_fomantic_ui.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/tests/__init__.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/.gitignore
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/LICENSE.txt
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/README.md
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/pyproject.toml
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 djangocms_fomantic_ui-0.0.2b2/PKG-INFO
```

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/admin.py` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/admin.py`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/cms_plugins.py` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/models.py` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/models.py`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/migrations/0001_initial.py` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/static/phi_plugins/images/Stellaris_Clapper-board.svg`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/accordion.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/button.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/embed.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/icon.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/message.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/modal.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/reveal.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/staff_shape.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/steps.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html` & `djangocms_fomantic_ui-0.0.2b2/src/djangocms_fomantic_ui/templates/djangocms_fomantic_ui/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/LICENSE.txt` & `djangocms_fomantic_ui-0.0.2b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/README.md` & `djangocms_fomantic_ui-0.0.2b2/README.md`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/pyproject.toml` & `djangocms_fomantic_ui-0.0.2b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms_fomantic_ui-0.0.2b1/PKG-INFO` & `djangocms_fomantic_ui-0.0.2b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-fomantic-ui
-Version: 0.0.2b1
+Version: 0.0.2b2
 Project-URL: Documentation, https://github.com/MacLake/djangocms-fomantic-ui#readme
 Project-URL: Issues, https://github.com/MacLake/djangocms-fomantic-ui/issues
 Project-URL: Source, https://github.com/MacLake/djangocms-fomantic-ui
 Author-email: Jens-Erik Weber <Jens-Erik.Weber@passiv.de>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

