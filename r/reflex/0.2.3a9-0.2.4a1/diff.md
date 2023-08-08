# Comparing `tmp/reflex-0.2.3a9.tar.gz` & `tmp/reflex-0.2.4a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reflex-0.2.3a9.tar", max compression
+gzip compressed data, was "reflex-0.2.4a1.tar", max compression
```

## Comparing `reflex-0.2.3a9.tar` & `reflex-0.2.4a1.tar`

### file list

```diff
@@ -1,179 +1,180 @@
--rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.3a9/LICENSE
--rw-r--r--   0        0        0     7905 2023-07-25 18:50:56.099599 reflex-0.2.3a9/README.md
--rw-r--r--   0        0        0     2001 2023-07-31 02:51:35.668499 reflex-0.2.3a9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.3a9/reflex/.templates/apps/counter/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-27 23:45:03.452394 reflex-0.2.3a9/reflex/.templates/apps/counter/counter.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.3a9/reflex/.templates/apps/default/__init__.py
--rw-r--r--   0        0        0     1214 2023-07-27 23:45:03.453010 reflex-0.2.3a9/reflex/.templates/apps/default/default.py
--rw-r--r--   0        0        0    15406 2023-07-14 23:13:37.770037 reflex-0.2.3a9/reflex/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      181 2023-07-14 23:13:37.770146 reflex-0.2.3a9/reflex/.templates/jinja/app/rxconfig.py.jinja2
--rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/_document.js.jinja2
--rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/base_page.js.jinja2
--rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
--rw-r--r--   0        0        0     3312 2023-07-14 23:13:37.770458 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/index.js.jinja2
--rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.3a9/reflex/.templates/jinja/web/pages/utils.js.jinja2
--rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.3a9/reflex/.templates/jinja/web/tailwind.config.js.jinja2
--rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.3a9/reflex/.templates/jinja/web/utils/theme.js.jinja2
--rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.3a9/reflex/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.3a9/reflex/.templates/web/bun.lockb
--rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.3a9/reflex/.templates/web/jsconfig.json
--rw-r--r--   0        0        0       65 2023-07-21 22:05:26.060616 reflex-0.2.3a9/reflex/.templates/web/next.config.js
--rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.3a9/reflex/.templates/web/package.json
--rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.3a9/reflex/.templates/web/pages/404.js
--rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.3a9/reflex/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.3a9/reflex/.templates/web/postcss.config.js
--rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.3a9/reflex/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.3a9/reflex/.templates/web/styles/tailwind.css
--rw-r--r--   0        0        0    10172 2023-07-27 23:45:03.453483 reflex-0.2.3a9/reflex/.templates/web/utils/state.js
--rw-r--r--   0        0        0     1996 2023-07-27 23:45:03.454124 reflex-0.2.3a9/reflex/__init__.py
--rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.3a9/reflex/admin.py
--rw-r--r--   0        0        0    24864 2023-07-28 19:12:55.971292 reflex-0.2.3a9/reflex/app.py
--rw-r--r--   0        0        0     2438 2023-07-14 23:13:37.772635 reflex-0.2.3a9/reflex/base.py
--rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.3a9/reflex/compiler/__init__.py
--rw-r--r--   0        0        0     6604 2023-07-17 23:29:33.627133 reflex-0.2.3a9/reflex/compiler/compiler.py
--rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.3a9/reflex/compiler/templates.py
--rw-r--r--   0        0        0     8631 2023-07-19 01:58:26.539302 reflex-0.2.3a9/reflex/compiler/utils.py
--rw-r--r--   0        0        0     7595 2023-07-19 01:58:26.539650 reflex-0.2.3a9/reflex/components/__init__.py
--rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.3a9/reflex/components/base/__init__.py
--rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.3a9/reflex/components/base/bare.py
--rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.3a9/reflex/components/base/body.py
--rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.3a9/reflex/components/base/document.py
--rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.3a9/reflex/components/base/head.py
--rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.3a9/reflex/components/base/link.py
--rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.3a9/reflex/components/base/meta.py
--rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.3a9/reflex/components/base/script.py
--rw-r--r--   0        0        0    24321 2023-07-25 18:39:55.676277 reflex-0.2.3a9/reflex/components/component.py
--rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.3a9/reflex/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.3a9/reflex/components/datadisplay/badge.py
--rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.3a9/reflex/components/datadisplay/code.py
--rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.3a9/reflex/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.3a9/reflex/components/datadisplay/divider.py
--rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.3a9/reflex/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.3a9/reflex/components/datadisplay/list.py
--rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.3a9/reflex/components/datadisplay/stat.py
--rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.3a9/reflex/components/datadisplay/table.py
--rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.3a9/reflex/components/datadisplay/tag.py
--rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.3a9/reflex/components/disclosure/__init__.py
--rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.3a9/reflex/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.3a9/reflex/components/disclosure/tabs.py
--rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.3a9/reflex/components/disclosure/transition.py
--rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.3a9/reflex/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.3a9/reflex/components/feedback/__init__.py
--rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.3a9/reflex/components/feedback/alert.py
--rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.3a9/reflex/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.3a9/reflex/components/feedback/progress.py
--rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.3a9/reflex/components/feedback/skeleton.py
--rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.3a9/reflex/components/feedback/spinner.py
--rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.3a9/reflex/components/forms/__init__.py
--rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.3a9/reflex/components/forms/button.py
--rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.3a9/reflex/components/forms/checkbox.py
--rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.3a9/reflex/components/forms/colormodeswitch.py
--rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.3a9/reflex/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.3a9/reflex/components/forms/date_picker.py
--rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.3a9/reflex/components/forms/date_time_picker.py
--rw-r--r--   0        0        0     2627 2023-07-14 23:13:37.775352 reflex-0.2.3a9/reflex/components/forms/debounce.py
--rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.3a9/reflex/components/forms/editable.py
--rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.3a9/reflex/components/forms/email.py
--rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.3a9/reflex/components/forms/form.py
--rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.3a9/reflex/components/forms/iconbutton.py
--rw-r--r--   0        0        0     3246 2023-07-31 00:05:16.998188 reflex-0.2.3a9/reflex/components/forms/input.py
--rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.3a9/reflex/components/forms/multiselect.py
--rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.3a9/reflex/components/forms/numberinput.py
--rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.3a9/reflex/components/forms/password.py
--rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.3a9/reflex/components/forms/pininput.py
--rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.3a9/reflex/components/forms/radio.py
--rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.3a9/reflex/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.3a9/reflex/components/forms/select.py
--rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.3a9/reflex/components/forms/slider.py
--rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.3a9/reflex/components/forms/switch.py
--rw-r--r--   0        0        0     1526 2023-07-14 23:13:37.776244 reflex-0.2.3a9/reflex/components/forms/textarea.py
--rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.3a9/reflex/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.3a9/reflex/components/graphing/__init__.py
--rw-r--r--   0        0        0     1351 2023-07-14 23:13:37.776443 reflex-0.2.3a9/reflex/components/graphing/plotly.py
--rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.3a9/reflex/components/graphing/victory.py
--rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.3a9/reflex/components/layout/__init__.py
--rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.3a9/reflex/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.3a9/reflex/components/layout/box.py
--rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.3a9/reflex/components/layout/card.py
--rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.3a9/reflex/components/layout/center.py
--rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.3a9/reflex/components/layout/cond.py
--rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.3a9/reflex/components/layout/container.py
--rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.3a9/reflex/components/layout/flex.py
--rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.3a9/reflex/components/layout/foreach.py
--rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.3a9/reflex/components/layout/fragment.py
--rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.3a9/reflex/components/layout/grid.py
--rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.3a9/reflex/components/layout/html.py
--rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.3a9/reflex/components/layout/responsive.py
--rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.3a9/reflex/components/layout/spacer.py
--rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.3a9/reflex/components/layout/stack.py
--rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.3a9/reflex/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.3a9/reflex/components/libs/__init__.py
--rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.3a9/reflex/components/libs/chakra.py
--rw-r--r--   0        0        0     1385 2023-07-14 23:13:37.777604 reflex-0.2.3a9/reflex/components/libs/react_player.py
--rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.3a9/reflex/components/media/__init__.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.3a9/reflex/components/media/audio.py
--rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.3a9/reflex/components/media/avatar.py
--rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.3a9/reflex/components/media/icon.py
--rw-r--r--   0        0        0     2053 2023-07-14 23:13:37.777927 reflex-0.2.3a9/reflex/components/media/image.py
--rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.3a9/reflex/components/media/video.py
--rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.3a9/reflex/components/navigation/__init__.py
--rw-r--r--   0        0        0     2919 2023-07-29 01:05:18.595845 reflex-0.2.3a9/reflex/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.3a9/reflex/components/navigation/link.py
--rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.3a9/reflex/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.3a9/reflex/components/navigation/nextlink.py
--rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.3a9/reflex/components/navigation/stepper.py
--rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.3a9/reflex/components/overlay/__init__.py
--rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.3a9/reflex/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.3a9/reflex/components/overlay/banner.py
--rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.3a9/reflex/components/overlay/drawer.py
--rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.3a9/reflex/components/overlay/menu.py
--rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.3a9/reflex/components/overlay/modal.py
--rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.3a9/reflex/components/overlay/popover.py
--rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.3a9/reflex/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.3a9/reflex/components/tags/__init__.py
--rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.3a9/reflex/components/tags/cond_tag.py
--rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.3a9/reflex/components/tags/iter_tag.py
--rw-r--r--   0        0        0     5150 2023-07-27 23:45:03.454877 reflex-0.2.3a9/reflex/components/tags/tag.py
--rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.3a9/reflex/components/tags/tagless.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.3a9/reflex/components/typography/__init__.py
--rw-r--r--   0        0        0      348 2023-07-27 23:45:03.455160 reflex-0.2.3a9/reflex/components/typography/heading.py
--rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.3a9/reflex/components/typography/highlight.py
--rw-r--r--   0        0        0     4679 2023-07-27 23:45:03.455385 reflex-0.2.3a9/reflex/components/typography/markdown.py
--rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.3a9/reflex/components/typography/span.py
--rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.3a9/reflex/components/typography/text.py
--rw-r--r--   0        0        0     7564 2023-07-27 23:45:03.455544 reflex-0.2.3a9/reflex/config.py
--rw-r--r--   0        0        0    12431 2023-07-31 02:59:56.786376 reflex-0.2.3a9/reflex/constants.py
--rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.3a9/reflex/el/__init__.py
--rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.3a9/reflex/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.3a9/reflex/el/constants/html.py
--rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.3a9/reflex/el/constants/react.py
--rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.3a9/reflex/el/constants/reflex.py
--rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.3a9/reflex/el/element.py
--rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.3a9/reflex/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.3a9/reflex/el/precompile.py
--rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.3a9/reflex/event.py
--rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.3a9/reflex/middleware/__init__.py
--rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.3a9/reflex/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.3a9/reflex/middleware/middleware.py
--rw-r--r--   0        0        0     9598 2023-07-31 02:59:56.786564 reflex-0.2.3a9/reflex/model.py
--rw-r--r--   0        0        0     1832 2023-07-27 23:45:03.455818 reflex-0.2.3a9/reflex/page.py
--rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.3a9/reflex/py.typed
--rw-r--r--   0        0        0    10623 2023-07-31 02:59:56.786732 reflex-0.2.3a9/reflex/reflex.py
--rw-r--r--   0        0        0     3934 2023-07-27 23:45:03.456240 reflex-0.2.3a9/reflex/route.py
--rw-r--r--   0        0        0    32524 2023-07-29 03:11:02.108051 reflex-0.2.3a9/reflex/state.py
--rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.3a9/reflex/style.py
--rw-r--r--   0        0        0    15133 2023-07-31 02:59:56.786903 reflex-0.2.3a9/reflex/testing.py
--rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.3a9/reflex/utils/__init__.py
--rw-r--r--   0        0        0     6212 2023-07-31 02:59:56.787060 reflex-0.2.3a9/reflex/utils/build.py
--rw-r--r--   0        0        0     3964 2023-07-31 02:59:56.787200 reflex-0.2.3a9/reflex/utils/console.py
--rw-r--r--   0        0        0     3774 2023-07-31 02:59:56.787338 reflex-0.2.3a9/reflex/utils/exec.py
--rw-r--r--   0        0        0    12342 2023-07-29 01:05:18.597732 reflex-0.2.3a9/reflex/utils/format.py
--rw-r--r--   0        0        0      590 2023-07-27 23:45:03.457502 reflex-0.2.3a9/reflex/utils/imports.py
--rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.3a9/reflex/utils/path_ops.py
--rw-r--r--   0        0        0    16616 2023-07-31 02:59:56.787507 reflex-0.2.3a9/reflex/utils/prerequisites.py
--rw-r--r--   0        0        0     6485 2023-07-31 02:59:56.787667 reflex-0.2.3a9/reflex/utils/processes.py
--rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.3a9/reflex/utils/telemetry.py
--rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.3a9/reflex/utils/types.py
--rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.3a9/reflex/utils/watch.py
--rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.3a9/reflex/vars.py
--rw-r--r--   0        0        0     9725 1970-01-01 00:00:00.000000 reflex-0.2.3a9/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-14 23:13:37.760267 reflex-0.2.4a1/LICENSE
+-rw-r--r--   0        0        0     8037 2023-08-07 21:39:55.276419 reflex-0.2.4a1/README.md
+-rw-r--r--   0        0        0     2001 2023-08-08 22:32:11.126503 reflex-0.2.4a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769763 reflex-0.2.4a1/reflex/.templates/apps/counter/__init__.py
+-rw-r--r--   0        0        0     1326 2023-08-01 01:04:16.279921 reflex-0.2.4a1/reflex/.templates/apps/counter/counter.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.769883 reflex-0.2.4a1/reflex/.templates/apps/default/__init__.py
+-rw-r--r--   0        0        0     1214 2023-07-27 23:45:03.453010 reflex-0.2.4a1/reflex/.templates/apps/default/default.py
+-rw-r--r--   0        0        0    15086 2023-08-01 00:52:11.115619 reflex-0.2.4a1/reflex/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      128 2023-08-07 21:39:55.290398 reflex-0.2.4a1/reflex/.templates/jinja/app/rxconfig.py.jinja2
+-rw-r--r--   0        0        0      182 2023-07-14 23:13:37.770264 reflex-0.2.4a1/reflex/.templates/jinja/web/pages/_document.js.jinja2
+-rw-r--r--   0        0        0      241 2023-07-14 23:13:37.770322 reflex-0.2.4a1/reflex/.templates/jinja/web/pages/base_page.js.jinja2
+-rw-r--r--   0        0        0      252 2023-07-14 23:13:37.770383 reflex-0.2.4a1/reflex/.templates/jinja/web/pages/custom_component.js.jinja2
+-rw-r--r--   0        0        0     3405 2023-08-07 21:39:55.290804 reflex-0.2.4a1/reflex/.templates/jinja/web/pages/index.js.jinja2
+-rw-r--r--   0        0        0     3170 2023-07-14 23:13:37.770519 reflex-0.2.4a1/reflex/.templates/jinja/web/pages/utils.js.jinja2
+-rw-r--r--   0        0        0      356 2023-07-14 23:13:37.770572 reflex-0.2.4a1/reflex/.templates/jinja/web/tailwind.config.js.jinja2
+-rw-r--r--   0        0        0       38 2023-07-14 23:13:37.770645 reflex-0.2.4a1/reflex/.templates/jinja/web/utils/theme.js.jinja2
+-rw-r--r--   0        0        0      417 2023-07-14 23:13:37.770733 reflex-0.2.4a1/reflex/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   284503 2023-07-18 01:18:12.037548 reflex-0.2.4a1/reflex/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       50 2023-07-14 23:13:37.771627 reflex-0.2.4a1/reflex/.templates/web/jsconfig.json
+-rw-r--r--   0        0        0       65 2023-08-04 21:44:19.109421 reflex-0.2.4a1/reflex/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1287 2023-07-23 00:56:20.970158 reflex-0.2.4a1/reflex/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2023-07-21 22:29:32.048334 reflex-0.2.4a1/reflex/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      597 2023-07-14 23:13:37.771876 reflex-0.2.4a1/reflex/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       82 2023-07-14 23:13:37.771931 reflex-0.2.4a1/reflex/.templates/web/postcss.config.js
+-rw-r--r--   0        0        0    29404 2023-07-14 23:13:37.772115 reflex-0.2.4a1/reflex/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0       59 2023-07-14 23:13:37.772177 reflex-0.2.4a1/reflex/.templates/web/styles/tailwind.css
+-rw-r--r--   0        0        0    10172 2023-08-04 22:58:57.272692 reflex-0.2.4a1/reflex/.templates/web/utils/state.js
+-rw-r--r--   0        0        0     1995 2023-08-07 21:39:55.291182 reflex-0.2.4a1/reflex/__init__.py
+-rw-r--r--   0        0        0      108 2023-08-07 21:39:55.291570 reflex-0.2.4a1/reflex/__main__.py
+-rw-r--r--   0        0        0      373 2023-07-14 23:13:37.772422 reflex-0.2.4a1/reflex/admin.py
+-rw-r--r--   0        0        0    24864 2023-08-01 16:45:11.246662 reflex-0.2.4a1/reflex/app.py
+-rw-r--r--   0        0        0     2438 2023-08-01 02:16:53.895976 reflex-0.2.4a1/reflex/base.py
+-rw-r--r--   0        0        0       27 2023-07-14 23:13:37.772707 reflex-0.2.4a1/reflex/compiler/__init__.py
+-rw-r--r--   0        0        0     6604 2023-08-04 22:58:57.273332 reflex-0.2.4a1/reflex/compiler/compiler.py
+-rw-r--r--   0        0        0     2725 2023-07-25 18:39:55.667575 reflex-0.2.4a1/reflex/compiler/templates.py
+-rw-r--r--   0        0        0     8631 2023-08-04 22:58:57.273585 reflex-0.2.4a1/reflex/compiler/utils.py
+-rw-r--r--   0        0        0     7651 2023-08-07 22:05:16.945390 reflex-0.2.4a1/reflex/components/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-19 01:58:26.539880 reflex-0.2.4a1/reflex/components/base/__init__.py
+-rw-r--r--   0        0        0      719 2023-07-14 23:13:37.773188 reflex-0.2.4a1/reflex/components/base/bare.py
+-rw-r--r--   0        0        0      151 2023-07-14 23:13:37.773235 reflex-0.2.4a1/reflex/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-07-19 01:58:26.540063 reflex-0.2.4a1/reflex/components/base/document.py
+-rw-r--r--   0        0        0      263 2023-07-14 23:13:37.773334 reflex-0.2.4a1/reflex/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-07-14 23:13:37.773386 reflex-0.2.4a1/reflex/components/base/link.py
+-rw-r--r--   0        0        0     1408 2023-07-14 23:13:37.773437 reflex-0.2.4a1/reflex/components/base/meta.py
+-rw-r--r--   0        0        0     2775 2023-07-19 01:58:26.540185 reflex-0.2.4a1/reflex/components/base/script.py
+-rw-r--r--   0        0        0    25014 2023-08-07 22:05:16.946189 reflex-0.2.4a1/reflex/components/component.py
+-rw-r--r--   0        0        0      496 2023-07-14 23:13:37.773654 reflex-0.2.4a1/reflex/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      330 2023-07-14 23:13:37.773723 reflex-0.2.4a1/reflex/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     3495 2023-07-25 18:39:55.680665 reflex-0.2.4a1/reflex/components/datadisplay/code.py
+-rw-r--r--   0        0        0     3951 2023-07-21 18:51:53.047714 reflex-0.2.4a1/reflex/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      533 2023-07-14 23:13:37.773921 reflex-0.2.4a1/reflex/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      185 2023-07-14 23:13:37.773974 reflex-0.2.4a1/reflex/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1422 2023-07-14 23:13:37.774028 reflex-0.2.4a1/reflex/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2151 2023-07-14 23:13:37.774087 reflex-0.2.4a1/reflex/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     6046 2023-07-20 20:03:35.348764 reflex-0.2.4a1/reflex/components/datadisplay/table.py
+-rw-r--r--   0        0        0     2182 2023-07-14 23:13:37.774210 reflex-0.2.4a1/reflex/components/datadisplay/tag.py
+-rw-r--r--   0        0        0      384 2023-07-14 23:13:37.774286 reflex-0.2.4a1/reflex/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     3511 2023-07-14 23:13:37.774347 reflex-0.2.4a1/reflex/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2771 2023-07-14 23:13:37.774404 reflex-0.2.4a1/reflex/components/disclosure/tabs.py
+-rw-r--r--   0        0        0     1737 2023-07-14 23:13:37.774459 reflex-0.2.4a1/reflex/components/disclosure/transition.py
+-rw-r--r--   0        0        0      283 2023-07-14 23:13:37.774510 reflex-0.2.4a1/reflex/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2023-07-14 23:13:37.774594 reflex-0.2.4a1/reflex/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1546 2023-07-19 01:58:26.540763 reflex-0.2.4a1/reflex/components/feedback/alert.py
+-rw-r--r--   0        0        0     1899 2023-07-14 23:13:37.774714 reflex-0.2.4a1/reflex/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      875 2023-07-14 23:13:37.774769 reflex-0.2.4a1/reflex/components/feedback/progress.py
+-rw-r--r--   0        0        0     1781 2023-07-14 23:13:37.774821 reflex-0.2.4a1/reflex/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      674 2023-07-14 23:13:37.774872 reflex-0.2.4a1/reflex/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1573 2023-07-14 23:13:37.774956 reflex-0.2.4a1/reflex/components/forms/__init__.py
+-rw-r--r--   0        0        0     1761 2023-07-14 23:13:37.775013 reflex-0.2.4a1/reflex/components/forms/button.py
+-rw-r--r--   0        0        0     2448 2023-07-14 23:13:37.775073 reflex-0.2.4a1/reflex/components/forms/checkbox.py
+-rw-r--r--   0        0        0     3137 2023-07-14 23:13:37.775129 reflex-0.2.4a1/reflex/components/forms/colormodeswitch.py
+-rw-r--r--   0        0        0      574 2023-07-14 23:13:37.775183 reflex-0.2.4a1/reflex/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775234 reflex-0.2.4a1/reflex/components/forms/date_picker.py
+-rw-r--r--   0        0        0      273 2023-07-14 23:13:37.775287 reflex-0.2.4a1/reflex/components/forms/date_time_picker.py
+-rw-r--r--   0        0        0     3702 2023-08-08 22:32:02.863751 reflex-0.2.4a1/reflex/components/forms/debounce.py
+-rw-r--r--   0        0        0     1943 2023-07-14 23:13:37.775412 reflex-0.2.4a1/reflex/components/forms/editable.py
+-rw-r--r--   0        0        0      239 2023-07-14 23:13:37.775465 reflex-0.2.4a1/reflex/components/forms/email.py
+-rw-r--r--   0        0        0     2990 2023-07-14 23:13:37.775521 reflex-0.2.4a1/reflex/components/forms/form.py
+-rw-r--r--   0        0        0      798 2023-07-14 23:13:37.775579 reflex-0.2.4a1/reflex/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     3948 2023-08-08 22:32:02.863964 reflex-0.2.4a1/reflex/components/forms/input.py
+-rw-r--r--   0        0        0    12659 2023-07-14 23:13:37.775734 reflex-0.2.4a1/reflex/components/forms/multiselect.py
+-rw-r--r--   0        0        0     3889 2023-07-14 23:13:37.775802 reflex-0.2.4a1/reflex/components/forms/numberinput.py
+-rw-r--r--   0        0        0      249 2023-07-14 23:13:37.775849 reflex-0.2.4a1/reflex/components/forms/password.py
+-rw-r--r--   0        0        0     2662 2023-07-14 23:13:37.775908 reflex-0.2.4a1/reflex/components/forms/pininput.py
+-rw-r--r--   0        0        0     3029 2023-07-14 23:13:37.775964 reflex-0.2.4a1/reflex/components/forms/radio.py
+-rw-r--r--   0        0        0     2845 2023-07-14 23:13:37.776021 reflex-0.2.4a1/reflex/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3510 2023-07-14 23:13:37.776068 reflex-0.2.4a1/reflex/components/forms/select.py
+-rw-r--r--   0        0        0     3116 2023-07-14 23:13:37.776140 reflex-0.2.4a1/reflex/components/forms/slider.py
+-rw-r--r--   0        0        0     1567 2023-07-14 23:13:37.776193 reflex-0.2.4a1/reflex/components/forms/switch.py
+-rw-r--r--   0        0        0     2228 2023-08-07 22:05:16.946880 reflex-0.2.4a1/reflex/components/forms/textarea.py
+-rw-r--r--   0        0        0     2905 2023-07-14 23:13:37.776307 reflex-0.2.4a1/reflex/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-07-14 23:13:37.776385 reflex-0.2.4a1/reflex/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1146 2023-08-04 23:50:22.462091 reflex-0.2.4a1/reflex/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17354 2023-07-14 23:13:37.776536 reflex-0.2.4a1/reflex/components/graphing/victory.py
+-rw-r--r--   0        0        0      872 2023-07-14 23:13:37.776623 reflex-0.2.4a1/reflex/components/layout/__init__.py
+-rw-r--r--   0        0        0      320 2023-07-14 23:13:37.776678 reflex-0.2.4a1/reflex/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      760 2023-07-14 23:13:37.776730 reflex-0.2.4a1/reflex/components/layout/box.py
+-rw-r--r--   0        0        0     2853 2023-07-14 23:13:37.776787 reflex-0.2.4a1/reflex/components/layout/card.py
+-rw-r--r--   0        0        0      394 2023-07-14 23:13:37.776833 reflex-0.2.4a1/reflex/components/layout/center.py
+-rw-r--r--   0        0        0     3832 2023-07-14 23:13:37.776892 reflex-0.2.4a1/reflex/components/layout/cond.py
+-rw-r--r--   0        0        0      359 2023-07-14 23:13:37.776948 reflex-0.2.4a1/reflex/components/layout/container.py
+-rw-r--r--   0        0        0      652 2023-07-14 23:13:37.776999 reflex-0.2.4a1/reflex/components/layout/flex.py
+-rw-r--r--   0        0        0     3159 2023-07-22 02:58:05.741564 reflex-0.2.4a1/reflex/components/layout/foreach.py
+-rw-r--r--   0        0        0      312 2023-07-14 23:13:37.777113 reflex-0.2.4a1/reflex/components/layout/fragment.py
+-rw-r--r--   0        0        0     4323 2023-07-14 23:13:37.777175 reflex-0.2.4a1/reflex/components/layout/grid.py
+-rw-r--r--   0        0        0      977 2023-07-14 23:13:37.777231 reflex-0.2.4a1/reflex/components/layout/html.py
+-rw-r--r--   0        0        0     1898 2023-07-14 23:13:37.777279 reflex-0.2.4a1/reflex/components/layout/responsive.py
+-rw-r--r--   0        0        0      184 2023-07-14 23:13:37.777323 reflex-0.2.4a1/reflex/components/layout/spacer.py
+-rw-r--r--   0        0        0      991 2023-07-14 23:13:37.777374 reflex-0.2.4a1/reflex/components/layout/stack.py
+-rw-r--r--   0        0        0     1465 2023-07-14 23:13:37.777429 reflex-0.2.4a1/reflex/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2023-07-14 23:13:37.777503 reflex-0.2.4a1/reflex/components/libs/__init__.py
+-rw-r--r--   0        0        0      220 2023-07-14 23:13:37.777552 reflex-0.2.4a1/reflex/components/libs/chakra.py
+-rw-r--r--   0        0        0     1070 2023-08-01 00:52:11.116784 reflex-0.2.4a1/reflex/components/libs/react_player.py
+-rw-r--r--   0        0        0      240 2023-07-14 23:13:37.777685 reflex-0.2.4a1/reflex/components/media/__init__.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777734 reflex-0.2.4a1/reflex/components/media/audio.py
+-rw-r--r--   0        0        0     1520 2023-07-14 23:13:37.777790 reflex-0.2.4a1/reflex/components/media/avatar.py
+-rw-r--r--   0        0        0     2387 2023-07-14 23:13:37.777859 reflex-0.2.4a1/reflex/components/media/icon.py
+-rw-r--r--   0        0        0     2105 2023-08-07 21:39:55.293304 reflex-0.2.4a1/reflex/components/media/image.py
+-rw-r--r--   0        0        0      195 2023-07-14 23:13:37.777986 reflex-0.2.4a1/reflex/components/media/video.py
+-rw-r--r--   0        0        0      450 2023-07-14 23:13:37.778063 reflex-0.2.4a1/reflex/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2919 2023-07-29 01:05:18.595845 reflex-0.2.4a1/reflex/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1602 2023-07-14 23:13:37.778175 reflex-0.2.4a1/reflex/components/navigation/link.py
+-rw-r--r--   0        0        0      526 2023-07-14 23:13:37.778225 reflex-0.2.4a1/reflex/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      503 2023-07-14 23:13:37.778277 reflex-0.2.4a1/reflex/components/navigation/nextlink.py
+-rw-r--r--   0        0        0     2836 2023-07-14 23:13:37.778336 reflex-0.2.4a1/reflex/components/navigation/stepper.py
+-rw-r--r--   0        0        0      887 2023-07-14 23:13:37.778422 reflex-0.2.4a1/reflex/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5019 2023-07-14 23:13:37.778510 reflex-0.2.4a1/reflex/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     1008 2023-07-14 23:13:37.778561 reflex-0.2.4a1/reflex/components/overlay/banner.py
+-rw-r--r--   0        0        0     4673 2023-07-14 23:13:37.778619 reflex-0.2.4a1/reflex/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5524 2023-07-14 23:13:37.778690 reflex-0.2.4a1/reflex/components/overlay/menu.py
+-rw-r--r--   0        0        0     4909 2023-07-14 23:13:37.778744 reflex-0.2.4a1/reflex/components/overlay/modal.py
+-rw-r--r--   0        0        0     5682 2023-07-14 23:13:37.778818 reflex-0.2.4a1/reflex/components/overlay/popover.py
+-rw-r--r--   0        0        0     1945 2023-07-14 23:13:37.778874 reflex-0.2.4a1/reflex/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2023-07-14 23:13:37.778947 reflex-0.2.4a1/reflex/components/tags/__init__.py
+-rw-r--r--   0        0        0      447 2023-07-14 23:13:37.779004 reflex-0.2.4a1/reflex/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     2306 2023-07-24 16:26:04.843847 reflex-0.2.4a1/reflex/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     5150 2023-08-01 01:10:31.754579 reflex-0.2.4a1/reflex/components/tags/tag.py
+-rw-r--r--   0        0        0      587 2023-07-14 23:13:37.779176 reflex-0.2.4a1/reflex/components/tags/tagless.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779262 reflex-0.2.4a1/reflex/components/typography/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-27 23:45:03.455160 reflex-0.2.4a1/reflex/components/typography/heading.py
+-rw-r--r--   0        0        0      676 2023-07-14 23:13:37.779367 reflex-0.2.4a1/reflex/components/typography/highlight.py
+-rw-r--r--   0        0        0     4679 2023-07-27 23:45:03.455385 reflex-0.2.4a1/reflex/components/typography/markdown.py
+-rw-r--r--   0        0        0      333 2023-07-14 23:13:37.779494 reflex-0.2.4a1/reflex/components/typography/span.py
+-rw-r--r--   0        0        0      302 2023-07-14 23:13:37.779551 reflex-0.2.4a1/reflex/components/typography/text.py
+-rw-r--r--   0        0        0     7740 2023-08-07 22:05:16.947584 reflex-0.2.4a1/reflex/config.py
+-rw-r--r--   0        0        0    12431 2023-07-31 02:59:56.786376 reflex-0.2.4a1/reflex/constants.py
+-rw-r--r--   0        0        0       73 2023-07-14 23:13:37.779820 reflex-0.2.4a1/reflex/el/__init__.py
+-rw-r--r--   0        0        0      113 2023-07-14 23:13:37.779899 reflex-0.2.4a1/reflex/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-07-14 23:13:37.779984 reflex-0.2.4a1/reflex/el/constants/html.py
+-rw-r--r--   0        0        0    15554 2023-07-14 23:13:37.780082 reflex-0.2.4a1/reflex/el/constants/react.py
+-rw-r--r--   0        0        0     1717 2023-07-14 23:13:37.780152 reflex-0.2.4a1/reflex/el/constants/reflex.py
+-rw-r--r--   0        0        0     1318 2023-07-14 23:13:37.780228 reflex-0.2.4a1/reflex/el/element.py
+-rw-r--r--   0        0        0   106323 2023-07-14 23:13:37.780493 reflex-0.2.4a1/reflex/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2655 2023-07-14 23:13:37.780585 reflex-0.2.4a1/reflex/el/precompile.py
+-rw-r--r--   0        0        0    13398 2023-07-14 23:13:37.780692 reflex-0.2.4a1/reflex/event.py
+-rw-r--r--   0        0        0      111 2023-07-14 23:13:37.780772 reflex-0.2.4a1/reflex/middleware/__init__.py
+-rw-r--r--   0        0        0     1726 2023-07-14 23:13:37.780837 reflex-0.2.4a1/reflex/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1157 2023-07-14 23:13:37.780910 reflex-0.2.4a1/reflex/middleware/middleware.py
+-rw-r--r--   0        0        0     9598 2023-07-31 19:03:43.654374 reflex-0.2.4a1/reflex/model.py
+-rw-r--r--   0        0        0     1832 2023-07-27 23:45:03.455818 reflex-0.2.4a1/reflex/page.py
+-rw-r--r--   0        0        0        0 2023-07-14 23:13:37.781036 reflex-0.2.4a1/reflex/py.typed
+-rw-r--r--   0        0        0    10771 2023-08-07 21:39:55.293843 reflex-0.2.4a1/reflex/reflex.py
+-rw-r--r--   0        0        0     3934 2023-07-27 23:45:03.456240 reflex-0.2.4a1/reflex/route.py
+-rw-r--r--   0        0        0    32475 2023-08-07 21:39:55.294228 reflex-0.2.4a1/reflex/state.py
+-rw-r--r--   0        0        0     1113 2023-07-14 23:13:37.781487 reflex-0.2.4a1/reflex/style.py
+-rw-r--r--   0        0        0    15279 2023-08-07 22:05:16.947753 reflex-0.2.4a1/reflex/testing.py
+-rw-r--r--   0        0        0       24 2023-07-14 23:13:37.781705 reflex-0.2.4a1/reflex/utils/__init__.py
+-rw-r--r--   0        0        0     6275 2023-08-07 21:39:55.295372 reflex-0.2.4a1/reflex/utils/build.py
+-rw-r--r--   0        0        0     3957 2023-08-07 21:39:55.295925 reflex-0.2.4a1/reflex/utils/console.py
+-rw-r--r--   0        0        0     3780 2023-08-07 21:39:55.296388 reflex-0.2.4a1/reflex/utils/exec.py
+-rw-r--r--   0        0        0    12342 2023-07-29 01:05:18.597732 reflex-0.2.4a1/reflex/utils/format.py
+-rw-r--r--   0        0        0      590 2023-07-27 23:45:03.457502 reflex-0.2.4a1/reflex/utils/imports.py
+-rw-r--r--   0        0        0     2429 2023-07-14 23:13:37.782189 reflex-0.2.4a1/reflex/utils/path_ops.py
+-rw-r--r--   0        0        0    17107 2023-08-07 21:39:55.296905 reflex-0.2.4a1/reflex/utils/prerequisites.py
+-rw-r--r--   0        0        0     7492 2023-08-07 21:39:55.297513 reflex-0.2.4a1/reflex/utils/processes.py
+-rw-r--r--   0        0        0     2362 2023-07-14 23:13:37.782441 reflex-0.2.4a1/reflex/utils/telemetry.py
+-rw-r--r--   0        0        0     4804 2023-07-14 23:13:37.782520 reflex-0.2.4a1/reflex/utils/types.py
+-rw-r--r--   0        0        0     2632 2023-07-14 23:13:37.782576 reflex-0.2.4a1/reflex/utils/watch.py
+-rw-r--r--   0        0        0    32892 2023-07-20 19:47:34.342520 reflex-0.2.4a1/reflex/vars.py
+-rw-r--r--   0        0        0     9857 1970-01-01 00:00:00.000000 reflex-0.2.4a1/PKG-INFO
```

### Comparing `reflex-0.2.3a9/LICENSE` & `reflex-0.2.4a1/LICENSE`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/README.md` & `reflex-0.2.4a1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,495 +1,503 @@
 00000000: 6060 6064 6966 660a 2b20 5365 6172 6368  ```diff.+ Search
 00000010: 696e 6720 666f 7220 5079 6e65 636f 6e65  ing for Pynecone
 00000020: 3f20 596f 7520 6172 6520 696e 2074 6865  ? You are in the
 00000030: 2072 6967 6874 2072 6570 6f2e 2050 796e   right repo. Pyn
 00000040: 6563 6f6e 6520 6861 7320 6265 656e 2072  econe has been r
 00000050: 656e 616d 6564 2074 6f20 5265 666c 6578  enamed to Reflex
 00000060: 2e20 2b0a 6060 600a 0a3c 6469 7620 616c  . +.```..<div al
-00000070: 6967 6e3d 2263 656e 7465 7222 3e0a 0a3c  ign="center">..<
-00000080: 696d 6720 7372 633d 2264 6f63 732f 696d  img src="docs/im
-00000090: 6167 6573 2f72 6566 6c65 782e 706e 6722  ages/reflex.png"
-000000a0: 3e0a 3c68 723e 0a0a 2320 2a2a 5265 666c  >.<hr>..# **Refl
-000000b0: 6578 2a2a 200a 2a2a e29c a820 5065 7266  ex** .**... Perf
-000000c0: 6f72 6d61 6e74 2c20 6375 7374 6f6d 697a  ormant, customiz
-000000d0: 6162 6c65 2077 6562 2061 7070 7320 696e  able web apps in
-000000e0: 2070 7572 6520 5079 7468 6f6e 2e20 4465   pure Python. De
-000000f0: 706c 6f79 2069 6e20 7365 636f 6e64 732e  ploy in seconds.
-00000100: 2a2a 0a0a f09f 9391 205b 446f 6373 5d28  **...... [Docs](
-00000110: 6874 7470 733a 2f2f 7265 666c 6578 2e64  https://reflex.d
-00000120: 6576 2f64 6f63 732f 6765 7474 696e 672d  ev/docs/getting-
-00000130: 7374 6172 7465 642f 696e 7472 6f64 7563  started/introduc
-00000140: 7469 6f6e 2920 266e 6273 703b 20f0 9f93  tion) &nbsp; ...
-00000150: b120 5b43 6f6d 706f 6e65 6e74 204c 6962  . [Component Lib
-00000160: 7261 7279 5d28 6874 7470 733a 2f2f 7265  rary](https://re
-00000170: 666c 6578 2e64 6576 2f64 6f63 732f 6c69  flex.dev/docs/li
-00000180: 6272 6172 7929 2026 6e62 7370 3b20 f09f  brary) &nbsp; ..
-00000190: 96bc efb8 8f20 5b47 616c 6c65 7279 5d28  ..... [Gallery](
-000001a0: 6874 7470 733a 2f2f 7265 666c 6578 2e64  https://reflex.d
-000001b0: 6576 2f64 6f63 732f 6761 6c6c 6572 7929  ev/docs/gallery)
-000001c0: 2026 6e62 7370 3b20 f09f 9bb8 205b 4465   &nbsp; .... [De
-000001d0: 706c 6f79 6d65 6e74 5d28 6874 7470 733a  ployment](https:
-000001e0: 2f2f 7265 666c 6578 2e64 6576 2f64 6f63  //reflex.dev/doc
-000001f0: 732f 686f 7374 696e 672f 6465 706c 6f79  s/hosting/deploy
-00000200: 290a 0a5b 215b 5079 5049 2076 6572 7369  )..[![PyPI versi
-00000210: 6f6e 5d28 6874 7470 733a 2f2f 6261 6467  on](https://badg
-00000220: 652e 6675 7279 2e69 6f2f 7079 2f72 6566  e.fury.io/py/ref
-00000230: 6c65 782e 7376 6729 5d28 6874 7470 733a  lex.svg)](https:
-00000240: 2f2f 6261 6467 652e 6675 7279 2e69 6f2f  //badge.fury.io/
-00000250: 7079 2f72 6566 6c65 7829 0a21 5b74 6573  py/reflex).![tes
-00000260: 7473 5d28 6874 7470 733a 2f2f 6769 7468  ts](https://gith
-00000270: 7562 2e63 6f6d 2f70 796e 6563 6f6e 652d  ub.com/pynecone-
-00000280: 696f 2f70 796e 6563 6f6e 652f 6163 7469  io/pynecone/acti
-00000290: 6f6e 732f 776f 726b 666c 6f77 732f 6275  ons/workflows/bu
-000002a0: 696c 642e 796d 6c2f 6261 6467 652e 7376  ild.yml/badge.sv
-000002b0: 6729 0a21 5b76 6572 7369 6f6e 735d 2868  g).![versions](h
-000002c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-000002d0: 6473 2e69 6f2f 7079 7069 2f70 7976 6572  ds.io/pypi/pyver
-000002e0: 7369 6f6e 732f 7265 666c 6578 2e73 7667  sions/reflex.svg
-000002f0: 290a 5b21 5b44 6973 636f 7264 5d28 6874  ).[![Discord](ht
-00000300: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-00000310: 732e 696f 2f64 6973 636f 7264 2f31 3032  s.io/discord/102
-00000320: 3938 3533 3039 3535 3237 3732 3731 3635  9853095527727165
-00000330: 3f63 6f6c 6f72 3d25 3233 3732 3839 6461  ?color=%237289da
-00000340: 266c 6162 656c 3d44 6973 636f 7264 295d  &label=Discord)]
-00000350: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
-00000360: 2e67 672f 5435 5753 6243 3259 7451 290a  .gg/T5WSbC2YtQ).
-00000370: 0a3c 2f64 6976 3e0a 0a23 2323 2052 4541  .</div>..### REA
-00000380: 444d 4520 696e 2064 6966 6665 7265 6e74  DME in different
-00000390: 206c 616e 6775 6167 650a 0a2d 2d2d 0a0a   language..---..
-000003a0: 5b45 6e67 6c69 7368 5d28 6874 7470 733a  [English](https:
-000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f72 6566  //github.com/ref
-000003c0: 6c65 782d 6465 762f 7265 666c 6578 2f62  lex-dev/reflex/b
-000003d0: 6c6f 622f 6d61 696e 2f52 4541 444d 452e  lob/main/README.
-000003e0: 6d64 2920 7c20 5be7 ae80 e4bd 93e4 b8ad  md) | [.........
-000003f0: e696 875d 2868 7474 7073 3a2f 2f67 6974  ...](https://git
-00000400: 6875 622e 636f 6d2f 7265 666c 6578 2d64  hub.com/reflex-d
-00000410: 6576 2f72 6566 6c65 782f 626c 6f62 2f6d  ev/reflex/blob/m
-00000420: 6169 6e2f 646f 6373 2f7a 682f 7a68 5f63  ain/docs/zh/zh_c
-00000430: 6e2f 5245 4144 4d45 2e6d 6429 207c 205b  n/README.md) | [
-00000440: e7b9 81e9 ab94 e4b8 ade6 9687 5d28 6874  ............](ht
-00000450: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000460: 2f72 6566 6c65 782d 6465 762f 7265 666c  /reflex-dev/refl
-00000470: 6578 2f62 6c6f 622f 6d61 696e 2f64 6f63  ex/blob/main/doc
-00000480: 732f 7a68 2f7a 685f 7477 2f52 4541 444d  s/zh/zh_tw/READM
-00000490: 452e 6d64 290a 0a2d 2d2d 0a0a 2323 20f0  E.md)..---..## .
-000004a0: 9f93 a620 312e 2049 6e73 7461 6c6c 0a0a  ... 1. Install..
-000004b0: 5265 666c 6578 2072 6571 7569 7265 7320  Reflex requires 
-000004c0: 7468 6520 666f 6c6c 6f77 696e 6720 746f  the following to
-000004d0: 2067 6574 2073 7461 7274 6564 3a0a 0a2d   get started:..-
-000004e0: 2020 2050 7974 686f 6e20 332e 372b 0a2d     Python 3.7+.-
-000004f0: 2020 205b 4e6f 6465 2e6a 7320 3136 2e38     [Node.js 16.8
-00000500: 2e30 2b5d 2868 7474 7073 3a2f 2f6e 6f64  .0+](https://nod
-00000510: 656a 732e 6f72 672f 656e 2f29 2028 446f  ejs.org/en/) (Do
-00000520: 6e27 7420 776f 7272 792c 2079 6f75 2077  n't worry, you w
-00000530: 6f6e e280 9974 2068 6176 6520 746f 2077  on...t have to w
-00000540: 7269 7465 2061 6e79 204a 6176 6153 6372  rite any JavaScr
-00000550: 6970 7421 290a 0a60 6060 0a70 6970 2069  ipt!)..```.pip i
-00000560: 6e73 7461 6c6c 2072 6566 6c65 780a 6060  nstall reflex.``
-00000570: 600a 0a23 2320 f09f a5b3 2032 2e20 4372  `..## .... 2. Cr
-00000580: 6561 7465 2079 6f75 7220 6669 7273 7420  eate your first 
-00000590: 6170 700a 0a49 6e73 7461 6c6c 696e 6720  app..Installing 
-000005a0: 6072 6566 6c65 7860 2061 6c73 6f20 696e  `reflex` also in
-000005b0: 7374 616c 6c73 2074 6865 2060 7265 666c  stalls the `refl
-000005c0: 6578 6020 636f 6d6d 616e 6420 6c69 6e65  ex` command line
-000005d0: 2074 6f6f 6c2e 2054 6573 7420 7468 6174   tool. Test that
-000005e0: 2074 6865 2069 6e73 7461 6c6c 2077 6173   the install was
-000005f0: 2073 7563 6365 7373 6675 6c20 6279 2063   successful by c
-00000600: 7265 6174 696e 6720 6120 6e65 7720 7072  reating a new pr
-00000610: 6f6a 6563 742e 0a0a 5265 706c 6163 6520  oject...Replace 
-00000620: 6d79 5f61 7070 5f6e 616d 6520 7769 7468  my_app_name with
-00000630: 2079 6f75 7220 7072 6f6a 6563 7420 6e61   your project na
-00000640: 6d65 3a0a 0a60 6060 0a6d 6b64 6972 206d  me:..```.mkdir m
-00000650: 795f 6170 705f 6e61 6d65 0a63 6420 6d79  y_app_name.cd my
-00000660: 5f61 7070 5f6e 616d 650a 7265 666c 6578  _app_name.reflex
-00000670: 2069 6e69 740a 6060 600a 0a57 6865 6e20   init.```..When 
-00000680: 796f 7520 7275 6e20 7468 6973 2063 6f6d  you run this com
-00000690: 6d61 6e64 2066 6f72 2074 6865 2066 6972  mand for the fir
-000006a0: 7374 2074 696d 652c 2077 6520 7769 6c6c  st time, we will
-000006b0: 2064 6f77 6e6c 6f61 6420 616e 6420 696e   download and in
-000006c0: 7374 616c 6c20 5b62 756e 5d28 6874 7470  stall [bun](http
-000006d0: 733a 2f2f 6275 6e2e 7368 2f29 2061 7574  s://bun.sh/) aut
-000006e0: 6f6d 6174 6963 616c 6c79 2e0a 0a54 6869  omatically...Thi
-000006f0: 7320 636f 6d6d 616e 6420 696e 6974 6961  s command initia
-00000700: 6c69 7a65 7320 6120 7465 6d70 6c61 7465  lizes a template
-00000710: 2061 7070 2069 6e20 796f 7572 206e 6577   app in your new
-00000720: 2064 6972 6563 746f 7279 2e0a 0a23 2320   directory...## 
-00000730: f09f 8f83 2033 2e20 5275 6e20 796f 7572  .... 3. Run your
-00000740: 2061 7070 0a0a 596f 7520 6361 6e20 7275   app..You can ru
-00000750: 6e20 7468 6973 2061 7070 2069 6e20 6465  n this app in de
-00000760: 7665 6c6f 706d 656e 7420 6d6f 6465 3a0a  velopment mode:.
-00000770: 0a60 6060 0a72 6566 6c65 7820 7275 6e0a  .```.reflex run.
-00000780: 6060 600a 0a59 6f75 2073 686f 756c 6420  ```..You should 
-00000790: 7365 6520 796f 7572 2061 7070 2072 756e  see your app run
-000007a0: 6e69 6e67 2061 7420 6874 7470 3a2f 2f6c  ning at http://l
-000007b0: 6f63 616c 686f 7374 3a33 3030 302e 0a0a  ocalhost:3000...
-000007c0: 4e6f 7720 796f 7520 6361 6e20 6d6f 6469  Now you can modi
-000007d0: 6679 2074 6865 2073 6f75 7263 6520 636f  fy the source co
-000007e0: 6465 2069 6e20 606d 795f 6170 705f 6e61  de in `my_app_na
-000007f0: 6d65 2f6d 795f 6170 705f 6e61 6d65 2e70  me/my_app_name.p
-00000800: 7960 2e20 5265 666c 6578 2068 6173 2066  y`. Reflex has f
-00000810: 6173 7420 7265 6672 6573 6865 7320 736f  ast refreshes so
-00000820: 2079 6f75 2063 616e 2073 6565 2079 6f75   you can see you
-00000830: 7220 6368 616e 6765 7320 696e 7374 616e  r changes instan
-00000840: 746c 7920 7768 656e 2079 6f75 2073 6176  tly when you sav
-00000850: 6520 796f 7572 2063 6f64 652e 0a0a 2323  e your code...##
-00000860: 20f0 9fab a720 4578 616d 706c 650a 0a4c   .... Example..L
-00000870: 6574 2773 2067 6f20 6f76 6572 2061 6e20  et's go over an 
-00000880: 6578 616d 706c 653a 2063 7265 6174 696e  example: creatin
-00000890: 6720 616e 2069 6d61 6765 2067 656e 6572  g an image gener
-000008a0: 6174 696f 6e20 5549 2061 726f 756e 6420  ation UI around 
-000008b0: 4441 4c4c c2b7 452e 2046 6f72 2073 696d  DALL..E. For sim
-000008c0: 706c 6963 6974 792c 2077 6520 6a75 7374  plicity, we just
-000008d0: 2063 616c 6c20 7468 6520 4f70 656e 4149   call the OpenAI
-000008e0: 2041 5049 2c20 6275 7420 796f 7520 636f   API, but you co
-000008f0: 756c 6420 7265 706c 6163 6520 7468 6973  uld replace this
-00000900: 2077 6974 6820 616e 204d 4c20 6d6f 6465   with an ML mode
-00000910: 6c20 7275 6e20 6c6f 6361 6c6c 792e 0a0a  l run locally...
-00000920: 266e 6273 703b 0a0a 3c64 6976 2061 6c69  &nbsp;..<div ali
-00000930: 676e 3d22 6365 6e74 6572 223e 0a3c 696d  gn="center">.<im
-00000940: 6720 7372 633d 2264 6f63 732f 696d 6167  g src="docs/imag
-00000950: 6573 2f64 616c 6c65 2e67 6966 2220 616c  es/dalle.gif" al
-00000960: 743d 2241 2066 726f 6e74 656e 6420 7772  t="A frontend wr
-00000970: 6170 7065 7220 666f 7220 4441 4c4c c2b7  apper for DALL..
-00000980: 452c 2073 686f 776e 2069 6e20 7468 6520  E, shown in the 
-00000990: 7072 6f63 6573 7320 6f66 2067 656e 6572  process of gener
-000009a0: 6174 696e 6720 616e 2069 6d61 6765 2e22  ating an image."
-000009b0: 2077 6964 7468 3d22 3535 3022 202f 3e0a   width="550" />.
-000009c0: 3c2f 6469 763e 0a0a 266e 6273 703b 0a0a  </div>..&nbsp;..
-000009d0: 4865 7265 2069 7320 7468 6520 636f 6d70  Here is the comp
-000009e0: 6c65 7465 2063 6f64 6520 746f 2063 7265  lete code to cre
-000009f0: 6174 6520 7468 6973 2e20 5468 6973 2069  ate this. This i
-00000a00: 7320 616c 6c20 646f 6e65 2069 6e20 6f6e  s all done in on
-00000a10: 6520 5079 7468 6f6e 2066 696c 6521 0a0a  e Python file!..
-00000a20: 6060 6070 7974 686f 6e0a 696d 706f 7274  ```python.import
-00000a30: 2072 6566 6c65 7820 6173 2072 780a 696d   reflex as rx.im
-00000a40: 706f 7274 206f 7065 6e61 690a 0a6f 7065  port openai..ope
-00000a50: 6e61 692e 6170 695f 6b65 7920 3d20 2259  nai.api_key = "Y
-00000a60: 4f55 525f 4150 495f 4b45 5922 0a0a 636c  OUR_API_KEY"..cl
-00000a70: 6173 7320 5374 6174 6528 7278 2e53 7461  ass State(rx.Sta
-00000a80: 7465 293a 0a20 2020 2022 2222 5468 6520  te):.    """The 
-00000a90: 6170 7020 7374 6174 652e 2222 220a 2020  app state.""".  
-00000aa0: 2020 7072 6f6d 7074 203d 2022 220a 2020    prompt = "".  
-00000ab0: 2020 696d 6167 655f 7572 6c20 3d20 2222    image_url = ""
-00000ac0: 0a20 2020 2070 726f 6365 7373 696e 6720  .    processing 
-00000ad0: 3d20 4661 6c73 650a 2020 2020 636f 6d70  = False.    comp
-00000ae0: 6c65 7465 203d 2046 616c 7365 0a0a 2020  lete = False..  
-00000af0: 2020 6465 6620 6765 745f 696d 6167 6528    def get_image(
-00000b00: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00000b10: 2222 4765 7420 7468 6520 696d 6167 6520  ""Get the image 
-00000b20: 6672 6f6d 2074 6865 2070 726f 6d70 742e  from the prompt.
-00000b30: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
-00000b40: 656c 662e 7072 6f6d 7074 203d 3d20 2222  elf.prompt == ""
-00000b50: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00000b60: 7475 726e 2072 782e 7769 6e64 6f77 5f61  turn rx.window_a
-00000b70: 6c65 7274 2822 5072 6f6d 7074 2045 6d70  lert("Prompt Emp
-00000b80: 7479 2229 0a0a 2020 2020 2020 2020 7365  ty")..        se
-00000b90: 6c66 2e70 726f 6365 7373 696e 672c 2073  lf.processing, s
-00000ba0: 656c 662e 636f 6d70 6c65 7465 203d 2054  elf.complete = T
-00000bb0: 7275 652c 2046 616c 7365 0a20 2020 2020  rue, False.     
-00000bc0: 2020 2079 6965 6c64 0a20 2020 2020 2020     yield.       
-00000bd0: 2072 6573 706f 6e73 6520 3d20 6f70 656e   response = open
-00000be0: 6169 2e49 6d61 6765 2e63 7265 6174 6528  ai.Image.create(
-00000bf0: 7072 6f6d 7074 3d73 656c 662e 7072 6f6d  prompt=self.prom
-00000c00: 7074 2c20 6e3d 312c 2073 697a 653d 2231  pt, n=1, size="1
-00000c10: 3032 3478 3130 3234 2229 0a20 2020 2020  024x1024").     
-00000c20: 2020 2073 656c 662e 696d 6167 655f 7572     self.image_ur
-00000c30: 6c20 3d20 7265 7370 6f6e 7365 5b22 6461  l = response["da
-00000c40: 7461 225d 5b30 5d5b 2275 726c 225d 0a20  ta"][0]["url"]. 
-00000c50: 2020 2020 2020 2073 656c 662e 7072 6f63         self.proc
-00000c60: 6573 7369 6e67 2c20 7365 6c66 2e63 6f6d  essing, self.com
-00000c70: 706c 6574 6520 3d20 4661 6c73 652c 2054  plete = False, T
-00000c80: 7275 650a 2020 2020 2020 2020 0a0a 6465  rue.        ..de
-00000c90: 6620 696e 6465 7828 293a 0a20 2020 2072  f index():.    r
-00000ca0: 6574 7572 6e20 7278 2e63 656e 7465 7228  eturn rx.center(
-00000cb0: 0a20 2020 2020 2020 2072 782e 7673 7461  .        rx.vsta
-00000cc0: 636b 280a 2020 2020 2020 2020 2020 2020  ck(.            
-00000cd0: 7278 2e68 6561 6469 6e67 2822 4441 4c4c  rx.heading("DALL
-00000ce0: c2b7 4522 292c 0a20 2020 2020 2020 2020  ..E"),.         
-00000cf0: 2020 2072 782e 696e 7075 7428 706c 6163     rx.input(plac
-00000d00: 6568 6f6c 6465 723d 2245 6e74 6572 2061  eholder="Enter a
-00000d10: 2070 726f 6d70 7422 2c20 6f6e 5f62 6c75   prompt", on_blu
-00000d20: 723d 5374 6174 652e 7365 745f 7072 6f6d  r=State.set_prom
-00000d30: 7074 292c 0a20 2020 2020 2020 2020 2020  pt),.           
-00000d40: 2072 782e 6275 7474 6f6e 280a 2020 2020   rx.button(.    
-00000d50: 2020 2020 2020 2020 2020 2020 2247 656e              "Gen
-00000d60: 6572 6174 6520 496d 6167 6522 2c0a 2020  erate Image",.  
-00000d70: 2020 2020 2020 2020 2020 2020 2020 6f6e                on
-00000d80: 5f63 6c69 636b 3d53 7461 7465 2e67 6574  _click=State.get
-00000d90: 5f69 6d61 6765 2c0a 2020 2020 2020 2020  _image,.        
-00000da0: 2020 2020 2020 2020 6973 5f6c 6f61 6469          is_loadi
-00000db0: 6e67 3d53 7461 7465 2e70 726f 6365 7373  ng=State.process
-00000dc0: 696e 672c 0a20 2020 2020 2020 2020 2020  ing,.           
-00000dd0: 2020 2020 2077 6964 7468 3d22 3130 3025       width="100%
-00000de0: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
-00000df0: 2c0a 2020 2020 2020 2020 2020 2020 7278  ,.            rx
-00000e00: 2e63 6f6e 6428 0a20 2020 2020 2020 2020  .cond(.         
-00000e10: 2020 2020 2020 2053 7461 7465 2e63 6f6d         State.com
-00000e20: 706c 6574 652c 0a20 2020 2020 2020 2020  plete,.         
-00000e30: 2020 2020 2020 2020 2020 2020 7278 2e69              rx.i
-00000e40: 6d61 6765 280a 2020 2020 2020 2020 2020  mage(.          
-00000e50: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00000e60: 7263 3d53 7461 7465 2e69 6d61 6765 5f75  rc=State.image_u
-00000e70: 726c 2c0a 2020 2020 2020 2020 2020 2020  rl,.            
-00000e80: 2020 2020 2020 2020 2020 2020 2068 6569               hei
-00000e90: 6768 743d 2232 3565 6d22 2c0a 2020 2020  ght="25em",.    
-00000ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000eb0: 2020 2020 2077 6964 7468 3d22 3235 656d       width="25em
-00000ec0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00000ed0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00000ee0: 2020 2020 2029 2c0a 2020 2020 2020 2020       ),.        
-00000ef0: 2020 2020 7061 6464 696e 673d 2232 656d      padding="2em
-00000f00: 222c 0a20 2020 2020 2020 2020 2020 2073  ",.            s
-00000f10: 6861 646f 773d 226c 6722 2c0a 2020 2020  hadow="lg",.    
-00000f20: 2020 2020 2020 2020 626f 7264 6572 5f72          border_r
-00000f30: 6164 6975 733d 226c 6722 2c0a 2020 2020  adius="lg",.    
-00000f40: 2020 2020 292c 0a20 2020 2020 2020 2077      ),.        w
-00000f50: 6964 7468 3d22 3130 3025 222c 0a20 2020  idth="100%",.   
-00000f60: 2020 2020 2068 6569 6768 743d 2231 3030       height="100
-00000f70: 7668 222c 0a20 2020 2029 0a0a 2320 4164  vh",.    )..# Ad
-00000f80: 6420 7374 6174 6520 616e 6420 7061 6765  d state and page
-00000f90: 2074 6f20 7468 6520 6170 702e 0a61 7070   to the app..app
-00000fa0: 203d 2072 782e 4170 7028 7374 6174 653d   = rx.App(state=
-00000fb0: 5374 6174 6529 0a61 7070 2e61 6464 5f70  State).app.add_p
-00000fc0: 6167 6528 696e 6465 782c 2074 6974 6c65  age(index, title
-00000fd0: 3d22 7265 666c 6578 3a44 414c 4cc2 b745  ="reflex:DALL..E
-00000fe0: 2229 0a61 7070 2e63 6f6d 7069 6c65 2829  ").app.compile()
-00000ff0: 0a60 6060 0a0a 4c65 7427 7320 6272 6561  .```..Let's brea
-00001000: 6b20 7468 6973 2064 6f77 6e2e 0a0a 2323  k this down...##
-00001010: 2320 2a2a 5549 2049 6e20 5265 666c 6578  # **UI In Reflex
-00001020: 2a2a 0a0a 4c65 7427 7320 7374 6172 7420  **..Let's start 
-00001030: 7769 7468 2074 6865 2055 492e 0a0a 6060  with the UI...``
-00001040: 6070 7974 686f 6e0a 6465 6620 696e 6465  `python.def inde
-00001050: 7828 293a 0a20 2020 2072 6574 7572 6e20  x():.    return 
-00001060: 7278 2e63 656e 7465 7228 0a20 2020 2020  rx.center(.     
-00001070: 2020 202e 2e2e 0a20 2020 2029 0a60 6060     ....    ).```
-00001080: 0a0a 5468 6973 2060 696e 6465 7860 2066  ..This `index` f
-00001090: 756e 6374 696f 6e20 6465 6669 6e65 7320  unction defines 
-000010a0: 7468 6520 6672 6f6e 7465 6e64 206f 6620  the frontend of 
-000010b0: 7468 6520 6170 702e 0a0a 5765 2075 7365  the app...We use
-000010c0: 2064 6966 6665 7265 6e74 2063 6f6d 706f   different compo
-000010d0: 6e65 6e74 7320 7375 6368 2061 7320 6063  nents such as `c
-000010e0: 656e 7465 7260 2c20 6076 7374 6163 6b60  enter`, `vstack`
-000010f0: 2c20 6069 6e70 7574 602c 2061 6e64 2060  , `input`, and `
-00001100: 6275 7474 6f6e 6020 746f 2062 7569 6c64  button` to build
-00001110: 2074 6865 2066 726f 6e74 656e 642e 2043   the frontend. C
-00001120: 6f6d 706f 6e65 6e74 7320 6361 6e20 6265  omponents can be
-00001130: 206e 6573 7465 6420 7769 7468 696e 2065   nested within e
-00001140: 6163 6820 6f74 6865 720a 746f 2063 7265  ach other.to cre
-00001150: 6174 6520 636f 6d70 6c65 7820 6c61 796f  ate complex layo
-00001160: 7574 732e 2041 6e64 2079 6f75 2063 616e  uts. And you can
-00001170: 2075 7365 206b 6579 776f 7264 2061 7267   use keyword arg
-00001180: 7320 746f 2073 7479 6c65 2074 6865 6d20  s to style them 
-00001190: 7769 7468 2074 6865 2066 756c 6c20 706f  with the full po
-000011a0: 7765 7220 6f66 2043 5353 2e0a 0a52 6566  wer of CSS...Ref
-000011b0: 6c65 7820 636f 6d65 7320 7769 7468 205b  lex comes with [
-000011c0: 3630 2b20 6275 696c 742d 696e 2063 6f6d  60+ built-in com
-000011d0: 706f 6e65 6e74 735d 2868 7474 7073 3a2f  ponents](https:/
-000011e0: 2f72 6566 6c65 782e 6465 762f 646f 6373  /reflex.dev/docs
-000011f0: 2f6c 6962 7261 7279 2920 746f 2068 656c  /library) to hel
-00001200: 7020 796f 7520 6765 7420 7374 6172 7465  p you get starte
-00001210: 642e 2057 6520 6172 6520 6163 7469 7665  d. We are active
-00001220: 6c79 2061 6464 696e 6720 6d6f 7265 2063  ly adding more c
-00001230: 6f6d 706f 6e65 6e74 732c 2061 6e64 2069  omponents, and i
-00001240: 7427 7320 6561 7379 2074 6f20 5b63 7265  t's easy to [cre
-00001250: 6174 6520 796f 7572 206f 776e 2063 6f6d  ate your own com
-00001260: 706f 6e65 6e74 735d 2868 7474 7073 3a2f  ponents](https:/
-00001270: 2f72 6566 6c65 782e 6465 762f 646f 6373  /reflex.dev/docs
-00001280: 2f61 6476 616e 6365 642d 6775 6964 652f  /advanced-guide/
-00001290: 7772 6170 7069 6e67 2d72 6561 6374 292e  wrapping-react).
-000012a0: 0a0a 2323 2320 2a2a 5374 6174 652a 2a0a  ..### **State**.
-000012b0: 0a52 6566 6c65 7820 7265 7072 6573 656e  .Reflex represen
-000012c0: 7473 2079 6f75 7220 5549 2061 7320 6120  ts your UI as a 
-000012d0: 6675 6e63 7469 6f6e 206f 6620 796f 7572  function of your
-000012e0: 2073 7461 7465 2e0a 0a60 6060 7079 7468   state...```pyth
-000012f0: 6f6e 0a63 6c61 7373 2053 7461 7465 2872  on.class State(r
-00001300: 782e 5374 6174 6529 3a0a 2020 2020 2222  x.State):.    ""
-00001310: 2254 6865 2061 7070 2073 7461 7465 2e22  "The app state."
-00001320: 2222 0a20 2020 2070 726f 6d70 7420 3d20  "".    prompt = 
-00001330: 2222 0a20 2020 2069 6d61 6765 5f75 726c  "".    image_url
-00001340: 203d 2022 220a 2020 2020 7072 6f63 6573   = "".    proces
-00001350: 7369 6e67 203d 2046 616c 7365 0a20 2020  sing = False.   
-00001360: 2063 6f6d 706c 6574 6520 3d20 4661 6c73   complete = Fals
-00001370: 650a 6060 600a 0a54 6865 2073 7461 7465  e.```..The state
-00001380: 2064 6566 696e 6573 2061 6c6c 2074 6865   defines all the
-00001390: 2076 6172 6961 626c 6573 2028 6361 6c6c   variables (call
-000013a0: 6564 2076 6172 7329 2069 6e20 616e 2061  ed vars) in an a
-000013b0: 7070 2074 6861 7420 6361 6e20 6368 616e  pp that can chan
-000013c0: 6765 2061 6e64 2074 6865 2066 756e 6374  ge and the funct
-000013d0: 696f 6e73 2074 6861 7420 6368 616e 6765  ions that change
-000013e0: 2074 6865 6d2e 0a0a 4865 7265 2074 6865   them...Here the
-000013f0: 2073 7461 7465 2069 7320 636f 6d70 7269   state is compri
-00001400: 7365 6420 6f66 2061 2060 7072 6f6d 7074  sed of a `prompt
-00001410: 6020 616e 6420 6069 6d61 6765 5f75 726c  ` and `image_url
-00001420: 602e 2054 6865 7265 2061 7265 2061 6c73  `. There are als
-00001430: 6f20 7468 6520 626f 6f6c 6561 6e73 2060  o the booleans `
-00001440: 7072 6f63 6573 7369 6e67 6020 616e 6420  processing` and 
-00001450: 6063 6f6d 706c 6574 6560 2074 6f20 696e  `complete` to in
-00001460: 6469 6361 7465 2077 6865 6e20 746f 2073  dicate when to s
-00001470: 686f 7720 7468 6520 6369 7263 756c 6172  how the circular
-00001480: 2070 726f 6772 6573 7320 616e 6420 696d   progress and im
-00001490: 6167 652e 0a0a 2323 2320 2a2a 4576 656e  age...### **Even
-000014a0: 7420 4861 6e64 6c65 7273 2a2a 0a0a 6060  t Handlers**..``
-000014b0: 6070 7974 686f 6e0a 6465 6620 6765 745f  `python.def get_
-000014c0: 696d 6167 6528 7365 6c66 293a 0a20 2020  image(self):.   
-000014d0: 2022 2222 4765 7420 7468 6520 696d 6167   """Get the imag
-000014e0: 6520 6672 6f6d 2074 6865 2070 726f 6d70  e from the promp
-000014f0: 742e 2222 220a 2020 2020 6966 2073 656c  t.""".    if sel
-00001500: 662e 7072 6f6d 7074 203d 3d20 2222 3a0a  f.prompt == "":.
-00001510: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00001520: 782e 7769 6e64 6f77 5f61 6c65 7274 2822  x.window_alert("
-00001530: 5072 6f6d 7074 2045 6d70 7479 2229 0a0a  Prompt Empty")..
-00001540: 2020 2020 7365 6c66 2e70 726f 6365 7373      self.process
-00001550: 696e 672c 2073 656c 662e 636f 6d70 6c65  ing, self.comple
-00001560: 7465 203d 2054 7275 652c 2046 616c 7365  te = True, False
-00001570: 0a20 2020 2079 6965 6c64 0a20 2020 2072  .    yield.    r
-00001580: 6573 706f 6e73 6520 3d20 6f70 656e 6169  esponse = openai
-00001590: 2e49 6d61 6765 2e63 7265 6174 6528 7072  .Image.create(pr
-000015a0: 6f6d 7074 3d73 656c 662e 7072 6f6d 7074  ompt=self.prompt
-000015b0: 2c20 6e3d 312c 2073 697a 653d 2231 3032  , n=1, size="102
-000015c0: 3478 3130 3234 2229 0a20 2020 2073 656c  4x1024").    sel
-000015d0: 662e 696d 6167 655f 7572 6c20 3d20 7265  f.image_url = re
-000015e0: 7370 6f6e 7365 5b22 6461 7461 225d 5b30  sponse["data"][0
-000015f0: 5d5b 2275 726c 225d 0a20 2020 2073 656c  ]["url"].    sel
-00001600: 662e 7072 6f63 6573 7369 6e67 2c20 7365  f.processing, se
-00001610: 6c66 2e63 6f6d 706c 6574 6520 3d20 4661  lf.complete = Fa
-00001620: 6c73 652c 2054 7275 650a 6060 600a 0a57  lse, True.```..W
-00001630: 6974 6869 6e20 7468 6520 7374 6174 652c  ithin the state,
-00001640: 2077 6520 6465 6669 6e65 2066 756e 6374   we define funct
-00001650: 696f 6e73 2063 616c 6c65 6420 6576 656e  ions called even
-00001660: 7420 6861 6e64 6c65 7273 2074 6861 7420  t handlers that 
-00001670: 6368 616e 6765 2074 6865 2073 7461 7465  change the state
-00001680: 2076 6172 732e 2045 7665 6e74 2068 616e   vars. Event han
-00001690: 646c 6572 7320 6172 6520 7468 6520 7761  dlers are the wa
-000016a0: 7920 7468 6174 2077 6520 6361 6e20 6d6f  y that we can mo
-000016b0: 6469 6679 2074 6865 2073 7461 7465 2069  dify the state i
-000016c0: 6e20 5265 666c 6578 2e20 5468 6579 2063  n Reflex. They c
-000016d0: 616e 2062 6520 6361 6c6c 6564 2069 6e20  an be called in 
-000016e0: 7265 7370 6f6e 7365 2074 6f20 7573 6572  response to user
-000016f0: 2061 6374 696f 6e73 2c20 7375 6368 2061   actions, such a
-00001700: 7320 636c 6963 6b69 6e67 2061 2062 7574  s clicking a but
-00001710: 746f 6e20 6f72 2074 7970 696e 6720 696e  ton or typing in
-00001720: 2061 2074 6578 7420 626f 782e 2054 6865   a text box. The
-00001730: 7365 2061 6374 696f 6e73 2061 7265 2063  se actions are c
-00001740: 616c 6c65 6420 6576 656e 7473 2e0a 0a4f  alled events...O
-00001750: 7572 2044 414c 4cc2 b745 2e20 6170 7020  ur DALL..E. app 
-00001760: 6861 7320 616e 2065 7665 6e74 2068 616e  has an event han
-00001770: 646c 6572 2c20 6067 6574 5f69 6d61 6765  dler, `get_image
-00001780: 6020 746f 2077 6869 6368 2067 6574 2074  ` to which get t
-00001790: 6869 7320 696d 6167 6520 6672 6f6d 2074  his image from t
-000017a0: 6865 204f 7065 6e41 4920 4150 492e 2055  he OpenAI API. U
-000017b0: 7369 6e67 2060 7969 656c 6460 2069 6e20  sing `yield` in 
-000017c0: 7468 6520 6d69 6464 6c65 206f 6620 616e  the middle of an
-000017d0: 2065 7665 6e74 2068 616e 646c 6572 2077   event handler w
-000017e0: 696c 6c20 6361 7573 6520 7468 6520 5549  ill cause the UI
-000017f0: 2074 6f20 7570 6461 7465 2e20 4f74 6865   to update. Othe
-00001800: 7277 6973 6520 7468 6520 5549 2077 696c  rwise the UI wil
-00001810: 6c20 7570 6461 7465 2061 7420 7468 6520  l update at the 
-00001820: 656e 6420 6f66 2074 6865 2065 7665 6e74  end of the event
-00001830: 2068 616e 646c 6572 2e0a 0a23 2323 202a   handler...### *
-00001840: 2a52 6f75 7469 6e67 2a2a 0a0a 4669 6e61  *Routing**..Fina
-00001850: 6c6c 792c 2077 6520 6465 6669 6e65 206f  lly, we define o
-00001860: 7572 2061 7070 2061 6e64 2070 6173 7320  ur app and pass 
-00001870: 6974 206f 7572 2073 7461 7465 2e0a 0a60  it our state...`
-00001880: 6060 7079 7468 6f6e 0a61 7070 203d 2072  ``python.app = r
-00001890: 782e 4170 7028 7374 6174 653d 5374 6174  x.App(state=Stat
-000018a0: 6529 0a60 6060 0a0a 5765 2061 6464 2061  e).```..We add a
-000018b0: 2072 6f75 7465 2066 726f 6d20 7468 6520   route from the 
-000018c0: 726f 6f74 206f 6620 7468 6520 6170 7020  root of the app 
-000018d0: 746f 2074 6865 2069 6e64 6578 2063 6f6d  to the index com
-000018e0: 706f 6e65 6e74 2e20 5765 2061 6c73 6f20  ponent. We also 
-000018f0: 6164 6420 6120 7469 746c 6520 7468 6174  add a title that
-00001900: 2077 696c 6c20 7368 6f77 2075 7020 696e   will show up in
-00001910: 2074 6865 2070 6167 6520 7072 6576 6965   the page previe
-00001920: 772f 6272 6f77 7365 7220 7461 622e 0a0a  w/browser tab...
-00001930: 6060 6070 7974 686f 6e0a 6170 702e 6164  ```python.app.ad
-00001940: 645f 7061 6765 2869 6e64 6578 2c20 7469  d_page(index, ti
-00001950: 746c 653d 2244 414c 4c2d 4522 290a 6170  tle="DALL-E").ap
-00001960: 702e 636f 6d70 696c 6528 290a 6060 600a  p.compile().```.
-00001970: 0a59 6f75 2063 616e 2063 7265 6174 6520  .You can create 
-00001980: 6120 6d75 6c74 692d 7061 6765 2061 7070  a multi-page app
-00001990: 2062 7920 6164 6469 6e67 206d 6f72 6520   by adding more 
-000019a0: 726f 7574 6573 2e0a 0a23 2320 5374 6174  routes...## Stat
-000019b0: 7573 0a0a 5265 666c 6578 206c 6175 6e63  us..Reflex launc
-000019c0: 6865 6420 696e 2044 6563 656d 6265 7220  hed in December 
-000019d0: 3230 3232 2077 6974 6820 7468 6520 6e61  2022 with the na
-000019e0: 6d65 2050 796e 6563 6f6e 652e 0a0a 4173  me Pynecone...As
-000019f0: 206f 6620 4a75 6e65 2032 3032 332c 2077   of June 2023, w
-00001a00: 6520 6172 6520 696e 2074 6865 202a 2a50  e are in the **P
-00001a10: 7562 6c69 6320 4265 7461 2a2a 2073 7461  ublic Beta** sta
-00001a20: 6765 2e0a 0a2d 2020 203a 7768 6974 655f  ge...-   :white_
-00001a30: 6368 6563 6b5f 6d61 726b 3a20 2a2a 5075  check_mark: **Pu
-00001a40: 626c 6963 2041 6c70 6861 2a2a 3a20 416e  blic Alpha**: An
-00001a50: 796f 6e65 2063 616e 2069 6e73 7461 6c6c  yone can install
-00001a60: 2061 6e64 2075 7365 2052 6566 6c65 782e   and use Reflex.
-00001a70: 2054 6865 7265 206d 6179 2062 6520 6973   There may be is
-00001a80: 7375 6573 2c20 6275 7420 7765 2061 7265  sues, but we are
-00001a90: 2077 6f72 6b69 6e67 2074 6f20 7265 736f   working to reso
-00001aa0: 6c76 6520 7468 656d 2061 6374 6976 656c  lve them activel
-00001ab0: 792e 0a2d 2020 203a 6c61 7267 655f 6f72  y..-   :large_or
-00001ac0: 616e 6765 5f64 6961 6d6f 6e64 3a20 2a2a  ange_diamond: **
-00001ad0: 5075 626c 6963 2042 6574 612a 2a3a 2053  Public Beta**: S
-00001ae0: 7461 626c 6520 656e 6f75 6768 2066 6f72  table enough for
-00001af0: 206e 6f6e 2d65 6e74 6572 7072 6973 6520   non-enterprise 
-00001b00: 7573 652d 6361 7365 732e 0a2d 2020 202a  use-cases..-   *
-00001b10: 2a50 7562 6c69 6320 486f 7374 696e 6720  *Public Hosting 
-00001b20: 4265 7461 2a2a 3a20 5f4f 7074 696f 6e61  Beta**: _Optiona
-00001b30: 6c6c 795f 2c20 6465 706c 6f79 2061 6e64  lly_, deploy and
-00001b40: 2068 6f73 7420 796f 7572 2061 7070 7320   host your apps 
-00001b50: 6f6e 2052 6566 6c65 7821 0a2d 2020 202a  on Reflex!.-   *
-00001b60: 2a50 7562 6c69 632a 2a3a 2052 6566 6c65  *Public**: Refle
-00001b70: 7820 6973 2070 726f 6475 6374 696f 6e20  x is production 
-00001b80: 7265 6164 792e 0a0a 5265 666c 6578 2068  ready...Reflex h
-00001b90: 6173 206e 6577 2072 656c 6561 7365 7320  as new releases 
-00001ba0: 616e 6420 6665 6174 7572 6573 2063 6f6d  and features com
-00001bb0: 696e 6720 6576 6572 7920 7765 656b 2120  ing every week! 
-00001bc0: 4d61 6b65 2073 7572 6520 746f 203a 7374  Make sure to :st
-00001bd0: 6172 3a20 7374 6172 2061 6e64 203a 6579  ar: star and :ey
-00001be0: 6573 3a20 7761 7463 6820 7468 6973 2072  es: watch this r
-00001bf0: 6570 6f73 6974 6f72 7920 746f 2073 7461  epository to sta
-00001c00: 7920 7570 2074 6f20 6461 7465 2e0a 0a23  y up to date...#
-00001c10: 2320 436f 6e74 7269 6275 7469 6e67 0a0a  # Contributing..
-00001c20: 5765 2077 656c 636f 6d65 2063 6f6e 7472  We welcome contr
-00001c30: 6962 7574 696f 6e73 206f 6620 616e 7920  ibutions of any 
-00001c40: 7369 7a65 2120 4265 6c6f 7720 6172 6520  size! Below are 
-00001c50: 736f 6d65 2067 6f6f 6420 7761 7973 2074  some good ways t
-00001c60: 6f20 6765 7420 7374 6172 7465 6420 696e  o get started in
-00001c70: 2074 6865 2052 6566 6c65 7820 636f 6d6d   the Reflex comm
-00001c80: 756e 6974 792e 0a0a 2d20 2020 2a2a 4a6f  unity...-   **Jo
-00001c90: 696e 204f 7572 2044 6973 636f 7264 2a2a  in Our Discord**
-00001ca0: 3a20 4f75 7220 5b44 6973 636f 7264 5d28  : Our [Discord](
-00001cb0: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
-00001cc0: 6767 2f54 3557 5362 4332 5974 5129 2069  gg/T5WSbC2YtQ) i
-00001cd0: 7320 7468 6520 6265 7374 2070 6c61 6365  s the best place
-00001ce0: 2074 6f20 6765 7420 6865 6c70 206f 6e20   to get help on 
-00001cf0: 796f 7572 2052 6566 6c65 7820 7072 6f6a  your Reflex proj
-00001d00: 6563 7420 616e 6420 746f 2064 6973 6375  ect and to discu
-00001d10: 7373 2068 6f77 2079 6f75 2063 616e 2063  ss how you can c
-00001d20: 6f6e 7472 6962 7574 652e 0a2d 2020 202a  ontribute..-   *
-00001d30: 2a47 6974 4875 6220 4469 7363 7573 7369  *GitHub Discussi
-00001d40: 6f6e 732a 2a3a 2041 2067 7265 6174 2077  ons**: A great w
-00001d50: 6179 2074 6f20 7461 6c6b 2061 626f 7574  ay to talk about
-00001d60: 2066 6561 7475 7265 7320 796f 7520 7761   features you wa
-00001d70: 6e74 2061 6464 6564 206f 7220 7468 696e  nt added or thin
-00001d80: 6773 2074 6861 7420 6172 6520 636f 6e66  gs that are conf
-00001d90: 7573 696e 672f 6e65 6564 2063 6c61 7269  using/need clari
-00001da0: 6669 6361 7469 6f6e 2e0a 2d20 2020 2a2a  fication..-   **
-00001db0: 4769 7448 7562 2049 7373 7565 732a 2a3a  GitHub Issues**:
-00001dc0: 2054 6865 7365 2061 7265 2061 6e20 6578   These are an ex
-00001dd0: 6365 6c6c 656e 7420 7761 7920 746f 2072  cellent way to r
-00001de0: 6570 6f72 7420 6275 6773 2e20 4164 6469  eport bugs. Addi
-00001df0: 7469 6f6e 616c 6c79 2c20 796f 7520 6361  tionally, you ca
-00001e00: 6e20 7472 7920 616e 6420 736f 6c76 6520  n try and solve 
-00001e10: 616e 2065 7869 7374 696e 6720 6973 7375  an existing issu
-00001e20: 6520 616e 6420 7375 626d 6974 2061 2050  e and submit a P
-00001e30: 522e 0a0a 5765 2061 7265 2061 6374 6976  R...We are activ
-00001e40: 656c 7920 6c6f 6f6b 696e 6720 666f 7220  ely looking for 
-00001e50: 636f 6e74 7269 6275 746f 7273 2c20 6e6f  contributors, no
-00001e60: 206d 6174 7465 7220 796f 7572 2073 6b69   matter your ski
-00001e70: 6c6c 206c 6576 656c 206f 7220 6578 7065  ll level or expe
-00001e80: 7269 656e 6365 2e0a 0a23 2320 4c69 6365  rience...## Lice
-00001e90: 6e73 650a 0a52 6566 6c65 7820 6973 206f  nse..Reflex is o
-00001ea0: 7065 6e2d 736f 7572 6365 2061 6e64 206c  pen-source and l
-00001eb0: 6963 656e 7365 6420 756e 6465 7220 7468  icensed under th
-00001ec0: 6520 5b41 7061 6368 6520 4c69 6365 6e73  e [Apache Licens
-00001ed0: 6520 322e 305d 284c 4943 454e 5345 292e  e 2.0](LICENSE).
-00001ee0: 0a                                       .
+00000070: 6967 6e3d 2263 656e 7465 7222 3e0a 3c69  ign="center">.<i
+00000080: 6d67 2073 7263 3d22 646f 6373 2f69 6d61  mg src="docs/ima
+00000090: 6765 732f 7265 666c 6578 5f64 6172 6b2e  ges/reflex_dark.
+000000a0: 7376 6723 6768 2d6c 6967 6874 2d6d 6f64  svg#gh-light-mod
+000000b0: 652d 6f6e 6c79 2220 616c 743d 2252 6566  e-only" alt="Ref
+000000c0: 6c65 7820 4c6f 676f 2220 7769 6474 683d  lex Logo" width=
+000000d0: 2233 3030 7078 223e 0a3c 696d 6720 7372  "300px">.<img sr
+000000e0: 633d 2264 6f63 732f 696d 6167 6573 2f72  c="docs/images/r
+000000f0: 6566 6c65 785f 6c69 6768 742e 7376 6723  eflex_light.svg#
+00000100: 6768 2d64 6172 6b2d 6d6f 6465 2d6f 6e6c  gh-dark-mode-onl
+00000110: 7922 2061 6c74 3d22 5265 666c 6578 204c  y" alt="Reflex L
+00000120: 6f67 6f22 2077 6964 7468 3d22 3330 3070  ogo" width="300p
+00000130: 7822 3e0a 0a3c 6872 3e0a 0a23 2323 202a  x">..<hr>..### *
+00000140: 2ae2 9ca8 2050 6572 666f 726d 616e 742c  *... Performant,
+00000150: 2063 7573 746f 6d69 7a61 626c 6520 7765   customizable we
+00000160: 6220 6170 7073 2069 6e20 7075 7265 2050  b apps in pure P
+00000170: 7974 686f 6e2e 2044 6570 6c6f 7920 696e  ython. Deploy in
+00000180: 2073 6563 6f6e 6473 2e20 e29c a82a 2a0a   seconds. ...**.
+00000190: 5b21 5b50 7950 4920 7665 7273 696f 6e5d  [![PyPI version]
+000001a0: 2868 7474 7073 3a2f 2f62 6164 6765 2e66  (https://badge.f
+000001b0: 7572 792e 696f 2f70 792f 7265 666c 6578  ury.io/py/reflex
+000001c0: 2e73 7667 295d 2868 7474 7073 3a2f 2f62  .svg)](https://b
+000001d0: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
+000001e0: 7265 666c 6578 290a 215b 7465 7374 735d  reflex).![tests]
+000001f0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000200: 636f 6d2f 7079 6e65 636f 6e65 2d69 6f2f  com/pynecone-io/
+00000210: 7079 6e65 636f 6e65 2f61 6374 696f 6e73  pynecone/actions
+00000220: 2f77 6f72 6b66 6c6f 7773 2f69 6e74 6567  /workflows/integ
+00000230: 7261 7469 6f6e 2e79 6d6c 2f62 6164 6765  ration.yml/badge
+00000240: 2e73 7667 290a 215b 7665 7273 696f 6e73  .svg).![versions
+00000250: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000260: 6965 6c64 732e 696f 2f70 7970 692f 7079  ields.io/pypi/py
+00000270: 7665 7273 696f 6e73 2f72 6566 6c65 782e  versions/reflex.
+00000280: 7376 6729 0a5b 215b 446f 6375 6d65 6e74  svg).[![Document
+00000290: 6169 746f 6e5d 2868 7474 7073 3a2f 2f69  aiton](https://i
+000002a0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002b0: 6467 652f 446f 6375 6d65 6e74 6174 696f  dge/Documentatio
+000002c0: 6e25 3230 2d49 6e74 726f 6475 6374 696f  n%20-Introductio
+000002d0: 6e25 3230 2d25 3230 2532 3330 3037 6563  n%20-%20%23007ec
+000002e0: 3629 5d28 6874 7470 733a 2f2f 7265 666c  6)](https://refl
+000002f0: 6578 2e64 6576 2f64 6f63 732f 6765 7474  ex.dev/docs/gett
+00000300: 696e 672d 7374 6172 7465 642f 696e 7472  ing-started/intr
+00000310: 6f64 7563 7469 6f6e 290a 5b21 5b44 6973  oduction).[![Dis
+00000320: 636f 7264 5d28 6874 7470 733a 2f2f 696d  cord](https://im
+00000330: 672e 7368 6965 6c64 732e 696f 2f64 6973  g.shields.io/dis
+00000340: 636f 7264 2f31 3032 3938 3533 3039 3535  cord/10298530955
+00000350: 3237 3732 3731 3635 3f63 6f6c 6f72 3d25  27727165?color=%
+00000360: 3233 3732 3839 6461 266c 6162 656c 3d44  237289da&label=D
+00000370: 6973 636f 7264 295d 2868 7474 7073 3a2f  iscord)](https:/
+00000380: 2f64 6973 636f 7264 2e67 672f 5435 5753  /discord.gg/T5WS
+00000390: 6243 3259 7451 290a 3c2f 6469 763e 0a0a  bC2YtQ).</div>..
+000003a0: 2d2d 2d0a 5b45 6e67 6c69 7368 5d28 6874  ---.[English](ht
+000003b0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000003c0: 2f72 6566 6c65 782d 6465 762f 7265 666c  /reflex-dev/refl
+000003d0: 6578 2f62 6c6f 622f 6d61 696e 2f52 4541  ex/blob/main/REA
+000003e0: 444d 452e 6d64 2920 7c20 5be7 ae80 e4bd  DME.md) | [.....
+000003f0: 93e4 b8ad e696 875d 2868 7474 7073 3a2f  .......](https:/
+00000400: 2f67 6974 6875 622e 636f 6d2f 7265 666c  /github.com/refl
+00000410: 6578 2d64 6576 2f72 6566 6c65 782f 626c  ex-dev/reflex/bl
+00000420: 6f62 2f6d 6169 6e2f 646f 6373 2f7a 682f  ob/main/docs/zh/
+00000430: 7a68 5f63 6e2f 5245 4144 4d45 2e6d 6429  zh_cn/README.md)
+00000440: 207c 205b e7b9 81e9 ab94 e4b8 ade6 9687   | [............
+00000450: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000460: 2e63 6f6d 2f72 6566 6c65 782d 6465 762f  .com/reflex-dev/
+00000470: 7265 666c 6578 2f62 6c6f 622f 6d61 696e  reflex/blob/main
+00000480: 2f64 6f63 732f 7a68 2f7a 685f 7477 2f52  /docs/zh/zh_tw/R
+00000490: 4541 444d 452e 6d64 290a 2d2d 2d0a 2323  EADME.md).---.##
+000004a0: 20e2 9a99 efb8 8f20 496e 7374 616c 6c61   ...... Installa
+000004b0: 7469 6f6e 0a0a 4f70 656e 2061 2074 6572  tion..Open a ter
+000004c0: 6d69 6e61 6c20 616e 6420 7275 6e20 2852  minal and run (R
+000004d0: 6571 7569 7265 7320 5079 7468 6f6e 2033  equires Python 3
+000004e0: 2e37 2b29 3a0a 0a60 6060 6261 7368 0a70  .7+):..```bash.p
+000004f0: 6970 2069 6e73 7461 6c6c 2072 6566 6c65  ip install refle
+00000500: 780a 6060 600a 0a23 2320 f09f a5b3 2043  x.```..## .... C
+00000510: 7265 6174 6520 796f 7572 2066 6972 7374  reate your first
+00000520: 2061 7070 0a0a 496e 7374 616c 6c69 6e67   app..Installing
+00000530: 2060 7265 666c 6578 6020 616c 736f 2069   `reflex` also i
+00000540: 6e73 7461 6c6c 7320 7468 6520 6072 6566  nstalls the `ref
+00000550: 6c65 7860 2063 6f6d 6d61 6e64 206c 696e  lex` command lin
+00000560: 6520 746f 6f6c 2e0a 0a54 6573 7420 7468  e tool...Test th
+00000570: 6174 2074 6865 2069 6e73 7461 6c6c 2077  at the install w
+00000580: 6173 2073 7563 6365 7373 6675 6c20 6279  as successful by
+00000590: 2063 7265 6174 696e 6720 6120 6e65 7720   creating a new 
+000005a0: 7072 6f6a 6563 742e 2028 5265 706c 6163  project. (Replac
+000005b0: 6520 606d 795f 6170 705f 6e61 6d65 6020  e `my_app_name` 
+000005c0: 7769 7468 2079 6f75 7220 7072 6f6a 6563  with your projec
+000005d0: 7420 6e61 6d65 293a 0a0a 6060 6062 6173  t name):..```bas
+000005e0: 680a 6d6b 6469 7220 6d79 5f61 7070 5f6e  h.mkdir my_app_n
+000005f0: 616d 650a 6364 206d 795f 6170 705f 6e61  ame.cd my_app_na
+00000600: 6d65 0a72 6566 6c65 7820 696e 6974 0a60  me.reflex init.`
+00000610: 6060 0a0a 5468 6973 2063 6f6d 6d61 6e64  ``..This command
+00000620: 2069 6e69 7469 616c 697a 6573 2061 2074   initializes a t
+00000630: 656d 706c 6174 6520 6170 7020 696e 2079  emplate app in y
+00000640: 6f75 7220 6e65 7720 6469 7265 6374 6f72  our new director
+00000650: 792e 200a 0a59 6f75 2063 616e 2072 756e  y. ..You can run
+00000660: 2074 6869 7320 6170 7020 696e 2064 6576   this app in dev
+00000670: 656c 6f70 6d65 6e74 206d 6f64 653a 0a0a  elopment mode:..
+00000680: 6060 6062 6173 680a 7265 666c 6578 2072  ```bash.reflex r
+00000690: 756e 0a60 6060 0a0a 596f 7520 7368 6f75  un.```..You shou
+000006a0: 6c64 2073 6565 2079 6f75 7220 6170 7020  ld see your app 
+000006b0: 7275 6e6e 696e 6720 6174 2068 7474 703a  running at http:
+000006c0: 2f2f 6c6f 6361 6c68 6f73 743a 3330 3030  //localhost:3000
+000006d0: 2e0a 0a4e 6f77 2079 6f75 2063 616e 206d  ...Now you can m
+000006e0: 6f64 6966 7920 7468 6520 736f 7572 6365  odify the source
+000006f0: 2063 6f64 6520 696e 2060 6d79 5f61 7070   code in `my_app
+00000700: 5f6e 616d 652f 6d79 5f61 7070 5f6e 616d  _name/my_app_nam
+00000710: 652e 7079 602e 2052 6566 6c65 7820 6861  e.py`. Reflex ha
+00000720: 7320 6661 7374 2072 6566 7265 7368 6573  s fast refreshes
+00000730: 2073 6f20 796f 7520 6361 6e20 7365 6520   so you can see 
+00000740: 796f 7572 2063 6861 6e67 6573 2069 6e73  your changes ins
+00000750: 7461 6e74 6c79 2077 6865 6e20 796f 7520  tantly when you 
+00000760: 7361 7665 2079 6f75 7220 636f 6465 2e0a  save your code..
+00000770: 0a0a 2323 20f0 9fab a720 4578 616d 706c  ..## .... Exampl
+00000780: 6520 4170 700a 0a4c 6574 2773 2067 6f20  e App..Let's go 
+00000790: 6f76 6572 2061 6e20 6578 616d 706c 653a  over an example:
+000007a0: 2063 7265 6174 696e 6720 616e 2069 6d61   creating an ima
+000007b0: 6765 2067 656e 6572 6174 696f 6e20 5549  ge generation UI
+000007c0: 2061 726f 756e 6420 4441 4c4c c2b7 452e   around DALL..E.
+000007d0: 2046 6f72 2073 696d 706c 6963 6974 792c   For simplicity,
+000007e0: 2077 6520 6a75 7374 2063 616c 6c20 7468   we just call th
+000007f0: 6520 4f70 656e 4149 2041 5049 2c20 6275  e OpenAI API, bu
+00000800: 7420 796f 7520 636f 756c 6420 7265 706c  t you could repl
+00000810: 6163 6520 7468 6973 2077 6974 6820 616e  ace this with an
+00000820: 204d 4c20 6d6f 6465 6c20 7275 6e20 6c6f   ML model run lo
+00000830: 6361 6c6c 792e 0a0a 266e 6273 703b 0a0a  cally...&nbsp;..
+00000840: 3c64 6976 2061 6c69 676e 3d22 6365 6e74  <div align="cent
+00000850: 6572 223e 0a3c 696d 6720 7372 633d 2264  er">.<img src="d
+00000860: 6f63 732f 696d 6167 6573 2f64 616c 6c65  ocs/images/dalle
+00000870: 2e67 6966 2220 616c 743d 2241 2066 726f  .gif" alt="A fro
+00000880: 6e74 656e 6420 7772 6170 7065 7220 666f  ntend wrapper fo
+00000890: 7220 4441 4c4c c2b7 452c 2073 686f 776e  r DALL..E, shown
+000008a0: 2069 6e20 7468 6520 7072 6f63 6573 7320   in the process 
+000008b0: 6f66 2067 656e 6572 6174 696e 6720 616e  of generating an
+000008c0: 2069 6d61 6765 2e22 2077 6964 7468 3d22   image." width="
+000008d0: 3535 3022 202f 3e0a 3c2f 6469 763e 0a0a  550" />.</div>..
+000008e0: 266e 6273 703b 0a0a 4865 7265 2069 7320  &nbsp;..Here is 
+000008f0: 7468 6520 636f 6d70 6c65 7465 2063 6f64  the complete cod
+00000900: 6520 746f 2063 7265 6174 6520 7468 6973  e to create this
+00000910: 2e20 5468 6973 2069 7320 616c 6c20 646f  . This is all do
+00000920: 6e65 2069 6e20 6f6e 6520 5079 7468 6f6e  ne in one Python
+00000930: 2066 696c 6521 0a0a 6060 6070 7974 686f   file!..```pytho
+00000940: 6e0a 696d 706f 7274 2072 6566 6c65 7820  n.import reflex 
+00000950: 6173 2072 780a 696d 706f 7274 206f 7065  as rx.import ope
+00000960: 6e61 690a 0a6f 7065 6e61 692e 6170 695f  nai..openai.api_
+00000970: 6b65 7920 3d20 2259 4f55 525f 4150 495f  key = "YOUR_API_
+00000980: 4b45 5922 0a0a 636c 6173 7320 5374 6174  KEY"..class Stat
+00000990: 6528 7278 2e53 7461 7465 293a 0a20 2020  e(rx.State):.   
+000009a0: 2022 2222 5468 6520 6170 7020 7374 6174   """The app stat
+000009b0: 652e 2222 220a 2020 2020 7072 6f6d 7074  e.""".    prompt
+000009c0: 203d 2022 220a 2020 2020 696d 6167 655f   = "".    image_
+000009d0: 7572 6c20 3d20 2222 0a20 2020 2070 726f  url = "".    pro
+000009e0: 6365 7373 696e 6720 3d20 4661 6c73 650a  cessing = False.
+000009f0: 2020 2020 636f 6d70 6c65 7465 203d 2046      complete = F
+00000a00: 616c 7365 0a0a 2020 2020 6465 6620 6765  alse..    def ge
+00000a10: 745f 696d 6167 6528 7365 6c66 293a 0a20  t_image(self):. 
+00000a20: 2020 2020 2020 2022 2222 4765 7420 7468         """Get th
+00000a30: 6520 696d 6167 6520 6672 6f6d 2074 6865  e image from the
+00000a40: 2070 726f 6d70 742e 2222 220a 2020 2020   prompt.""".    
+00000a50: 2020 2020 6966 2073 656c 662e 7072 6f6d      if self.prom
+00000a60: 7074 203d 3d20 2222 3a0a 2020 2020 2020  pt == "":.      
+00000a70: 2020 2020 2020 7265 7475 726e 2072 782e        return rx.
+00000a80: 7769 6e64 6f77 5f61 6c65 7274 2822 5072  window_alert("Pr
+00000a90: 6f6d 7074 2045 6d70 7479 2229 0a0a 2020  ompt Empty")..  
+00000aa0: 2020 2020 2020 7365 6c66 2e70 726f 6365        self.proce
+00000ab0: 7373 696e 672c 2073 656c 662e 636f 6d70  ssing, self.comp
+00000ac0: 6c65 7465 203d 2054 7275 652c 2046 616c  lete = True, Fal
+00000ad0: 7365 0a20 2020 2020 2020 2079 6965 6c64  se.        yield
+00000ae0: 0a20 2020 2020 2020 2072 6573 706f 6e73  .        respons
+00000af0: 6520 3d20 6f70 656e 6169 2e49 6d61 6765  e = openai.Image
+00000b00: 2e63 7265 6174 6528 7072 6f6d 7074 3d73  .create(prompt=s
+00000b10: 656c 662e 7072 6f6d 7074 2c20 6e3d 312c  elf.prompt, n=1,
+00000b20: 2073 697a 653d 2231 3032 3478 3130 3234   size="1024x1024
+00000b30: 2229 0a20 2020 2020 2020 2073 656c 662e  ").        self.
+00000b40: 696d 6167 655f 7572 6c20 3d20 7265 7370  image_url = resp
+00000b50: 6f6e 7365 5b22 6461 7461 225d 5b30 5d5b  onse["data"][0][
+00000b60: 2275 726c 225d 0a20 2020 2020 2020 2073  "url"].        s
+00000b70: 656c 662e 7072 6f63 6573 7369 6e67 2c20  elf.processing, 
+00000b80: 7365 6c66 2e63 6f6d 706c 6574 6520 3d20  self.complete = 
+00000b90: 4661 6c73 652c 2054 7275 650a 2020 2020  False, True.    
+00000ba0: 2020 2020 0a0a 6465 6620 696e 6465 7828      ..def index(
+00000bb0: 293a 0a20 2020 2072 6574 7572 6e20 7278  ):.    return rx
+00000bc0: 2e63 656e 7465 7228 0a20 2020 2020 2020  .center(.       
+00000bd0: 2072 782e 7673 7461 636b 280a 2020 2020   rx.vstack(.    
+00000be0: 2020 2020 2020 2020 7278 2e68 6561 6469          rx.headi
+00000bf0: 6e67 2822 4441 4c4c c2b7 4522 292c 0a20  ng("DALL..E"),. 
+00000c00: 2020 2020 2020 2020 2020 2072 782e 696e             rx.in
+00000c10: 7075 7428 706c 6163 6568 6f6c 6465 723d  put(placeholder=
+00000c20: 2245 6e74 6572 2061 2070 726f 6d70 7422  "Enter a prompt"
+00000c30: 2c20 6f6e 5f62 6c75 723d 5374 6174 652e  , on_blur=State.
+00000c40: 7365 745f 7072 6f6d 7074 292c 0a20 2020  set_prompt),.   
+00000c50: 2020 2020 2020 2020 2072 782e 6275 7474           rx.butt
+00000c60: 6f6e 280a 2020 2020 2020 2020 2020 2020  on(.            
+00000c70: 2020 2020 2247 656e 6572 6174 6520 496d      "Generate Im
+00000c80: 6167 6522 2c0a 2020 2020 2020 2020 2020  age",.          
+00000c90: 2020 2020 2020 6f6e 5f63 6c69 636b 3d53        on_click=S
+00000ca0: 7461 7465 2e67 6574 5f69 6d61 6765 2c0a  tate.get_image,.
+00000cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000cc0: 6973 5f6c 6f61 6469 6e67 3d53 7461 7465  is_loading=State
+00000cd0: 2e70 726f 6365 7373 696e 672c 0a20 2020  .processing,.   
+00000ce0: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00000cf0: 7468 3d22 3130 3025 222c 0a20 2020 2020  th="100%",.     
+00000d00: 2020 2020 2020 2029 2c0a 2020 2020 2020         ),.      
+00000d10: 2020 2020 2020 7278 2e63 6f6e 6428 0a20        rx.cond(. 
+00000d20: 2020 2020 2020 2020 2020 2020 2020 2053                 S
+00000d30: 7461 7465 2e63 6f6d 706c 6574 652c 0a20  tate.complete,. 
+00000d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d50: 2020 2020 7278 2e69 6d61 6765 280a 2020      rx.image(.  
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000d70: 2020 2020 2020 2073 7263 3d53 7461 7465         src=State
+00000d80: 2e69 6d61 6765 5f75 726c 2c0a 2020 2020  .image_url,.    
+00000d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000da0: 2020 2020 2068 6569 6768 743d 2232 3565       height="25e
+00000db0: 6d22 2c0a 2020 2020 2020 2020 2020 2020  m",.            
+00000dc0: 2020 2020 2020 2020 2020 2020 2077 6964               wid
+00000dd0: 7468 3d22 3235 656d 222c 0a20 2020 2020  th="25em",.     
+00000de0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00000df0: 0a20 2020 2020 2020 2020 2020 2029 2c0a  .            ),.
+00000e00: 2020 2020 2020 2020 2020 2020 7061 6464              padd
+00000e10: 696e 673d 2232 656d 222c 0a20 2020 2020  ing="2em",.     
+00000e20: 2020 2020 2020 2073 6861 646f 773d 226c         shadow="l
+00000e30: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
+00000e40: 626f 7264 6572 5f72 6164 6975 733d 226c  border_radius="l
+00000e50: 6722 2c0a 2020 2020 2020 2020 292c 0a20  g",.        ),. 
+00000e60: 2020 2020 2020 2077 6964 7468 3d22 3130         width="10
+00000e70: 3025 222c 0a20 2020 2020 2020 2068 6569  0%",.        hei
+00000e80: 6768 743d 2231 3030 7668 222c 0a20 2020  ght="100vh",.   
+00000e90: 2029 0a0a 2320 4164 6420 7374 6174 6520   )..# Add state 
+00000ea0: 616e 6420 7061 6765 2074 6f20 7468 6520  and page to the 
+00000eb0: 6170 702e 0a61 7070 203d 2072 782e 4170  app..app = rx.Ap
+00000ec0: 7028 290a 6170 702e 6164 645f 7061 6765  p().app.add_page
+00000ed0: 2869 6e64 6578 2c20 7469 746c 653d 2272  (index, title="r
+00000ee0: 6566 6c65 783a 4441 4c4c c2b7 4522 290a  eflex:DALL..E").
+00000ef0: 6170 702e 636f 6d70 696c 6528 290a 6060  app.compile().``
+00000f00: 600a 0a23 2320 4c65 7427 7320 6272 6561  `..## Let's brea
+00000f10: 6b20 7468 6973 2064 6f77 6e2e 0a0a 2323  k this down...##
+00000f20: 2320 2a2a 5265 666c 6578 2055 492a 2a0a  # **Reflex UI**.
+00000f30: 0a4c 6574 2773 2073 7461 7274 2077 6974  .Let's start wit
+00000f40: 6820 7468 6520 5549 2e0a 0a60 6060 7079  h the UI...```py
+00000f50: 7468 6f6e 0a64 6566 2069 6e64 6578 2829  thon.def index()
+00000f60: 3a0a 2020 2020 7265 7475 726e 2072 782e  :.    return rx.
+00000f70: 6365 6e74 6572 280a 2020 2020 2020 2020  center(.        
+00000f80: 2e2e 2e0a 2020 2020 290a 6060 600a 0a54  ....    ).```..T
+00000f90: 6869 7320 6069 6e64 6578 6020 6675 6e63  his `index` func
+00000fa0: 7469 6f6e 2064 6566 696e 6573 2074 6865  tion defines the
+00000fb0: 2066 726f 6e74 656e 6420 6f66 2074 6865   frontend of the
+00000fc0: 2061 7070 2e0a 0a57 6520 7573 6520 6469   app...We use di
+00000fd0: 6666 6572 656e 7420 636f 6d70 6f6e 656e  fferent componen
+00000fe0: 7473 2073 7563 6820 6173 2060 6365 6e74  ts such as `cent
+00000ff0: 6572 602c 2060 7673 7461 636b 602c 2060  er`, `vstack`, `
+00001000: 696e 7075 7460 2c20 616e 6420 6062 7574  input`, and `but
+00001010: 746f 6e60 2074 6f20 6275 696c 6420 7468  ton` to build th
+00001020: 6520 6672 6f6e 7465 6e64 2e20 436f 6d70  e frontend. Comp
+00001030: 6f6e 656e 7473 2063 616e 2062 6520 6e65  onents can be ne
+00001040: 7374 6564 2077 6974 6869 6e20 6561 6368  sted within each
+00001050: 206f 7468 6572 0a74 6f20 6372 6561 7465   other.to create
+00001060: 2063 6f6d 706c 6578 206c 6179 6f75 7473   complex layouts
+00001070: 2e20 416e 6420 796f 7520 6361 6e20 7573  . And you can us
+00001080: 6520 6b65 7977 6f72 6420 6172 6773 2074  e keyword args t
+00001090: 6f20 7374 796c 6520 7468 656d 2077 6974  o style them wit
+000010a0: 6820 7468 6520 6675 6c6c 2070 6f77 6572  h the full power
+000010b0: 206f 6620 4353 532e 0a0a 5265 666c 6578   of CSS...Reflex
+000010c0: 2063 6f6d 6573 2077 6974 6820 5b36 302b   comes with [60+
+000010d0: 2062 7569 6c74 2d69 6e20 636f 6d70 6f6e   built-in compon
+000010e0: 656e 7473 5d28 6874 7470 733a 2f2f 7265  ents](https://re
+000010f0: 666c 6578 2e64 6576 2f64 6f63 732f 6c69  flex.dev/docs/li
+00001100: 6272 6172 7929 2074 6f20 6865 6c70 2079  brary) to help y
+00001110: 6f75 2067 6574 2073 7461 7274 6564 2e20  ou get started. 
+00001120: 5765 2061 7265 2061 6374 6976 656c 7920  We are actively 
+00001130: 6164 6469 6e67 206d 6f72 6520 636f 6d70  adding more comp
+00001140: 6f6e 656e 7473 2c20 616e 6420 6974 2773  onents, and it's
+00001150: 2065 6173 7920 746f 205b 6372 6561 7465   easy to [create
+00001160: 2079 6f75 7220 6f77 6e20 636f 6d70 6f6e   your own compon
+00001170: 656e 7473 5d28 6874 7470 733a 2f2f 7265  ents](https://re
+00001180: 666c 6578 2e64 6576 2f64 6f63 732f 6164  flex.dev/docs/ad
+00001190: 7661 6e63 6564 2d67 7569 6465 2f77 7261  vanced-guide/wra
+000011a0: 7070 696e 672d 7265 6163 7429 2e0a 0a23  pping-react)...#
+000011b0: 2323 202a 2a53 7461 7465 2a2a 0a0a 5265  ## **State**..Re
+000011c0: 666c 6578 2072 6570 7265 7365 6e74 7320  flex represents 
+000011d0: 796f 7572 2055 4920 6173 2061 2066 756e  your UI as a fun
+000011e0: 6374 696f 6e20 6f66 2079 6f75 7220 7374  ction of your st
+000011f0: 6174 652e 0a0a 6060 6070 7974 686f 6e0a  ate...```python.
+00001200: 636c 6173 7320 5374 6174 6528 7278 2e53  class State(rx.S
+00001210: 7461 7465 293a 0a20 2020 2022 2222 5468  tate):.    """Th
+00001220: 6520 6170 7020 7374 6174 652e 2222 220a  e app state.""".
+00001230: 2020 2020 7072 6f6d 7074 203d 2022 220a      prompt = "".
+00001240: 2020 2020 696d 6167 655f 7572 6c20 3d20      image_url = 
+00001250: 2222 0a20 2020 2070 726f 6365 7373 696e  "".    processin
+00001260: 6720 3d20 4661 6c73 650a 2020 2020 636f  g = False.    co
+00001270: 6d70 6c65 7465 203d 2046 616c 7365 0a60  mplete = False.`
+00001280: 6060 0a0a 5468 6520 7374 6174 6520 6465  ``..The state de
+00001290: 6669 6e65 7320 616c 6c20 7468 6520 7661  fines all the va
+000012a0: 7269 6162 6c65 7320 2863 616c 6c65 6420  riables (called 
+000012b0: 7661 7273 2920 696e 2061 6e20 6170 7020  vars) in an app 
+000012c0: 7468 6174 2063 616e 2063 6861 6e67 6520  that can change 
+000012d0: 616e 6420 7468 6520 6675 6e63 7469 6f6e  and the function
+000012e0: 7320 7468 6174 2063 6861 6e67 6520 7468  s that change th
+000012f0: 656d 2e0a 0a48 6572 6520 7468 6520 7374  em...Here the st
+00001300: 6174 6520 6973 2063 6f6d 7072 6973 6564  ate is comprised
+00001310: 206f 6620 6120 6070 726f 6d70 7460 2061   of a `prompt` a
+00001320: 6e64 2060 696d 6167 655f 7572 6c60 2e20  nd `image_url`. 
+00001330: 5468 6572 6520 6172 6520 616c 736f 2074  There are also t
+00001340: 6865 2062 6f6f 6c65 616e 7320 6070 726f  he booleans `pro
+00001350: 6365 7373 696e 6760 2061 6e64 2060 636f  cessing` and `co
+00001360: 6d70 6c65 7465 6020 746f 2069 6e64 6963  mplete` to indic
+00001370: 6174 6520 7768 656e 2074 6f20 7368 6f77  ate when to show
+00001380: 2074 6865 2063 6972 6375 6c61 7220 7072   the circular pr
+00001390: 6f67 7265 7373 2061 6e64 2069 6d61 6765  ogress and image
+000013a0: 2e0a 0a23 2323 202a 2a45 7665 6e74 2048  ...### **Event H
+000013b0: 616e 646c 6572 732a 2a0a 0a60 6060 7079  andlers**..```py
+000013c0: 7468 6f6e 0a64 6566 2067 6574 5f69 6d61  thon.def get_ima
+000013d0: 6765 2873 656c 6629 3a0a 2020 2020 2222  ge(self):.    ""
+000013e0: 2247 6574 2074 6865 2069 6d61 6765 2066  "Get the image f
+000013f0: 726f 6d20 7468 6520 7072 6f6d 7074 2e22  rom the prompt."
+00001400: 2222 0a20 2020 2069 6620 7365 6c66 2e70  "".    if self.p
+00001410: 726f 6d70 7420 3d3d 2022 223a 0a20 2020  rompt == "":.   
+00001420: 2020 2020 2072 6574 7572 6e20 7278 2e77       return rx.w
+00001430: 696e 646f 775f 616c 6572 7428 2250 726f  indow_alert("Pro
+00001440: 6d70 7420 456d 7074 7922 290a 0a20 2020  mpt Empty")..   
+00001450: 2073 656c 662e 7072 6f63 6573 7369 6e67   self.processing
+00001460: 2c20 7365 6c66 2e63 6f6d 706c 6574 6520  , self.complete 
+00001470: 3d20 5472 7565 2c20 4661 6c73 650a 2020  = True, False.  
+00001480: 2020 7969 656c 640a 2020 2020 7265 7370    yield.    resp
+00001490: 6f6e 7365 203d 206f 7065 6e61 692e 496d  onse = openai.Im
+000014a0: 6167 652e 6372 6561 7465 2870 726f 6d70  age.create(promp
+000014b0: 743d 7365 6c66 2e70 726f 6d70 742c 206e  t=self.prompt, n
+000014c0: 3d31 2c20 7369 7a65 3d22 3130 3234 7831  =1, size="1024x1
+000014d0: 3032 3422 290a 2020 2020 7365 6c66 2e69  024").    self.i
+000014e0: 6d61 6765 5f75 726c 203d 2072 6573 706f  mage_url = respo
+000014f0: 6e73 655b 2264 6174 6122 5d5b 305d 5b22  nse["data"][0]["
+00001500: 7572 6c22 5d0a 2020 2020 7365 6c66 2e70  url"].    self.p
+00001510: 726f 6365 7373 696e 672c 2073 656c 662e  rocessing, self.
+00001520: 636f 6d70 6c65 7465 203d 2046 616c 7365  complete = False
+00001530: 2c20 5472 7565 0a60 6060 0a0a 5769 7468  , True.```..With
+00001540: 696e 2074 6865 2073 7461 7465 2c20 7765  in the state, we
+00001550: 2064 6566 696e 6520 6675 6e63 7469 6f6e   define function
+00001560: 7320 6361 6c6c 6564 2065 7665 6e74 2068  s called event h
+00001570: 616e 646c 6572 7320 7468 6174 2063 6861  andlers that cha
+00001580: 6e67 6520 7468 6520 7374 6174 6520 7661  nge the state va
+00001590: 7273 2e20 4576 656e 7420 6861 6e64 6c65  rs. Event handle
+000015a0: 7273 2061 7265 2074 6865 2077 6179 2074  rs are the way t
+000015b0: 6861 7420 7765 2063 616e 206d 6f64 6966  hat we can modif
+000015c0: 7920 7468 6520 7374 6174 6520 696e 2052  y the state in R
+000015d0: 6566 6c65 782e 2054 6865 7920 6361 6e20  eflex. They can 
+000015e0: 6265 2063 616c 6c65 6420 696e 2072 6573  be called in res
+000015f0: 706f 6e73 6520 746f 2075 7365 7220 6163  ponse to user ac
+00001600: 7469 6f6e 732c 2073 7563 6820 6173 2063  tions, such as c
+00001610: 6c69 636b 696e 6720 6120 6275 7474 6f6e  licking a button
+00001620: 206f 7220 7479 7069 6e67 2069 6e20 6120   or typing in a 
+00001630: 7465 7874 2062 6f78 2e20 5468 6573 6520  text box. These 
+00001640: 6163 7469 6f6e 7320 6172 6520 6361 6c6c  actions are call
+00001650: 6564 2065 7665 6e74 732e 0a0a 4f75 7220  ed events...Our 
+00001660: 4441 4c4c c2b7 452e 2061 7070 2068 6173  DALL..E. app has
+00001670: 2061 6e20 6576 656e 7420 6861 6e64 6c65   an event handle
+00001680: 722c 2060 6765 745f 696d 6167 6560 2074  r, `get_image` t
+00001690: 6f20 7768 6963 6820 6765 7420 7468 6973  o which get this
+000016a0: 2069 6d61 6765 2066 726f 6d20 7468 6520   image from the 
+000016b0: 4f70 656e 4149 2041 5049 2e20 5573 696e  OpenAI API. Usin
+000016c0: 6720 6079 6965 6c64 6020 696e 2074 6865  g `yield` in the
+000016d0: 206d 6964 646c 6520 6f66 2061 6e20 6576   middle of an ev
+000016e0: 656e 7420 6861 6e64 6c65 7220 7769 6c6c  ent handler will
+000016f0: 2063 6175 7365 2074 6865 2055 4920 746f   cause the UI to
+00001700: 2075 7064 6174 652e 204f 7468 6572 7769   update. Otherwi
+00001710: 7365 2074 6865 2055 4920 7769 6c6c 2075  se the UI will u
+00001720: 7064 6174 6520 6174 2074 6865 2065 6e64  pdate at the end
+00001730: 206f 6620 7468 6520 6576 656e 7420 6861   of the event ha
+00001740: 6e64 6c65 722e 0a0a 2323 2320 2a2a 526f  ndler...### **Ro
+00001750: 7574 696e 672a 2a0a 0a46 696e 616c 6c79  uting**..Finally
+00001760: 2c20 7765 2064 6566 696e 6520 6f75 7220  , we define our 
+00001770: 6170 702e 0a0a 6060 6070 7974 686f 6e0a  app...```python.
+00001780: 6170 7020 3d20 7278 2e41 7070 2829 0a60  app = rx.App().`
+00001790: 6060 0a0a 5765 2061 6464 2061 2070 6167  ``..We add a pag
+000017a0: 6520 6672 6f6d 2074 6865 2072 6f6f 7420  e from the root 
+000017b0: 6f66 2074 6865 2061 7070 2074 6f20 7468  of the app to th
+000017c0: 6520 696e 6465 7820 636f 6d70 6f6e 656e  e index componen
+000017d0: 742e 2057 6520 616c 736f 2061 6464 2061  t. We also add a
+000017e0: 2074 6974 6c65 2074 6861 7420 7769 6c6c   title that will
+000017f0: 2073 686f 7720 7570 2069 6e20 7468 6520   show up in the 
+00001800: 7061 6765 2070 7265 7669 6577 2f62 726f  page preview/bro
+00001810: 7773 6572 2074 6162 2e0a 0a60 6060 7079  wser tab...```py
+00001820: 7468 6f6e 0a61 7070 2e61 6464 5f70 6167  thon.app.add_pag
+00001830: 6528 696e 6465 782c 2074 6974 6c65 3d22  e(index, title="
+00001840: 4441 4c4c 2d45 2229 0a61 7070 2e63 6f6d  DALL-E").app.com
+00001850: 7069 6c65 2829 0a60 6060 0a0a 596f 7520  pile().```..You 
+00001860: 6361 6e20 6372 6561 7465 2061 206d 756c  can create a mul
+00001870: 7469 2d70 6167 6520 6170 7020 6279 2061  ti-page app by a
+00001880: 6464 696e 6720 6d6f 7265 2070 6167 6573  dding more pages
+00001890: 2e0a 0a23 2320 f09f 9391 2052 6573 6f75  ...## .... Resou
+000018a0: 7263 6573 0a0a 3c64 6976 2061 6c69 676e  rces..<div align
+000018b0: 3d22 6365 6e74 6572 223e 0a0a f09f 9391  ="center">......
+000018c0: 205b 446f 6373 5d28 6874 7470 733a 2f2f   [Docs](https://
+000018d0: 7265 666c 6578 2e64 6576 2f64 6f63 732f  reflex.dev/docs/
+000018e0: 6765 7474 696e 672d 7374 6172 7465 642f  getting-started/
+000018f0: 696e 7472 6f64 7563 7469 6f6e 2920 266e  introduction) &n
+00001900: 6273 703b 207c 2020 266e 6273 703b 20f0  bsp; |  &nbsp; .
+00001910: 9f97 9eef b88f 205b 426c 6f67 5d28 6874  ...... [Blog](ht
+00001920: 7470 733a 2f2f 7265 666c 6578 2e64 6576  tps://reflex.dev
+00001930: 2f62 6c6f 6729 2026 6e62 7370 3b20 7c20  /blog) &nbsp; | 
+00001940: 2026 6e62 7370 3b20 f09f 93b1 205b 436f   &nbsp; .... [Co
+00001950: 6d70 6f6e 656e 7420 4c69 6272 6172 795d  mponent Library]
+00001960: 2868 7474 7073 3a2f 2f72 6566 6c65 782e  (https://reflex.
+00001970: 6465 762f 646f 6373 2f6c 6962 7261 7279  dev/docs/library
+00001980: 2920 266e 6273 703b 207c 2020 266e 6273  ) &nbsp; |  &nbs
+00001990: 703b 20f0 9f96 bcef b88f 205b 4761 6c6c  p; ....... [Gall
+000019a0: 6572 795d 2868 7474 7073 3a2f 2f72 6566  ery](https://ref
+000019b0: 6c65 782e 6465 762f 646f 6373 2f67 616c  lex.dev/docs/gal
+000019c0: 6c65 7279 2920 266e 6273 703b 207c 2020  lery) &nbsp; |  
+000019d0: 266e 6273 703b 20f0 9f9b b820 5b44 6570  &nbsp; .... [Dep
+000019e0: 6c6f 796d 656e 745d 2868 7474 7073 3a2f  loyment](https:/
+000019f0: 2f72 6566 6c65 782e 6465 762f 646f 6373  /reflex.dev/docs
+00001a00: 2f68 6f73 7469 6e67 2f64 6570 6c6f 7929  /hosting/deploy)
+00001a10: 2020 266e 6273 703b 2020 200a 0a3c 2f64    &nbsp;   ..</d
+00001a20: 6976 3e0a 0a0a 0a0a 0a23 2320 e29c 8520  iv>......## ... 
+00001a30: 5374 6174 7573 0a0a 5265 666c 6578 206c  Status..Reflex l
+00001a40: 6175 6e63 6865 6420 696e 2044 6563 656d  aunched in Decem
+00001a50: 6265 7220 3230 3232 2077 6974 6820 7468  ber 2022 with th
+00001a60: 6520 6e61 6d65 2050 796e 6563 6f6e 652e  e name Pynecone.
+00001a70: 0a0a 4173 206f 6620 4a75 6c79 2032 3032  ..As of July 202
+00001a80: 332c 2077 6520 6172 6520 696e 2074 6865  3, we are in the
+00001a90: 202a 2a50 7562 6c69 6320 4265 7461 2a2a   **Public Beta**
+00001aa0: 2073 7461 6765 2e0a 0a2d 2020 203a 7768   stage...-   :wh
+00001ab0: 6974 655f 6368 6563 6b5f 6d61 726b 3a20  ite_check_mark: 
+00001ac0: 2a2a 5075 626c 6963 2041 6c70 6861 2a2a  **Public Alpha**
+00001ad0: 3a20 416e 796f 6e65 2063 616e 2069 6e73  : Anyone can ins
+00001ae0: 7461 6c6c 2061 6e64 2075 7365 2052 6566  tall and use Ref
+00001af0: 6c65 782e 2054 6865 7265 206d 6179 2062  lex. There may b
+00001b00: 6520 6973 7375 6573 2c20 6275 7420 7765  e issues, but we
+00001b10: 2061 7265 2077 6f72 6b69 6e67 2074 6f20   are working to 
+00001b20: 7265 736f 6c76 6520 7468 656d 2061 6374  resolve them act
+00001b30: 6976 656c 792e 0a2d 2020 203a 6c61 7267  ively..-   :larg
+00001b40: 655f 6f72 616e 6765 5f64 6961 6d6f 6e64  e_orange_diamond
+00001b50: 3a20 2a2a 5075 626c 6963 2042 6574 612a  : **Public Beta*
+00001b60: 2a3a 2053 7461 626c 6520 656e 6f75 6768  *: Stable enough
+00001b70: 2066 6f72 206e 6f6e 2d65 6e74 6572 7072   for non-enterpr
+00001b80: 6973 6520 7573 652d 6361 7365 732e 0a2d  ise use-cases..-
+00001b90: 2020 202a 2a50 7562 6c69 6320 486f 7374     **Public Host
+00001ba0: 696e 6720 4265 7461 2a2a 3a20 5f4f 7074  ing Beta**: _Opt
+00001bb0: 696f 6e61 6c6c 795f 2c20 6465 706c 6f79  ionally_, deploy
+00001bc0: 2061 6e64 2068 6f73 7420 796f 7572 2061   and host your a
+00001bd0: 7070 7320 6f6e 2052 6566 6c65 7821 0a2d  pps on Reflex!.-
+00001be0: 2020 202a 2a50 7562 6c69 632a 2a3a 2052     **Public**: R
+00001bf0: 6566 6c65 7820 6973 2070 726f 6475 6374  eflex is product
+00001c00: 696f 6e20 7265 6164 792e 0a0a 5265 666c  ion ready...Refl
+00001c10: 6578 2068 6173 206e 6577 2072 656c 6561  ex has new relea
+00001c20: 7365 7320 616e 6420 6665 6174 7572 6573  ses and features
+00001c30: 2063 6f6d 696e 6720 6576 6572 7920 7765   coming every we
+00001c40: 656b 2120 4d61 6b65 2073 7572 6520 746f  ek! Make sure to
+00001c50: 203a 7374 6172 3a20 7374 6172 2061 6e64   :star: star and
+00001c60: 203a 6579 6573 3a20 7761 7463 6820 7468   :eyes: watch th
+00001c70: 6973 2072 6570 6f73 6974 6f72 7920 746f  is repository to
+00001c80: 2073 7461 7920 7570 2074 6f20 6461 7465   stay up to date
+00001c90: 2e0a 0a23 2320 436f 6e74 7269 6275 7469  ...## Contributi
+00001ca0: 6e67 0a0a 5765 2077 656c 636f 6d65 2063  ng..We welcome c
+00001cb0: 6f6e 7472 6962 7574 696f 6e73 206f 6620  ontributions of 
+00001cc0: 616e 7920 7369 7a65 2120 4265 6c6f 7720  any size! Below 
+00001cd0: 6172 6520 736f 6d65 2067 6f6f 6420 7761  are some good wa
+00001ce0: 7973 2074 6f20 6765 7420 7374 6172 7465  ys to get starte
+00001cf0: 6420 696e 2074 6865 2052 6566 6c65 7820  d in the Reflex 
+00001d00: 636f 6d6d 756e 6974 792e 0a0a 2d20 2020  community...-   
+00001d10: 2a2a 4a6f 696e 204f 7572 2044 6973 636f  **Join Our Disco
+00001d20: 7264 2a2a 3a20 4f75 7220 5b44 6973 636f  rd**: Our [Disco
+00001d30: 7264 5d28 6874 7470 733a 2f2f 6469 7363  rd](https://disc
+00001d40: 6f72 642e 6767 2f54 3557 5362 4332 5974  ord.gg/T5WSbC2Yt
+00001d50: 5129 2069 7320 7468 6520 6265 7374 2070  Q) is the best p
+00001d60: 6c61 6365 2074 6f20 6765 7420 6865 6c70  lace to get help
+00001d70: 206f 6e20 796f 7572 2052 6566 6c65 7820   on your Reflex 
+00001d80: 7072 6f6a 6563 7420 616e 6420 746f 2064  project and to d
+00001d90: 6973 6375 7373 2068 6f77 2079 6f75 2063  iscuss how you c
+00001da0: 616e 2063 6f6e 7472 6962 7574 652e 0a2d  an contribute..-
+00001db0: 2020 202a 2a47 6974 4875 6220 4469 7363     **GitHub Disc
+00001dc0: 7573 7369 6f6e 732a 2a3a 2041 2067 7265  ussions**: A gre
+00001dd0: 6174 2077 6179 2074 6f20 7461 6c6b 2061  at way to talk a
+00001de0: 626f 7574 2066 6561 7475 7265 7320 796f  bout features yo
+00001df0: 7520 7761 6e74 2061 6464 6564 206f 7220  u want added or 
+00001e00: 7468 696e 6773 2074 6861 7420 6172 6520  things that are 
+00001e10: 636f 6e66 7573 696e 672f 6e65 6564 2063  confusing/need c
+00001e20: 6c61 7269 6669 6361 7469 6f6e 2e0a 2d20  larification..- 
+00001e30: 2020 2a2a 4769 7448 7562 2049 7373 7565    **GitHub Issue
+00001e40: 732a 2a3a 2054 6865 7365 2061 7265 2061  s**: These are a
+00001e50: 6e20 6578 6365 6c6c 656e 7420 7761 7920  n excellent way 
+00001e60: 746f 2072 6570 6f72 7420 6275 6773 2e20  to report bugs. 
+00001e70: 4164 6469 7469 6f6e 616c 6c79 2c20 796f  Additionally, yo
+00001e80: 7520 6361 6e20 7472 7920 616e 6420 736f  u can try and so
+00001e90: 6c76 6520 616e 2065 7869 7374 696e 6720  lve an existing 
+00001ea0: 6973 7375 6520 616e 6420 7375 626d 6974  issue and submit
+00001eb0: 2061 2050 522e 0a0a 5765 2061 7265 2061   a PR...We are a
+00001ec0: 6374 6976 656c 7920 6c6f 6f6b 696e 6720  ctively looking 
+00001ed0: 666f 7220 636f 6e74 7269 6275 746f 7273  for contributors
+00001ee0: 2c20 6e6f 206d 6174 7465 7220 796f 7572  , no matter your
+00001ef0: 2073 6b69 6c6c 206c 6576 656c 206f 7220   skill level or 
+00001f00: 6578 7065 7269 656e 6365 2e0a 0a23 2320  experience...## 
+00001f10: 4c69 6365 6e73 650a 0a52 6566 6c65 7820  License..Reflex 
+00001f20: 6973 206f 7065 6e2d 736f 7572 6365 2061  is open-source a
+00001f30: 6e64 206c 6963 656e 7365 6420 756e 6465  nd licensed unde
+00001f40: 7220 7468 6520 5b41 7061 6368 6520 4c69  r the [Apache Li
+00001f50: 6365 6e73 6520 322e 305d 284c 4943 454e  cense 2.0](LICEN
+00001f60: 5345 292e 0a                             SE)..
```

### Comparing `reflex-0.2.3a9/pyproject.toml` & `reflex-0.2.4a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reflex"
-version = "0.2.3a9"
+version = "0.2.4a1"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `reflex-0.2.3a9/reflex/.templates/apps/counter/counter.py` & `reflex-0.2.4a1/reflex/.templates/apps/counter/counter.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/apps/default/default.py` & `reflex-0.2.4a1/reflex/.templates/apps/default/default.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/jinja/web/pages/index.js.jinja2` & `reflex-0.2.4a1/reflex/.templates/jinja/web/pages/index.js.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -45,33 +45,37 @@
     }
 
     // If we are not processing an event, process the next event.
     if (!{{const.result}}.{{const.processing}}) {
       processEvent({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
     }
 
-    // If there is a new result, update the state.
-    if ({{const.result}}.{{const.state}} != null) {
-      // Apply the new result to the state and the new events to the queue.
-      {{state_name|react_setter}}(state => ({
-        ...{{const.result}}.{{const.state}},
-        events: [...state.{{const.events}}, ...{{const.result}}.{{const.events}}],
-      }))
+    // Reset the result.
+    {{const.result|react_setter}}(result => {
+      // If there is a new result, update the state.
+      if ({{const.result}}.{{const.state}} != null) {
+        // Apply the new result to the state and the new events to the queue.
+        {{state_name|react_setter}}(state => {
+          return {
+            ...{{const.result}}.{{const.state}},
+            events: [...state.{{const.events}}, ...{{const.result}}.{{const.events}}],
+          } 
+        })
+        return {
+          {{const.state}}: null,
+          {{const.events}}: [],
+          {{const.final}}: true,
+          {{const.processing}}: !{{const.result}}.{{const.final}},
+        }
+      }
+      return result;
+    })
 
-      // Reset the result.
-      {{const.result|react_setter}}(result => ({
-        {{const.state}}: null,
-        {{const.events}}: [],
-        {{const.final}}: true,
-        {{const.processing}}: !{{const.result}}.{{const.final}},
-      }))
-
-      // Process the next event.
-      processEvent({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
-    }
+    // Process the next event.
+    processEvent({{state_name}}, {{state_name|react_setter}}, {{const.result}}, {{const.result|react_setter}}, {{const.router}}, {{const.socket}}.current)
   })
 
   // Set focus to the specified element.
   useEffect(() => {
     if (focusRef.current) {
       focusRef.current.focus();
     }
```

### Comparing `reflex-0.2.3a9/reflex/.templates/jinja/web/pages/utils.js.jinja2` & `reflex-0.2.4a1/reflex/.templates/jinja/web/pages/utils.js.jinja2`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/web/bun.lockb` & `reflex-0.2.4a1/reflex/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/web/package.json` & `reflex-0.2.4a1/reflex/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/web/pages/_app.js` & `reflex-0.2.4a1/reflex/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/web/styles/code/prism.js` & `reflex-0.2.4a1/reflex/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/.templates/web/utils/state.js` & `reflex-0.2.4a1/reflex/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/__init__.py` & `reflex-0.2.4a1/reflex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Import all classes and functions the end user will need to make an app.
 
 Anything imported here will be available in the default Reflex import as `rx.*`.
-To signal to typecheckers that something should be reexported, 
+To signal to typecheckers that something should be reexported,
 we use the Flask "import name as name" syntax.
 """
 
 from . import el as el
 from .admin import AdminDash as AdminDash
 from .app import App as App
 from .app import UploadFile as UploadFile
```

### Comparing `reflex-0.2.3a9/reflex/app.py` & `reflex-0.2.4a1/reflex/app.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/base.py` & `reflex-0.2.4a1/reflex/base.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/compiler/compiler.py` & `reflex-0.2.4a1/reflex/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/compiler/templates.py` & `reflex-0.2.4a1/reflex/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/compiler/utils.py` & `reflex-0.2.4a1/reflex/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/__init__.py` & `reflex-0.2.4a1/reflex/components/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Import all the components."""
 from __future__ import annotations
 
 from .base import Script
 from .component import Component
+from .component import NoSSRComponent as NoSSRComponent
 from .datadisplay import *
 from .disclosure import *
 from .feedback import *
 from .forms import *
 from .graphing import *
 from .layout import *
 from .media import *
```

### Comparing `reflex-0.2.3a9/reflex/components/base/bare.py` & `reflex-0.2.4a1/reflex/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/base/document.py` & `reflex-0.2.4a1/reflex/components/base/document.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/base/link.py` & `reflex-0.2.4a1/reflex/components/base/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/base/meta.py` & `reflex-0.2.4a1/reflex/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/base/script.py` & `reflex-0.2.4a1/reflex/components/base/script.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/component.py` & `reflex-0.2.4a1/reflex/components/component.py`

 * *Files 7% similar despite different names*

```diff
@@ -773,7 +773,25 @@
     """
 
     @wraps(component_fn)
     def wrapper(*children, **props) -> CustomComponent:
         return CustomComponent(component_fn=component_fn, children=children, **props)
 
     return wrapper
+
+
+class NoSSRComponent(Component):
+    """A dynamic component that is not rendered on the server."""
+
+    def _get_imports(self):
+        return {"next/dynamic": {ImportVar(tag="dynamic", is_default=True)}}
+
+    def _get_custom_code(self) -> str:
+        opts_fragment = ", { ssr: false });"
+        library_import = f"const {self.tag} = dynamic(() => import('{self.library}')"
+        mod_import = (
+            # https://nextjs.org/docs/pages/building-your-application/optimizing/lazy-loading#with-named-exports
+            f".then((mod) => mod.{self.tag})"
+            if not self.is_default
+            else ""
+        )
+        return "".join((library_import, mod_import, opts_fragment))
```

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/code.py` & `reflex-0.2.4a1/reflex/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/datatable.py` & `reflex-0.2.4a1/reflex/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/divider.py` & `reflex-0.2.4a1/reflex/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/list.py` & `reflex-0.2.4a1/reflex/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/stat.py` & `reflex-0.2.4a1/reflex/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/table.py` & `reflex-0.2.4a1/reflex/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/datadisplay/tag.py` & `reflex-0.2.4a1/reflex/components/datadisplay/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/disclosure/accordion.py` & `reflex-0.2.4a1/reflex/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/disclosure/tabs.py` & `reflex-0.2.4a1/reflex/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/disclosure/transition.py` & `reflex-0.2.4a1/reflex/components/disclosure/transition.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/feedback/alert.py` & `reflex-0.2.4a1/reflex/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/feedback/circularprogress.py` & `reflex-0.2.4a1/reflex/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/feedback/progress.py` & `reflex-0.2.4a1/reflex/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/feedback/skeleton.py` & `reflex-0.2.4a1/reflex/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/feedback/spinner.py` & `reflex-0.2.4a1/reflex/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/__init__.py` & `reflex-0.2.4a1/reflex/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/button.py` & `reflex-0.2.4a1/reflex/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/checkbox.py` & `reflex-0.2.4a1/reflex/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/colormodeswitch.py` & `reflex-0.2.4a1/reflex/components/forms/colormodeswitch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/copytoclipboard.py` & `reflex-0.2.4a1/reflex/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/debounce.py` & `reflex-0.2.4a1/reflex/components/forms/debounce.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,48 +16,52 @@
     is experiencing high latency.
     """
 
     library = "react-debounce-input"
     tag = "DebounceInput"
 
     # Minimum input characters before triggering the on_change event
-    min_length: Var[int] = 0  # type: ignore
+    min_length: Var[int]
 
     # Time to wait between end of input and triggering on_change
-    debounce_timeout: Var[int] = 100  # type: ignore
+    debounce_timeout: Var[int]
 
     # If true, notify when Enter key is pressed
-    force_notify_by_enter: Var[bool] = True  # type: ignore
+    force_notify_by_enter: Var[bool]
 
     # If true, notify when form control loses focus
-    force_notify_on_blur: Var[bool] = True  # type: ignore
+    force_notify_on_blur: Var[bool]
+
+    # If provided, create a fully-controlled input
+    value: Var[str]
 
     def _render(self) -> Tag:
         """Carry first child props directly on this tag.
 
         Since react-debounce-input wants to create and manage the underlying
         input component itself, we carry all props, events, and styles from
         the child, and then neuter the child's render method so it produces no output.
 
         Returns:
             The rendered debounce element wrapping the first child element.
 
         Raises:
             RuntimeError: unless exactly one child element is provided.
         """
-        if not self.children or len(self.children) > 1:
+        child, props = _collect_first_child_and_props(self)
+        if isinstance(child, type(self)) or len(self.children) > 1:
             raise RuntimeError(
                 "Provide a single child for DebounceInput, such as rx.input() or "
                 "rx.text_area()",
             )
-        child = self.children[0]
+        self.children = []
         tag = super()._render()
         tag.add_props(
+            **props,
             **child.event_triggers,
-            **props_not_none(child),
             sx=child.style,
             id=child.id,
             class_name=child.class_name,
             element=Var.create("{%s}" % child.tag, is_local=False, is_string=False),
         )
         # do NOT render the child, DebounceInput will create it
         object.__setattr__(child, "render", lambda: "")
@@ -71,7 +75,33 @@
         c: the component to get_props from
 
     Returns:
         dict of all props that are not None.
     """
     cdict = {a: getattr(c, a) for a in c.get_props() if getattr(c, a, None) is not None}
     return cdict
+
+
+def _collect_first_child_and_props(c: Component) -> tuple[Component, dict[str, Any]]:
+    """Recursively find the first child of a different type than `c` with props.
+
+    This function is used to collapse nested DebounceInput components by
+    applying props from each level. Parent props take precedent over child
+    props. The first child component that differs in type will be returned
+    along with all combined parent props seen along the way.
+
+    Args:
+        c: the component to get_props from
+
+    Returns:
+        tuple containing the first nested child of a different type and the collected
+        props from each component traversed.
+    """
+    props = props_not_none(c)
+    if not c.children:
+        return c, props
+    child = c.children[0]
+    if not isinstance(child, type(c)):
+        return child, {**props_not_none(child), **props}
+    # carry props from nested DebounceInput components
+    recursive_child, child_props = _collect_first_child_and_props(child)
+    return recursive_child, {**child_props, **props}
```

### Comparing `reflex-0.2.3a9/reflex/components/forms/editable.py` & `reflex-0.2.4a1/reflex/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/form.py` & `reflex-0.2.4a1/reflex/components/forms/form.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/iconbutton.py` & `reflex-0.2.4a1/reflex/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/input.py` & `reflex-0.2.4a1/reflex/components/forms/input.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """An input component."""
 
 from typing import Dict
 
-from reflex.components.component import EVENT_ARG
+from reflex.components.component import EVENT_ARG, Component
+from reflex.components.forms.debounce import DebounceInput
 from reflex.components.libs.chakra import ChakraComponent
 from reflex.utils import imports
 from reflex.vars import ImportVar, Var
 
 
 class Input(ChakraComponent):
     """The Input component is a component that is used to get user input in a text field."""
@@ -65,14 +66,32 @@
             "on_change": EVENT_ARG.target.value,
             "on_focus": EVENT_ARG.target.value,
             "on_blur": EVENT_ARG.target.value,
             "on_key_down": EVENT_ARG.key,
             "on_key_up": EVENT_ARG.key,
         }
 
+    @classmethod
+    def create(cls, *children, **props) -> Component:
+        """Create an Input component.
+
+        Args:
+            children: The children of the component.
+            props: The properties of the component.
+
+        Returns:
+            The component.
+        """
+        if isinstance(props.get("value"), Var) and props.get("on_change"):
+            # create a debounced input if the user requests full control to avoid typing jank
+            return DebounceInput.create(
+                super().create(*children, **props), debounce_timeout=0
+            )
+        return super().create(*children, **props)
+
 
 class InputGroup(ChakraComponent):
     """The InputGroup component is a component that is used to group a set of inputs."""
 
     tag = "InputGroup"
```

### Comparing `reflex-0.2.3a9/reflex/components/forms/multiselect.py` & `reflex-0.2.4a1/reflex/components/forms/multiselect.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/numberinput.py` & `reflex-0.2.4a1/reflex/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/pininput.py` & `reflex-0.2.4a1/reflex/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/radio.py` & `reflex-0.2.4a1/reflex/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/rangeslider.py` & `reflex-0.2.4a1/reflex/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/select.py` & `reflex-0.2.4a1/reflex/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/slider.py` & `reflex-0.2.4a1/reflex/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/switch.py` & `reflex-0.2.4a1/reflex/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/forms/upload.py` & `reflex-0.2.4a1/reflex/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/graphing/plotly.py` & `reflex-0.2.4a1/reflex/components/graphing/plotly.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Component for displaying a plotly graph."""
 
 from typing import Dict
 
 from plotly.graph_objects import Figure
 
-from reflex.components.component import Component
+from reflex.components.component import NoSSRComponent
 from reflex.components.tags import Tag
 from reflex.vars import Var
 
 
-class PlotlyLib(Component):
+class PlotlyLib(NoSSRComponent):
     """A component that wraps a plotly lib."""
 
     library = "react-plotly.js"
 
 
 class Plotly(PlotlyLib):
     """Display a plotly graph."""
@@ -31,22 +31,14 @@
 
     # The height of the graph.
     height: Var[str]
 
     # If true, the graph will resize when the window is resized.
     use_resize_handler: Var[bool]
 
-    def _get_imports(self):
-        return {}
-
-    def _get_custom_code(self) -> str:
-        return """import dynamic from 'next/dynamic'
-const Plot = dynamic(() => import('react-plotly.js'), { ssr: false });
-"""
-
     def _render(self) -> Tag:
         if (
             isinstance(self.data, Figure)
             and self.layout is None
             and self.width is not None
         ):
             layout = Var.create({"width": self.width, "height": self.height})
```

### Comparing `reflex-0.2.3a9/reflex/components/graphing/victory.py` & `reflex-0.2.4a1/reflex/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/__init__.py` & `reflex-0.2.4a1/reflex/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/box.py` & `reflex-0.2.4a1/reflex/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/card.py` & `reflex-0.2.4a1/reflex/components/layout/card.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/cond.py` & `reflex-0.2.4a1/reflex/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/flex.py` & `reflex-0.2.4a1/reflex/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/foreach.py` & `reflex-0.2.4a1/reflex/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/grid.py` & `reflex-0.2.4a1/reflex/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/html.py` & `reflex-0.2.4a1/reflex/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/responsive.py` & `reflex-0.2.4a1/reflex/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/stack.py` & `reflex-0.2.4a1/reflex/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/layout/wrap.py` & `reflex-0.2.4a1/reflex/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/libs/react_player.py` & `reflex-0.2.4a1/reflex/components/libs/react_player.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 """React-Player component."""
 
 from __future__ import annotations
 
-from typing import Optional
-
-from reflex.components.component import Component
-from reflex.utils import imports
+from reflex.components.component import NoSSRComponent
 from reflex.vars import Var
 
 
-class ReactPlayerComponent(Component):
+class ReactPlayerComponent(NoSSRComponent):
     """Using react-player and not implement all props and callback yet.
     reference: https://github.com/cookpete/react-player.
     """
 
-    library = "react-player"
+    library = "react-player/lazy"
 
     tag = "ReactPlayer"
 
     # The url of a video or song to play
     url: Var[str]
 
     # Set to true or false to pause or play the media
@@ -40,16 +37,7 @@
     muted: Var[bool]
 
     # Set the width of the player: ex:640px
     width: Var[str]
 
     # Set the height of the player: ex:640px
     height: Var[str]
-
-    def _get_imports(self) -> Optional[imports.ImportDict]:
-        return {}
-
-    def _get_custom_code(self) -> Optional[str]:
-        return """
-import dynamic from "next/dynamic";
-const ReactPlayer = dynamic(() => import("react-player/lazy"), { ssr: false });
-"""
```

### Comparing `reflex-0.2.3a9/reflex/components/media/avatar.py` & `reflex-0.2.4a1/reflex/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/media/icon.py` & `reflex-0.2.4a1/reflex/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/media/image.py` & `reflex-0.2.4a1/reflex/components/media/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,17 @@
 
     # "eager" | "lazy"
     loading: Var[str]
 
     # The path/url to the image or PIL image object.
     src: Var[Any]
 
+    # The alt text of the image.
+    alt: Var[str]
+
     # Provide multiple sources for an image, allowing the browser
     # to select the most appropriate source based on factors like
     # screen resolution and device capabilities.
     # Learn more _[here](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)_
     src_set: Var[str]
 
     def get_triggers(self) -> Set[str]:
```

### Comparing `reflex-0.2.3a9/reflex/components/navigation/breadcrumb.py` & `reflex-0.2.4a1/reflex/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/navigation/link.py` & `reflex-0.2.4a1/reflex/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/navigation/linkoverlay.py` & `reflex-0.2.4a1/reflex/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/navigation/stepper.py` & `reflex-0.2.4a1/reflex/components/navigation/stepper.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/__init__.py` & `reflex-0.2.4a1/reflex/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/alertdialog.py` & `reflex-0.2.4a1/reflex/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/banner.py` & `reflex-0.2.4a1/reflex/components/overlay/banner.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/drawer.py` & `reflex-0.2.4a1/reflex/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/menu.py` & `reflex-0.2.4a1/reflex/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/modal.py` & `reflex-0.2.4a1/reflex/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/popover.py` & `reflex-0.2.4a1/reflex/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/overlay/tooltip.py` & `reflex-0.2.4a1/reflex/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/tags/iter_tag.py` & `reflex-0.2.4a1/reflex/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/tags/tag.py` & `reflex-0.2.4a1/reflex/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/tags/tagless.py` & `reflex-0.2.4a1/reflex/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/typography/highlight.py` & `reflex-0.2.4a1/reflex/components/typography/highlight.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/components/typography/markdown.py` & `reflex-0.2.4a1/reflex/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/config.py` & `reflex-0.2.4a1/reflex/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,21 +257,27 @@
         if self.event_namespace:
             return f'/{self.event_namespace.strip("/")}'
 
         event_url = constants.Endpoint.EVENT.get_url()
         return urllib.parse.urlsplit(event_url).path
 
 
-def get_config() -> Config:
+def get_config(reload: bool = False) -> Config:
     """Get the app config.
 
+    Args:
+        reload: Re-import the rxconfig module from disk
+
     Returns:
         The app config.
     """
     from reflex.config import Config
 
-    sys.path.append(os.getcwd())
+    sys.path.insert(0, os.getcwd())
     try:
-        return __import__(constants.CONFIG_MODULE).config
+        rxconfig = __import__(constants.CONFIG_MODULE)
+        if reload:
+            importlib.reload(rxconfig)
+        return rxconfig.config
 
     except ImportError:
         return Config(app_name="")  # type: ignore
```

### Comparing `reflex-0.2.3a9/reflex/constants.py` & `reflex-0.2.4a1/reflex/constants.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/constants/html.py` & `reflex-0.2.4a1/reflex/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/constants/react.py` & `reflex-0.2.4a1/reflex/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/constants/reflex.py` & `reflex-0.2.4a1/reflex/el/constants/reflex.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/element.py` & `reflex-0.2.4a1/reflex/el/element.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/elements/__init__.py` & `reflex-0.2.4a1/reflex/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/el/precompile.py` & `reflex-0.2.4a1/reflex/el/precompile.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/event.py` & `reflex-0.2.4a1/reflex/event.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/middleware/hydrate_middleware.py` & `reflex-0.2.4a1/reflex/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/middleware/middleware.py` & `reflex-0.2.4a1/reflex/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/model.py` & `reflex-0.2.4a1/reflex/model.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/page.py` & `reflex-0.2.4a1/reflex/page.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/reflex.py` & `reflex-0.2.4a1/reflex/reflex.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Reflex CLI to create, run, and deploy apps."""
 
 import os
 import signal
-import threading
 from pathlib import Path
 
 import httpx
 import typer
 from alembic.util.exc import CommandError
 
 from reflex import constants, model
@@ -51,15 +50,15 @@
     name: str = typer.Option(
         None, metavar="APP_NAME", help="The name of the app to be initialized."
     ),
     template: constants.Template = typer.Option(
         constants.Template.DEFAULT, help="The template to initialize the app with."
     ),
     loglevel: constants.LogLevel = typer.Option(
-        constants.LogLevel.INFO, help="The log level to use."
+        console.LOG_LEVEL, help="The log level to use."
     ),
 ):
     """Initialize a new Reflex app in the current directory."""
     # Set the log level.
     console.set_log_level(loglevel)
 
     # Get the app name.
@@ -82,15 +81,15 @@
     else:
         telemetry.send("reinit", config.telemetry_enabled)
 
     # Initialize the .gitignore.
     prerequisites.initialize_gitignore()
 
     # Finish initializing the app.
-    console.success(f"Finished Initializing: {app_name}")
+    console.success(f"Initialized {app_name}")
 
 
 @cli.command()
 def run(
     env: constants.Env = typer.Option(
         get_config().env, help="The environment to run the app in."
     ),
@@ -98,15 +97,15 @@
         False, "--frontend-only", help="Execute only frontend."
     ),
     backend: bool = typer.Option(False, "--backend-only", help="Execute only backend."),
     frontend_port: str = typer.Option(None, help="Specify a different frontend port."),
     backend_port: str = typer.Option(None, help="Specify a different backend port."),
     backend_host: str = typer.Option(None, help="Specify the backend host."),
     loglevel: constants.LogLevel = typer.Option(
-        constants.LogLevel.INFO, help="The log level to use."
+        console.LOG_LEVEL, help="The log level to use."
     ),
 ):
     """Run the app in the current directory."""
     # Set the log level.
     console.set_log_level(loglevel)
 
     # Set ports as os env variables to take precedence over config and
@@ -163,42 +162,49 @@
             exec.run_backend_prod,
         )
     assert setup_frontend and frontend_cmd and backend_cmd, "Invalid env"
 
     # Post a telemetry event.
     telemetry.send(f"run-{env.value}", config.telemetry_enabled)
 
-    # Run the frontend and backend.
+    # Display custom message when there is a keyboard interrupt.
+    signal.signal(signal.SIGINT, processes.catch_keyboard_interrupt)
+
+    # Run the frontend and backend together.
+    commands = []
     if frontend:
         setup_frontend(Path.cwd())
-        threading.Thread(target=frontend_cmd, args=(Path.cwd(), frontend_port)).start()
+        commands.append((frontend_cmd, Path.cwd(), frontend_port))
     if backend:
-        threading.Thread(
-            target=backend_cmd,
-            args=(app.__name__, backend_host, backend_port),
-        ).start()
-
-    # Display custom message when there is a keyboard interrupt.
-    signal.signal(signal.SIGINT, processes.catch_keyboard_interrupt)
+        commands.append((backend_cmd, app.__name__, backend_host, backend_port))
+    processes.run_concurrently(*commands)
 
 
 @cli.command()
-def deploy(dry_run: bool = typer.Option(False, help="Whether to run a dry run.")):
+def deploy(
+    dry_run: bool = typer.Option(False, help="Whether to run a dry run."),
+    loglevel: constants.LogLevel = typer.Option(
+        console.LOG_LEVEL, help="The log level to use."
+    ),
+):
     """Deploy the app to the Reflex hosting service."""
+    # Set the log level.
+    console.set_log_level(loglevel)
+
     # Get the app config.
     config = get_config()
 
     # Check if the deploy url is set.
     if config.rxdeploy_url is None:
-        typer.echo("This feature is coming soon!")
+        console.info("This feature is coming soon!")
         return
 
     # Compile the app in production mode.
-    typer.echo("Compiling production app")
-    export()
+    console.info("Compiling production app")
+    export(loglevel=loglevel)
 
     # Exit early if this is a dry run.
     if dry_run:
         return
 
     # Deploy the app.
     data = {"userId": config.username, "projectId": config.app_name}
@@ -223,15 +229,15 @@
     frontend: bool = typer.Option(
         True, "--backend-only", help="Export only backend.", show_default=False
     ),
     backend: bool = typer.Option(
         True, "--frontend-only", help="Export only frontend.", show_default=False
     ),
     loglevel: constants.LogLevel = typer.Option(
-        constants.LogLevel.INFO, help="The log level to use."
+        console.LOG_LEVEL, help="The log level to use."
     ),
 ):
     """Export the app to a zip file."""
     # Set the log level.
     console.set_log_level(loglevel)
 
     # Check that the app is initialized.
```

### Comparing `reflex-0.2.3a9/reflex/route.py` & `reflex-0.2.4a1/reflex/route.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/state.py` & `reflex-0.2.4a1/reflex/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -628,17 +628,14 @@
         for prop_name in self.base_vars:
             setattr(self, prop_name, fields[prop_name].default)
 
         # Recursively reset the substates.
         for substate in self.substates.values():
             substate.reset()
 
-        # Clean the state.
-        self.clean()
-
     def get_substate(self, path: Sequence[str]) -> Optional[State]:
         """Get the substate.
 
         Args:
             path: The path to the substate.
 
         Returns:
```

### Comparing `reflex-0.2.3a9/reflex/style.py` & `reflex-0.2.4a1/reflex/style.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/testing.py` & `reflex-0.2.4a1/reflex/testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,14 +151,16 @@
                 reflex.reflex.init(
                     name=self.app_name,
                     template=reflex.constants.Template.DEFAULT,
                     loglevel=reflex.constants.LogLevel.INFO,
                 )
                 self.app_module_path.write_text(source_code)
         with chdir(self.app_path):
+            # ensure config is reloaded when testing different app
+            reflex.config.get_config(reload=True)
             self.app_module = reflex.utils.prerequisites.get_app()
         self.app_instance = self.app_module.app
 
     def _start_backend(self):
         if self.app_instance is None:
             raise RuntimeError("App was not initialized.")
         self.backend = uvicorn.Server(
@@ -281,14 +283,15 @@
         if step is None:
             step = POLL_INTERVAL
         deadline = time.time() + timeout
         while time.time() < deadline:
             success = target()
             if success:
                 return success
+            time.sleep(step)
         return False
 
     def _poll_for_servers(self, timeout: TimeoutType = None) -> socket.socket:
         """Poll backend server for listening sockets.
 
         Args:
             timeout: how long to wait for listening socket.
```

### Comparing `reflex-0.2.3a9/reflex/utils/build.py` & `reflex-0.2.4a1/reflex/utils/build.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,15 @@
 import random
 import subprocess
 from pathlib import Path
 from typing import Optional, Union
 
 from reflex import constants
 from reflex.config import get_config
-from reflex.utils import console, path_ops, prerequisites
-from reflex.utils.processes import new_process, show_progress
+from reflex.utils import console, path_ops, prerequisites, processes
 
 
 def update_json_file(file_path: str, update_dict: dict[str, Union[int, str]]):
     """Update the contents of a json file.
 
     Args:
         file_path: the path to the JSON file.
@@ -105,32 +104,32 @@
 
     # Generate the sitemap file.
     command = "export"
     if deploy_url is not None:
         generate_sitemap_config(deploy_url)
         command = "export-sitemap"
 
-    checkpoints = [
-        "Linting and checking ",
-        "Compiled successfully",
-        "Route (pages)",
-        "Collecting page data",
-        "automatically rendered as static HTML",
-        'Copying "static build" directory',
-        'Copying "public" directory',
-        "Finalizing page optimization",
-        "Export successful",
-    ]
-
-    # Start the subprocess with the progress bar.
-    process = new_process(
-        [prerequisites.get_package_manager(), "run", command],
-        cwd=constants.WEB_DIR,
-    )
-    show_progress("Creating Production Build", process, checkpoints)
+    if frontend:
+        checkpoints = [
+            "Linting and checking ",
+            "Compiled successfully",
+            "Route (pages)",
+            "Collecting page data",
+            "automatically rendered as static HTML",
+            'Copying "static build" directory',
+            'Copying "public" directory',
+            "Finalizing page optimization",
+            "Export successful",
+        ]
+        # Start the subprocess with the progress bar.
+        process = processes.new_process(
+            [prerequisites.get_package_manager(), "run", command],
+            cwd=constants.WEB_DIR,
+        )
+        processes.show_progress("Creating Production Build", process, checkpoints)
 
     # Zip up the app.
     if zip:
         if os.name == "posix":
             posix_export(backend, frontend)
         if os.name == "nt":
             nt_export(backend, frontend)
@@ -188,15 +187,15 @@
     )
 
     # Set the environment variables in client (env.json).
     set_environment_variables()
 
     # Disable the Next telemetry.
     if disable_telemetry:
-        new_process(
+        processes.new_process(
             [
                 prerequisites.get_package_manager(),
                 "run",
                 "next",
                 "telemetry",
                 "disable",
             ],
```

### Comparing `reflex-0.2.3a9/reflex/utils/console.py` & `reflex-0.2.4a1/reflex/utils/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     """Print an error message.
 
     Args:
         msg: The error message.
         kwargs: Keyword arguments to pass to the print function.
     """
     if LOG_LEVEL <= LogLevel.ERROR:
-        print(f"[red]Error: {msg}[/red]", **kwargs)
+        print(f"[red]{msg}[/red]", **kwargs)
 
 
 def ask(
     question: str, choices: Optional[List[str]] = None, default: Optional[str] = None
 ) -> str:
     """Takes a prompt question and optionally a list of choices
      and returns the user input.
```

### Comparing `reflex-0.2.3a9/reflex/utils/exec.py` & `reflex-0.2.4a1/reflex/utils/exec.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import os
 from pathlib import Path
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites, processes
-from reflex.utils.processes import new_process
 from reflex.utils.watch import AssetFolderWatch
 
 
 def start_watching_assets_folder(root):
     """Start watching assets folder.
 
     Args:
@@ -26,15 +25,15 @@
     run_command: list[str],
 ):
     """Run the process and launch the URL.
 
     Args:
         run_command: The command to run.
     """
-    process = new_process(
+    process = processes.new_process(
         run_command,
         cwd=constants.WEB_DIR,
     )
 
     if process.stdout:
         for line in process.stdout:
             if "ready started server on" in line:
@@ -74,15 +73,15 @@
         port: The port to run the frontend on.
     """
     # Set the port.
     os.environ["PORT"] = get_config().frontend_port if port is None else port
 
     # Run the frontend in production mode.
     console.rule("[bold green]App Running")
-    run_process_and_launch_url([constants.NPM_PATH, "run", "prod"])
+    run_process_and_launch_url([prerequisites.get_package_manager(), "run", "prod"])
 
 
 def run_backend(
     app_name: str,
     host: str,
     port: int,
     loglevel: constants.LogLevel = constants.LogLevel.ERROR,
@@ -91,24 +90,24 @@
 
     Args:
         host: The app host
         app_name: The app name.
         port: The app port
         loglevel: The log level.
     """
-    new_process(
+    processes.new_process(
         [
             "uvicorn",
             f"{app_name}:{constants.APP_VAR}.{constants.API_VAR}",
             "--host",
             host,
             "--port",
             str(port),
             "--log-level",
-            loglevel,
+            loglevel.value,
             "--reload",
             "--reload-dir",
             app_name.split(".")[0],
         ],
         run=True,
         show_logs=True,
     )
@@ -151,8 +150,8 @@
 
     command += [
         "--log-level",
         loglevel.value,
         "--workers",
         str(num_workers),
     ]
-    new_process(command, run=True, show_logs=True)
+    processes.new_process(command, run=True, show_logs=True)
```

### Comparing `reflex-0.2.3a9/reflex/utils/format.py` & `reflex-0.2.4a1/reflex/utils/format.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/utils/imports.py` & `reflex-0.2.4a1/reflex/utils/imports.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/utils/path_ops.py` & `reflex-0.2.4a1/reflex/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/utils/prerequisites.py` & `reflex-0.2.4a1/reflex/utils/prerequisites.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,43 +5,41 @@
 import glob
 import json
 import os
 import platform
 import re
 import sys
 import tempfile
-import threading
 from fileinput import FileInput
 from pathlib import Path
 from types import ModuleType
 from typing import Optional
 
 import httpx
 import typer
 from alembic.util.exc import CommandError
 from packaging import version
 from redis import Redis
 
 from reflex import constants, model
 from reflex.config import get_config
-from reflex.utils import console, path_ops
-from reflex.utils.processes import new_process, show_logs, show_status
+from reflex.utils import console, path_ops, processes
 
 IS_WINDOWS = platform.system() == "Windows"
 
 
 def check_node_version() -> bool:
     """Check the version of Node.js.
 
     Returns:
         Whether the version of Node.js is valid.
     """
     try:
         # Run the node -v command and capture the output.
-        result = new_process([constants.NODE_PATH, "-v"], run=True)
+        result = processes.new_process([constants.NODE_PATH, "-v"], run=True)
     except FileNotFoundError:
         return False
 
     # The output will be in the form "vX.Y.Z", but version.parse() can handle it
     current_version = version.parse(result.stdout)  # type: ignore
     # Compare the version numbers
     return (
@@ -55,15 +53,15 @@
     """Get the version of bun.
 
     Returns:
         The version of bun.
     """
     try:
         # Run the bun -v command and capture the output
-        result = new_process([constants.BUN_PATH, "-v"], run=True)
+        result = processes.new_process([constants.BUN_PATH, "-v"], run=True)
         return version.parse(result.stdout)  # type: ignore
     except FileNotFoundError:
         return None
 
 
 def get_windows_package_manager() -> str:
     """Get the package manager for windows.
@@ -164,15 +162,15 @@
     app_name = os.getcwd().split(os.path.sep)[-1].replace("-", "_")
 
     # Make sure the app is not named "reflex".
     if app_name == constants.MODULE_NAME:
         console.error(
             f"The app directory cannot be named [bold]{constants.MODULE_NAME}[/bold]."
         )
-        raise typer.Exit()
+        raise typer.Exit(1)
 
     return app_name
 
 
 def create_config(app_name: str):
     """Create a new rxconfig file.
 
@@ -273,20 +271,21 @@
 
 def initialize_node():
     """Validate nodejs have install or not."""
     if not check_node_version():
         install_node()
 
 
-def download_and_run(url: str, *args, **env):
+def download_and_run(url: str, *args, show_status: bool = False, **env):
     """Download and run a script.
 
     Args:
         url: The url of the script.
         args: The arguments to pass to the script.
+        show_status: Whether to show the status of the script.
         env: The environment variables to use.
     """
     # Download the script
     console.debug(f"Downloading {url}")
     response = httpx.get(url)
     if response.status_code != httpx.codes.OK:
         response.raise_for_status()
@@ -294,48 +293,55 @@
     # Save the script to a temporary file.
     script = tempfile.NamedTemporaryFile()
     with open(script.name, "w") as f:
         f.write(response.text)
 
     # Run the script.
     env = {**os.environ, **env}
-    process = new_process(["bash", f.name, *args], env=env)
-    show_logs(f"Installing {url}", process)
+    process = processes.new_process(["bash", f.name, *args], env=env)
+    show = processes.show_status if show_status else processes.show_logs
+    show(f"Installing {url}", process)
 
 
 def install_node():
     """Install nvm and nodejs for use by Reflex.
        Independent of any existing system installations.
 
     Raises:
         Exit: if installation failed
     """
-    # NVM is not supported on Windows.
     if IS_WINDOWS:
-        console.error(
-            f"Node.js version {constants.NODE_VERSION} or higher is required to run Reflex."
+        # See if existing node is good enough.
+        # On Windows, this must be installed manually, outside of Reflex.
+        if not check_node_version():
+            # We don't currently support auto install of node on Windows
+            # because NVM is not supported there
+            console.error(
+                f"Node.js version {constants.NODE_VERSION} or higher is required to run Reflex."
+            )
+            raise typer.Exit(1)
+        return
+    else:  # All other platforms (Linux, MacOS)
+        # TODO we can skip installation if check_node_version() checks out
+        # Create the nvm directory and install.
+        path_ops.mkdir(constants.NVM_DIR)
+        env = {**os.environ, "NVM_DIR": constants.NVM_DIR}
+        download_and_run(constants.NVM_INSTALL_URL, show_status=True, **env)
+
+        # Install node.
+        # We use bash -c as we need to source nvm.sh to use nvm.
+        process = processes.new_process(
+            [
+                "bash",
+                "-c",
+                f". {constants.NVM_DIR}/nvm.sh && nvm install {constants.NODE_VERSION}",
+            ],
+            env=env,
         )
-        raise typer.Exit()
-
-    # Create the nvm directory and install.
-    path_ops.mkdir(constants.NVM_DIR)
-    env = {**os.environ, "NVM_DIR": constants.NVM_DIR}
-    download_and_run(constants.NVM_INSTALL_URL, **env)
-
-    # Install node.
-    # We use bash -c as we need to source nvm.sh to use nvm.
-    process = new_process(
-        [
-            "bash",
-            "-c",
-            f". {constants.NVM_DIR}/nvm.sh && nvm install {constants.NODE_VERSION}",
-        ],
-        env=env,
-    )
-    show_logs("Installing node", process)
+        processes.show_status("Installing node", process)
 
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If required packages are not found.
@@ -362,56 +368,56 @@
         BUN_INSTALL=constants.BUN_ROOT_PATH,
     )
 
 
 def install_frontend_packages():
     """Installs the base and custom frontend packages."""
     # Install the base packages.
-    process = new_process(
+    process = processes.new_process(
         [get_install_package_manager(), "install", "--loglevel", "silly"],
         cwd=constants.WEB_DIR,
     )
-    show_status("Installing base frontend packages", process)
+    processes.show_status("Installing base frontend packages", process)
 
     # Install the app packages.
     packages = get_config().frontend_packages
     if len(packages) > 0:
-        process = new_process(
+        process = processes.new_process(
             [get_install_package_manager(), "add", *packages],
             cwd=constants.WEB_DIR,
         )
-        show_status("Installing custom frontend packages", process)
+        processes.show_status("Installing custom frontend packages", process)
 
 
 def check_initialized(frontend: bool = True):
     """Check that the app is initialized.
 
     Args:
         frontend: Whether to check if the frontend is initialized.
 
     Raises:
         Exit: If the app is not initialized.
     """
     has_config = os.path.exists(constants.CONFIG_FILE)
-    has_reflex_dir = IS_WINDOWS or os.path.exists(constants.REFLEX_DIR)
+    has_reflex_dir = not frontend or IS_WINDOWS or os.path.exists(constants.REFLEX_DIR)
     has_web_dir = not frontend or os.path.exists(constants.WEB_DIR)
 
     # Check if the app is initialized.
     if not (has_config and has_reflex_dir and has_web_dir):
         console.error(
             f"The app is not initialized. Run [bold]{constants.MODULE_NAME} init[/bold] first."
         )
-        raise typer.Exit()
+        raise typer.Exit(1)
 
     # Check that the template is up to date.
     if frontend and not is_latest_template():
         console.error(
             "The base app template has updated. Run [bold]reflex init[/bold] again."
         )
-        raise typer.Exit()
+        raise typer.Exit(1)
 
     # Print a warning for Windows users.
     if IS_WINDOWS:
         console.warn(
             "We strongly advise using Windows Subsystem for Linux (WSL) for optimal performance with reflex."
         )
 
@@ -428,31 +434,23 @@
         app_version = json.load(f)["version"]
     return app_version == constants.VERSION
 
 
 def initialize_frontend_dependencies():
     """Initialize all the frontend dependencies."""
     # Create the reflex directory.
-    path_ops.mkdir(constants.REFLEX_DIR)
+    if not IS_WINDOWS:
+        path_ops.mkdir(constants.REFLEX_DIR)
 
     # Install the frontend dependencies.
-    threads = [
-        threading.Thread(target=initialize_bun),
-        threading.Thread(target=initialize_node),
-    ]
-    for thread in threads:
-        thread.start()
+    processes.run_concurrently(install_node, install_bun)
 
     # Set up the web directory.
     initialize_web_directory()
 
-    # Wait for the threads to finish.
-    for thread in threads:
-        thread.join()
-
 
 def check_admin_settings():
     """Check if admin settings are set and valid for logging in cli app."""
     admin_dash = get_config().admin_dash
     if admin_dash:
         if not admin_dash.models:
             console.log(
```

### Comparing `reflex-0.2.3a9/reflex/utils/processes.py` & `reflex-0.2.4a1/reflex/utils/processes.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Process operations."""
 
 from __future__ import annotations
 
+import collections
 import contextlib
 import os
 import signal
 import subprocess
-import sys
-from typing import List, Optional
+from concurrent import futures
+from typing import Callable, List, Optional, Tuple, Union
 from urllib.parse import urlparse
 
 import psutil
+import typer
 
 from reflex import constants
 from reflex.config import get_config
 from reflex.utils import console, prerequisites
 
 
 def kill(pid):
@@ -95,14 +97,18 @@
 
     Args:
         port: The port.
         _type: The type of the port.
 
     Returns:
         The new port or the current one.
+
+
+    Raises:
+        Exit: If the user wants to exit.
     """
     console.info(
         f"Something is already running on port [bold underline]{port}[/bold underline]. This is the port the {_type} runs on."
     )
     frontend_action = console.ask("Kill or change it?", choices=["k", "c", "n"])
     if frontend_action == "k":
         kill_process_on_port(port)
@@ -116,15 +122,15 @@
         else:
             console.info(
                 f"The {_type} will run on port [bold underline]{new_port}[/bold underline]."
             )
             return new_port
     else:
         console.log("Exiting...")
-        sys.exit()
+        raise typer.Exit()
 
 
 def new_process(args, run: bool = False, show_logs: bool = False, **kwargs):
     """Wrapper over subprocess.Popen to unify the launch of child processes.
 
     Args:
         args: A string, or a sequence of program arguments.
@@ -149,41 +155,67 @@
         **kwargs,
     }
     console.debug(f"Running command: {args}")
     fn = subprocess.run if run else subprocess.Popen
     return fn(args, **kwargs)
 
 
+def run_concurrently(*fns: Union[Callable, Tuple]):
+    """Run functions concurrently in a thread pool.
+
+
+    Args:
+        *fns: The functions to run.
+    """
+    # Convert the functions to tuples.
+    fns = [fn if isinstance(fn, tuple) else (fn,) for fn in fns]  # type: ignore
+
+    # Run the functions concurrently.
+    with futures.ThreadPoolExecutor(max_workers=len(fns)) as executor:
+        # Submit the tasks.
+        tasks = [executor.submit(*fn) for fn in fns]  # type: ignore
+
+        # Get the results in the order completed to check any exceptions.
+        for task in futures.as_completed(tasks):
+            task.result()
+
+
 def stream_logs(
     message: str,
     process: subprocess.Popen,
 ):
     """Stream the logs for a process.
 
     Args:
         message: The message to display.
         process: The process.
 
     Yields:
         The lines of the process output.
+
+    Raises:
+        Exit: If the process failed.
     """
+    # Store the tail of the logs.
+    logs = collections.deque(maxlen=512)
     with process:
         console.debug(message)
         if process.stdout is None:
             return
         for line in process.stdout:
             console.debug(line, end="")
+            logs.append(line)
             yield line
 
     if process.returncode != 0:
-        console.error(f"Error during {message}")
-        console.error(
-            "Run in with [bold]--loglevel debug[/bold] to see the full error."
-        )
-        os._exit(1)
+        console.error(f"{message} failed with exit code {process.returncode}")
+        for line in logs:
+            console.error(line, end="")
+        console.error("Run with [bold]--loglevel debug [/bold] for the full log.")
+        raise typer.Exit(1)
 
 
 def show_logs(
     message: str,
     process: subprocess.Popen,
 ):
     """Show the logs for a process.
@@ -201,15 +233,15 @@
 
     Args:
         message: The initial message to display.
         process: The process.
     """
     with console.status(message) as status:
         for line in stream_logs(message, process):
-            status.update(f"{message}: {line}")
+            status.update(f"{message} {line}")
 
 
 def show_progress(message: str, process: subprocess.Popen, checkpoints: List[str]):
     """Show a progress bar for a process.
 
     Args:
         message: The message to display.
```

### Comparing `reflex-0.2.3a9/reflex/utils/telemetry.py` & `reflex-0.2.4a1/reflex/utils/telemetry.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/utils/types.py` & `reflex-0.2.4a1/reflex/utils/types.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/utils/watch.py` & `reflex-0.2.4a1/reflex/utils/watch.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/reflex/vars.py` & `reflex-0.2.4a1/reflex/vars.py`

 * *Files identical despite different names*

### Comparing `reflex-0.2.3a9/PKG-INFO` & `reflex-0.2.4a1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reflex
-Version: 0.2.3a9
+Version: 0.2.4a1
 Summary: Web apps in pure Python.
 Home-page: https://reflex.dev
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
@@ -43,78 +43,64 @@
 Description-Content-Type: text/markdown
 
 ```diff
 + Searching for Pynecone? You are in the right repo. Pynecone has been renamed to Reflex. +
 ```
 
 <div align="center">
+<img src="docs/images/reflex_dark.svg#gh-light-mode-only" alt="Reflex Logo" width="300px">
+<img src="docs/images/reflex_light.svg#gh-dark-mode-only" alt="Reflex Logo" width="300px">
 
-<img src="docs/images/reflex.png">
 <hr>
 
-# **Reflex** 
-**✨ Performant, customizable web apps in pure Python. Deploy in seconds.**
-
-📑 [Docs](https://reflex.dev/docs/getting-started/introduction) &nbsp; 📱 [Component Library](https://reflex.dev/docs/library) &nbsp; 🖼️ [Gallery](https://reflex.dev/docs/gallery) &nbsp; 🛸 [Deployment](https://reflex.dev/docs/hosting/deploy)
-
+### **✨ Performant, customizable web apps in pure Python. Deploy in seconds. ✨**
 [![PyPI version](https://badge.fury.io/py/reflex.svg)](https://badge.fury.io/py/reflex)
-![tests](https://github.com/pynecone-io/pynecone/actions/workflows/build.yml/badge.svg)
+![tests](https://github.com/pynecone-io/pynecone/actions/workflows/integration.yml/badge.svg)
 ![versions](https://img.shields.io/pypi/pyversions/reflex.svg)
+[![Documentaiton](https://img.shields.io/badge/Documentation%20-Introduction%20-%20%23007ec6)](https://reflex.dev/docs/getting-started/introduction)
 [![Discord](https://img.shields.io/discord/1029853095527727165?color=%237289da&label=Discord)](https://discord.gg/T5WSbC2YtQ)
-
 </div>
 
-### README in different language
-
 ---
-
 [English](https://github.com/reflex-dev/reflex/blob/main/README.md) | [简体中文](https://github.com/reflex-dev/reflex/blob/main/docs/zh/zh_cn/README.md) | [繁體中文](https://github.com/reflex-dev/reflex/blob/main/docs/zh/zh_tw/README.md)
-
 ---
+## ⚙️ Installation
 
-## 📦 1. Install
+Open a terminal and run (Requires Python 3.7+):
 
-Reflex requires the following to get started:
-
--   Python 3.7+
--   [Node.js 16.8.0+](https://nodejs.org/en/) (Don't worry, you won’t have to write any JavaScript!)
-
-```
+```bash
 pip install reflex
 ```
 
-## 🥳 2. Create your first app
+## 🥳 Create your first app
 
-Installing `reflex` also installs the `reflex` command line tool. Test that the install was successful by creating a new project.
+Installing `reflex` also installs the `reflex` command line tool.
 
-Replace my_app_name with your project name:
+Test that the install was successful by creating a new project. (Replace `my_app_name` with your project name):
 
-```
+```bash
 mkdir my_app_name
 cd my_app_name
 reflex init
 ```
 
-When you run this command for the first time, we will download and install [bun](https://bun.sh/) automatically.
-
-This command initializes a template app in your new directory.
-
-## 🏃 3. Run your app
+This command initializes a template app in your new directory. 
 
 You can run this app in development mode:
 
-```
+```bash
 reflex run
 ```
 
 You should see your app running at http://localhost:3000.
 
 Now you can modify the source code in `my_app_name/my_app_name.py`. Reflex has fast refreshes so you can see your changes instantly when you save your code.
 
-## 🫧 Example
+
+## 🫧 Example App
 
 Let's go over an example: creating an image generation UI around DALL·E. For simplicity, we just call the OpenAI API, but you could replace this with an ML model run locally.
 
 &nbsp;
 
 <div align="center">
 <img src="docs/images/dalle.gif" alt="A frontend wrapper for DALL·E, shown in the process of generating an image." width="550" />
@@ -173,22 +159,22 @@
             border_radius="lg",
         ),
         width="100%",
         height="100vh",
     )
 
 # Add state and page to the app.
-app = rx.App(state=State)
+app = rx.App()
 app.add_page(index, title="reflex:DALL·E")
 app.compile()
 ```
 
-Let's break this down.
+## Let's break this down.
 
-### **UI In Reflex**
+### **Reflex UI**
 
 Let's start with the UI.
 
 ```python
 def index():
     return rx.center(
         ...
@@ -236,34 +222,46 @@
 
 Within the state, we define functions called event handlers that change the state vars. Event handlers are the way that we can modify the state in Reflex. They can be called in response to user actions, such as clicking a button or typing in a text box. These actions are called events.
 
 Our DALL·E. app has an event handler, `get_image` to which get this image from the OpenAI API. Using `yield` in the middle of an event handler will cause the UI to update. Otherwise the UI will update at the end of the event handler.
 
 ### **Routing**
 
-Finally, we define our app and pass it our state.
+Finally, we define our app.
 
 ```python
-app = rx.App(state=State)
+app = rx.App()
 ```
 
-We add a route from the root of the app to the index component. We also add a title that will show up in the page preview/browser tab.
+We add a page from the root of the app to the index component. We also add a title that will show up in the page preview/browser tab.
 
 ```python
 app.add_page(index, title="DALL-E")
 app.compile()
 ```
 
-You can create a multi-page app by adding more routes.
+You can create a multi-page app by adding more pages.
+
+## 📑 Resources
+
+<div align="center">
+
+📑 [Docs](https://reflex.dev/docs/getting-started/introduction) &nbsp; |  &nbsp; 🗞️ [Blog](https://reflex.dev/blog) &nbsp; |  &nbsp; 📱 [Component Library](https://reflex.dev/docs/library) &nbsp; |  &nbsp; 🖼️ [Gallery](https://reflex.dev/docs/gallery) &nbsp; |  &nbsp; 🛸 [Deployment](https://reflex.dev/docs/hosting/deploy)  &nbsp;   
+
+</div>
+
+
+
+
 
-## Status
+## ✅ Status
 
 Reflex launched in December 2022 with the name Pynecone.
 
-As of June 2023, we are in the **Public Beta** stage.
+As of July 2023, we are in the **Public Beta** stage.
 
 -   :white_check_mark: **Public Alpha**: Anyone can install and use Reflex. There may be issues, but we are working to resolve them actively.
 -   :large_orange_diamond: **Public Beta**: Stable enough for non-enterprise use-cases.
 -   **Public Hosting Beta**: _Optionally_, deploy and host your apps on Reflex!
 -   **Public**: Reflex is production ready.
 
 Reflex has new releases and features coming every week! Make sure to :star: star and :eyes: watch this repository to stay up to date.
```

