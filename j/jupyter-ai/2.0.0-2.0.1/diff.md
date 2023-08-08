# Comparing `tmp/jupyter_ai-2.0.0.tar.gz` & `tmp/jupyter_ai-2.0.1.tar.gz`

## Comparing `jupyter_ai-2.0.0.tar` & `jupyter_ai-2.0.1.tar`

### file list

```diff
@@ -1,168 +1,168 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.eslintignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.eslintrc.js
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.prettierignore
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.prettierrc
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.stylelintrc
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/RELEASE.md
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/babel.config.js
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/conftest.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/install.json
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jest.config.js
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/package.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/project.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/setup.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/tsconfig.json
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter-config/nb-config/jupyter_ai.json
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter-config/server-config/jupyter_ai.json
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/_version.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/config_manager.py
--rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/extension.py
--rw-r--r--   0        0        0    10196 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/handlers.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/models.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/__init__.py
--rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/ask.py
--rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/base.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/clear.py
--rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/default.py
--rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/generate.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/help.py
--rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/chat_handlers/learn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/document_loaders/__init__.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/document_loaders/directory.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/document_loaders/splitter.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/package.json
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
--rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/00b26ac825e209505639.woff2
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2
--rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf
--rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf
--rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2
--rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf
--rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2
--rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff
--rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/136.8884739eec39ebcdc16d.js
--rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf
--rw-r--r--   0        0        0    26370 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/175.3ce83a66bfa8eca86e8a.js
--rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff
--rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf
--rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf
--rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff
--rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
--rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/30da91e84c893f875e25.woff
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/3398dd02302557a793f2.woff
--rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js.LICENSE.txt
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js
--rw-r--r--   0        0        0    37391 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js
--rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js
--rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf
--rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2
--rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js.LICENSE.txt
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
--rw-r--r--   0        0        0  1567983 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/598.8678074bee7747bafd9c.js
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/598.8678074bee7747bafd9c.js.LICENSE.txt
--rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2
--rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/5e28753be717dac97f55.woff
--rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/643.96795a98d50725eba5a4.js
--rw-r--r--   0        0        0    11044 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/675.756cf111884ba023580a.js
--rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2
--rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff
--rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2
--rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js
--rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf
--rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2
--rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2
--rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2
--rw-r--r--   0        0        0   467656 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js.LICENSE.txt
--rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2
--rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js
--rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/850c0af5c2238497feba.woff
--rw-r--r--   0        0        0    92966 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js.LICENSE.txt
--rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff
--rw-r--r--   0        0        0   273048 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js
--rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf
--rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff
--rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf
--rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2
--rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff
--rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff
--rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2
--rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf
--rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff
--rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2
--rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff
--rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf
--rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/c943cc986384f59e86be.woff
--rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf
--rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2
--rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff
--rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2
--rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2
--rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff
--rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2
--rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff
--rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf
--rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf
--rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff
--rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf
--rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf
--rw-r--r--   0        0        0    12202 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/remoteEntry.9e618ad3e8b43b5c8553.js
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/style.js
--rw-r--r--   0        0        0   110333 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/tests/__init__.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/jupyter_ai/tests/test_handlers.py
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/schema/plugin.json
--rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/chat_handler.ts
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/handler.ts
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/icons.ts
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/index.ts
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/selection-watcher.ts
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/theme-provider.ts
--rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/utils.ts
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/__tests__/jupyter_gai.spec.ts
--rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/chat-code-view.tsx
--rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/chat-input.tsx
--rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/chat-messages.tsx
--rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/chat-settings.tsx
--rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/chat.tsx
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/expandable-text-field.tsx
--rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/jl-theme-provider.tsx
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/scroll-container.tsx
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/select.tsx
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/components/settings/model-fields.tsx
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/contexts/collaborators-context.tsx
--rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/contexts/selection-context.tsx
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/types/mui.d.ts
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/types/svg.d.ts
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/widgets/chat-error.tsx
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/src/widgets/chat-sidebar.tsx
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/base.css
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/chat-settings.css
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/expandable-text-field.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/index.js
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/react-markdown.css
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/icons/chat.svg
--rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/style/icons/jupyternaut.svg
--rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/ui-tests/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/ui-tests/jupyter_server_test_config.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/ui-tests/package.json
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/ui-tests/playwright.config.js
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/ui-tests/tests/jupyter_ai.spec.ts
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/.gitignore
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/LICENSE
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/README.md
--rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 jupyter_ai-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.eslintignore
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.eslintrc.js
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.prettierignore
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.prettierrc
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.stylelintrc
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2116 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/RELEASE.md
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/babel.config.js
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/conftest.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/install.json
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jest.config.js
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/package.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/project.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/setup.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/tsconfig.json
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter-config/nb-config/jupyter_ai.json
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter-config/server-config/jupyter_ai.json
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/_version.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/config_manager.py
+-rw-r--r--   0        0        0     4208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/extension.py
+-rw-r--r--   0        0        0    10716 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/handlers.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/models.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/__init__.py
+-rw-r--r--   0        0        0     2299 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/ask.py
+-rw-r--r--   0        0        0     3586 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/base.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/clear.py
+-rw-r--r--   0        0        0     2756 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/default.py
+-rw-r--r--   0        0        0     9325 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/generate.py
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/help.py
+-rw-r--r--   0        0        0    10476 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/chat_handlers/learn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/document_loaders/__init__.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/document_loaders/directory.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/document_loaders/splitter.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/package.json
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json
+-rw-r--r--   0        0        0    12028 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/00b26ac825e209505639.woff2
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2
+-rw-r--r--   0        0        0    12368 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf
+-rw-r--r--   0        0        0    31308 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf
+-rw-r--r--   0        0        0    28076 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2
+-rw-r--r--   0        0        0    33580 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf
+-rw-r--r--   0        0        0    25324 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2
+-rw-r--r--   0        0        0    12316 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff
+-rw-r--r--   0        0        0    11274 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/136.4d366ce861ce9febfd0e.js
+-rw-r--r--   0        0        0    51336 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf
+-rw-r--r--   0        0        0    26369 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/175.90d6aaca4fe91c2928ea.js
+-rw-r--r--   0        0        0     7716 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff
+-rw-r--r--   0        0        0    16648 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf
+-rw-r--r--   0        0        0    19572 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf
+-rw-r--r--   0        0        0    24504 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff
+-rw-r--r--   0        0        0     9738 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js
+-rw-r--r--   0        0        0    33516 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/30da91e84c893f875e25.woff
+-rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/3398dd02302557a793f2.woff
+-rw-r--r--   0        0        0    41949 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js.LICENSE.txt
+-rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js
+-rw-r--r--   0        0        0    37391 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js
+-rw-r--r--   0        0        0    22364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js
+-rw-r--r--   0        0        0     7588 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf
+-rw-r--r--   0        0        0    11316 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js.LICENSE.txt
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/560.2fa7b4ae7a0d43e8eb1f.js
+-rw-r--r--   0        0        0  1567983 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js.LICENSE.txt
+-rw-r--r--   0        0        0     6908 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2
+-rw-r--r--   0        0        0    13208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/5e28753be717dac97f55.woff
+-rw-r--r--   0        0        0     5582 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/643.96795a98d50725eba5a4.js
+-rw-r--r--   0        0        0    11044 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/675.756cf111884ba023580a.js
+-rw-r--r--   0        0        0    63632 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf
+-rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2
+-rw-r--r--   0        0        0    21811 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js
+-rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff
+-rw-r--r--   0        0        0     5468 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2
+-rw-r--r--   0        0        0     9787 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js
+-rw-r--r--   0        0        0    32968 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf
+-rw-r--r--   0        0        0    13568 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2
+-rw-r--r--   0        0        0     3624 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2
+-rw-r--r--   0        0        0    11348 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2
+-rw-r--r--   0        0        0   467656 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js.LICENSE.txt
+-rw-r--r--   0        0        0    16440 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2
+-rw-r--r--   0        0        0     3848 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js
+-rw-r--r--   0        0        0    18668 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/850c0af5c2238497feba.woff
+-rw-r--r--   0        0        0    92966 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js.LICENSE.txt
+-rw-r--r--   0        0        0    18748 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff
+-rw-r--r--   0        0        0   273048 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js
+-rw-r--r--   0        0        0    19584 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf
+-rw-r--r--   0        0        0    14112 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff
+-rw-r--r--   0        0        0    12228 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf
+-rw-r--r--   0        0        0    16988 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2
+-rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2
+-rw-r--r--   0        0        0     5980 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff
+-rw-r--r--   0        0        0    13296 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff
+-rw-r--r--   0        0        0     4928 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2
+-rw-r--r--   0        0        0    11508 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf
+-rw-r--r--   0        0        0    19412 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff
+-rw-r--r--   0        0        0    26272 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2
+-rw-r--r--   0        0        0    30772 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff
+-rw-r--r--   0        0        0    10364 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf
+-rw-r--r--   0        0        0    29912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/c943cc986384f59e86be.woff
+-rw-r--r--   0        0        0    53580 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf
+-rw-r--r--   0        0        0     5208 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2
+-rw-r--r--   0        0        0    10588 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff
+-rw-r--r--   0        0        0    16400 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2
+-rw-r--r--   0        0        0     6912 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2
+-rw-r--r--   0        0        0    16028 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff
+-rw-r--r--   0        0        0    12216 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2
+-rw-r--r--   0        0        0    14408 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff
+-rw-r--r--   0        0        0    12344 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf
+-rw-r--r--   0        0        0    27556 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf
+-rw-r--r--   0        0        0    19676 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff
+-rw-r--r--   0        0        0    19436 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf
+-rw-r--r--   0        0        0    31196 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf
+-rw-r--r--   0        0        0    12194 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/remoteEntry.052677c5c981b7060dd0.js
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/style.js
+-rw-r--r--   0        0        0   110333 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/tests/__init__.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/jupyter_ai/tests/test_handlers.py
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/schema/plugin.json
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/chat_handler.ts
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/handler.ts
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/icons.ts
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/index.ts
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/selection-watcher.ts
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/theme-provider.ts
+-rw-r--r--   0        0        0     1413 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/utils.ts
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/__tests__/jupyter_gai.spec.ts
+-rw-r--r--   0        0        0     2328 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/chat-code-view.tsx
+-rw-r--r--   0        0        0     2904 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/chat-input.tsx
+-rw-r--r--   0        0        0     4430 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/chat-messages.tsx
+-rw-r--r--   0        0        0    13105 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/chat-settings.tsx
+-rw-r--r--   0        0        0     7117 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/chat.tsx
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/expandable-text-field.tsx
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/jl-theme-provider.tsx
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/scroll-container.tsx
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/select.tsx
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/components/settings/model-fields.tsx
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/contexts/collaborators-context.tsx
+-rw-r--r--   0        0        0     1311 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/contexts/selection-context.tsx
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/types/mui.d.ts
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/types/svg.d.ts
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/widgets/chat-error.tsx
+-rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/src/widgets/chat-sidebar.tsx
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/base.css
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/chat-settings.css
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/expandable-text-field.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/index.js
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/react-markdown.css
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/icons/chat.svg
+-rw-r--r--   0        0        0     2160 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/style/icons/jupyternaut.svg
+-rw-r--r--   0        0        0     3343 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/ui-tests/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/ui-tests/jupyter_server_test_config.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/ui-tests/package.json
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/ui-tests/playwright.config.js
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/ui-tests/tests/jupyter_ai.spec.ts
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/LICENSE
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/README.md
+-rw-r--r--   0        0        0     2793 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8257 2020-02-02 00:00:00.000000 jupyter_ai-2.0.1/PKG-INFO
```

### Comparing `jupyter_ai-2.0.0/.eslintrc.js` & `jupyter_ai-2.0.1/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/RELEASE.md` & `jupyter_ai-2.0.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jest.config.js` & `jupyter_ai-2.0.1/jest.config.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/package.json` & `jupyter_ai-2.0.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2.0.1'"}*

```diff
@@ -124,9 +124,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `jupyter_ai-2.0.0/tsconfig.json` & `jupyter_ai-2.0.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/config_manager.py` & `jupyter_ai-2.0.1/jupyter_ai/config_manager.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/extension.py` & `jupyter_ai-2.0.1/jupyter_ai/extension.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/handlers.py` & `jupyter_ai-2.0.1/jupyter_ai/handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -111,20 +111,31 @@
         installed, one is synthesized from the server's current shell
         environment."""
         collaborative = self.config.ServerApp.jpserver_extensions.get_value({}).get(
             "jupyter_collaboration", False
         )
 
         if collaborative:
-            return ChatUser(**asdict(self.current_user))
+            names = self.current_user.name.split(" ", maxsplit=2)
+            initials = "".join(
+                [(name.capitalize()[0] if len(name) > 0 else "") for name in names]
+            )
+            chat_user_kwargs = {
+                # set in case IdentityProvider doesn't return initials, e.g.
+                # JupyterHub (#302)
+                "initials": initials,
+                **asdict(self.current_user),
+            }
+            return ChatUser(**chat_user_kwargs)
 
         login = getpass.getuser()
+        initials = login[0].capitalize()
         return ChatUser(
             username=login,
-            initials=login[0].capitalize(),
+            initials=initials,
             name=login,
             display_name=login,
             color=None,
             avatar_url=None,
         )
 
     def generate_client_id(self):
@@ -191,15 +202,16 @@
         # handling messages from a websocket.  instead, process each message
         # as a distinct concurrent task.
         self.loop.create_task(self._route(chat_message))
 
     async def _route(self, message):
         """Method that routes an incoming message to the appropriate handler."""
         default = self.chat_handlers["default"]
-        maybe_command = message.body.split(" ", 1)[0]
+        # Split on any whitespace, either spaces or newlines
+        maybe_command = message.body.split(None, 1)[0]
         is_command = (
             message.body.startswith("/")
             and maybe_command in self.chat_handlers.keys()
             and maybe_command != "default"
         )
         command = maybe_command if is_command else "default"
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/models.py` & `jupyter_ai-2.0.1/jupyter_ai/models.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/ask.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/ask.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/base.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/base.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/clear.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/clear.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/default.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/default.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/generate.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/generate.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/help.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/help.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/chat_handlers/learn.py` & `jupyter_ai-2.0.1/jupyter_ai/chat_handlers/learn.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/document_loaders/directory.py` & `jupyter_ai-2.0.1/jupyter_ai/document_loaders/directory.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/document_loaders/splitter.py` & `jupyter_ai-2.0.1/jupyter_ai/document_loaders/splitter.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/package.json` & `jupyter_ai-2.0.1/jupyter_ai/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9745833333333334%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.052677c5c981b7060dd0.js'}}",*

 * * "'version'": "'2.0.1'"}*

```diff
@@ -62,15 +62,15 @@
         "schema/*.json",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jupyterlab/jupyter-ai",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.9e618ad3e8b43b5c8553.js",
+            "load": "static/remoteEntry.052677c5c981b7060dd0.js",
             "style": "./style"
         },
         "discovery": {
             "server": {
                 "base": {
                     "name": "jupyter_ai"
                 },
@@ -129,9 +129,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig` & `jupyter_ai-2.0.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/package.json.orig`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.975%*

 * *Differences: {"'version'": "'2.0.1'"}*

```diff
@@ -124,9 +124,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "2.0.0"
+    "version": "2.0.1"
 }
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json` & `jupyter_ai-2.0.1/jupyter_ai/labextension/schemas/@jupyter-ai/core/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/00b26ac825e209505639.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/00b26ac825e209505639.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/036d4e95149b69ff9bcc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/07d8e303ce4fc12b4bb5.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/08ce98e51b04d58945a3.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/0cdd387c9590a1a9f979.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/0d85ae7cc30f23790a7f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/0f60d1b897938ec918c8.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/11e4dc8a6471ff6d6ee5.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/136.8884739eec39ebcdc16d.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/136.4d366ce861ce9febfd0e.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -15,16 +15,16 @@
                 showSharedLinkDialog: () => L
             });
             var r = n(97930);
             const s = new r.Token("@jupyter/collaboration:IUserMenu"),
                 o = new r.Token("@jupyter/collaboration:IGlobalAwareness");
             var a = n(66029),
                 i = n(18778),
-                l = n(93172),
-                c = n(5987);
+                l = n(68833),
+                c = n(54151);
             const d = "jp-Collaborator";
             class u extends i.Panel {
                 constructor(e, t, n) {
                     super({}), this._onAwarenessChanged = () => {
                         const e = this._awareness.getStates(),
                             t = [];
                         e.forEach(((e, n) => {
@@ -248,15 +248,15 @@
                         parent: document.body
                     })]
                 });
 
             function x(e) {
                 return [m.of(e), C]
             }
-            var j = n(81580),
+            var j = n(8035),
                 A = n(84059);
             class I extends i.MenuBar.Renderer {
                 constructor(e) {
                     super(), this._user = e
                 }
                 renderItem(e) {
                     const t = this.createItemClass(e),
@@ -292,15 +292,15 @@
                 }
             }
             class P extends i.Menu {
                 constructor(e) {
                     super(e)
                 }
             }
-            var E = n(55354);
+            var E = n(48314);
             async function L({
                 translator: e
             }) {
                 const t = (null != e ? e : E.nullTranslator).load("collaboration"),
                     n = c.PageConfig.getToken(),
                     r = new URL(c.URLExt.normalize(c.PageConfig.getUrl({
                         workspace: c.PageConfig.defaultWorkspace
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/138ac28d1663b3037e9c.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/175.3ce83a66bfa8eca86e8a.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/175.90d6aaca4fe91c2928ea.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [175], {
         1175: (e, t, n) => {
             n.r(t), n.d(t, {
                 default: () => me
             });
-            var r = n(94004),
+            var r = n(8220),
                 o = n(48204),
                 l = n(66029),
                 i = n.n(l),
-                a = n(93172),
+                a = n(68833),
                 s = n(53959),
                 c = n(35048),
                 d = n(13264),
                 u = n(28504),
                 m = n(28066),
                 h = n(53626);
 
@@ -250,15 +250,15 @@
                     return null == e || e.on("change", t), () => {
                         null == e || e.off("change", t)
                     }
                 }), [e]), e ? i().createElement(M.Provider, {
                     value: n
                 }, t) : t
             }
-            var A = n(81580);
+            var A = n(8035);
             const N = new A.LabIcon({
                     name: "jupyter-ai::chat",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px">\n  <g class="jp-icon3" fill="#616161">\n    <path d="M0 0h24v24H0V0z" fill="none"/>\n    <path d="M15 4v7H5.17L4 12.17V4h11m1-2H3c-.55 0-1 .45-1 1v14l4-4h10c.55 0 1-.45 1-1V3c0-.55-.45-1-1-1zm5 4h-2v9H6v2c0 .55.45 1 1 1h11l4 4V7c0-.55-.45-1-1-1z"/>\n  </g>\n</svg>\n'
                 }),
                 R = new A.LabIcon({
                     name: "jupyter-ai::jupyternaut",
                     svgstr: '<svg viewBox="0 0 38 38" fill="none"\n    xmlns="http://www.w3.org/2000/svg">\n    <g clip-path="url(#clip0_0_2356)">\n        <rect width="38" height="38" fill="white" />\n        <circle cx="19" cy="19" r="19" fill="#F37726" />\n        <path fill-rule="evenodd" clip-rule="evenodd"\n            d="M19.9483 6.83653C20.5827 6.6205 21.0391 6.0196 21.0391 5.31212C21.0391 4.42296 20.3183 3.70215 19.4291 3.70215C18.5399 3.70215 17.8191 4.42296 17.8191 5.31212C17.8191 6.01951 18.2753 6.62033 18.9096 6.83644V8.00387H18.3702C12.0844 8.00387 6.97151 13.1171 6.97151 19.4026C6.97151 25.6885 12.0848 30.8013 18.3702 30.8013H19.7682C26.0541 30.8013 31.167 25.6881 31.167 19.4026C31.167 13.1773 26.1511 8.10183 19.9483 8.00527V6.83653ZM18.3702 29H19.7682C25.1351 29 29.4985 24.0213 29.4985 20.6545C29.4985 15.2876 25.1351 10.9242 19.7682 10.9242H18.3702C13.0034 10.9242 8.64 15.2876 8.64 20.6545C8.64 24.0213 13.0034 29 18.3702 29ZM32.8926 23.997C33.6267 23.997 33.6301 23.4847 33.6348 22.7562V22.7562V22.7562V22.7561C33.636 22.5714 33.6373 22.3728 33.6506 22.1651C33.7079 21.3027 33.7245 20.4643 33.7079 19.6759L33.7046 19.5569C33.6673 18.2251 33.661 17.999 32.3999 17.7511L32.252 17.7265L32.2535 17.776C32.2611 18.0225 32.2686 18.269 32.2686 18.515C32.2686 20.3168 31.9974 22.0628 31.4956 23.704C31.3593 24.1499 31.8389 24.5669 32.249 24.3451L32.8926 23.997ZM5.28037 23.997C4.54628 23.997 4.54296 23.4847 4.53822 22.7563C4.53702 22.5715 4.53573 22.3729 4.52241 22.1651C4.46511 21.3027 4.44849 20.4644 4.4651 19.6759L4.46846 19.557C4.50567 18.2251 4.51198 17.9991 5.77316 17.7512L5.921 17.7265L5.91949 17.776L5.91949 17.776C5.91193 18.0225 5.90438 18.269 5.90438 18.515C5.90438 20.3169 6.17557 22.0628 6.67738 23.704C6.81372 24.1499 6.33412 24.5669 5.92398 24.3451L5.28037 23.997ZM19.5225 11.9922C14.8928 11.9922 11.0449 14.9283 10.0641 18.7499C9.93031 19.2711 10.6154 19.4434 10.9411 19.0152C12.324 17.1972 14.0829 16.8622 15.6479 16.5641C17.7622 16.1614 19.5225 15.8262 19.5225 11.9922Z"\n            fill="white" />\n    </g>\n    <defs>\n        <clipPath id="clip0_0_2356">\n            <rect width="38" height="38" fill="white" />\n        </clipPath>\n    </defs>\n</svg>\n'
@@ -439,16 +439,16 @@
                         sx: {
                             maxHeight: "50%",
                             minHeight: 400
                         }
                     }
                 }), e.children))
             }
-            var O, Z, D = n(5987),
-                J = n(32790);
+            var O, Z, D = n(54151),
+                J = n(70255);
             async function V(e = "", t = {}) {
                 const n = J.ServerConnection.makeSettings(),
                     r = D.URLExt.join(n.baseUrl, "api/ai", e);
                 let o;
                 try {
                     o = await J.ServerConnection.makeRequest(r, t, n)
                 } catch (e) {
@@ -913,18 +913,18 @@
                 }, i().createElement(d.Z, null)) : i().createElement(s.Z, null)), t === te.Chat && i().createElement(ee, {
                     chatHandler: e.chatHandler,
                     setChatView: n
                 }), t === te.Settings && i().createElement(Y, null)))))
             }! function(e) {
                 e[e.Chat = 0] = "Chat", e[e.Settings = 1] = "Settings"
             }(te || (te = {}));
-            var re = n(91696),
-                oe = n(36408),
-                le = n(37785),
-                ie = n(17861),
+            var re = n(63150),
+                oe = n(14745),
+                le = n(56041),
+                ie = n(14543),
                 ae = n(96697),
                 se = n(74901);
 
             function ce(e) {
                 var t;
                 if (!(e instanceof re.DocumentWidget)) return null;
                 let n;
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/1ae6bd7475590e97e7f1.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/1c67f068fea8bb09bf09.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/1e6f9579e90e2cac37f8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/1ece03f79f95277d57dc.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/2014c523c3210bcc1666.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/296.c1fab29ee6698d164796.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/30da91e84c893f875e25.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/30da91e84c893f875e25.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/3398dd02302557a793f2.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/3398dd02302557a793f2.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/341.0605e2406474f3489b51.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/342.133afdc0cac64ea6f3b3.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/380.1d8633fd1460b6a300c6.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/3931dd81faed86ba021b.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/397.d17905aa3243f76edf83.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/500e04d54f0d51666332.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/51814d270d06ff0255db.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/527.fbb5737cced749a84de3.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/598.8678074bee7747bafd9c.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/598.4f92e467887ba95a5a14.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 598.8678074bee7747bafd9c.js.LICENSE.txt */
+/*! For license information please see 598.4f92e467887ba95a5a14.js.LICENSE.txt */
 (self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || []).push([
     [598], {
         73989: (e, t, n) => {
             "use strict";
 
             function a(e) {
                 if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
@@ -10128,15 +10128,15 @@
                     }, a, t, {
                         begin: "[*!#%]",
                         relevance: 0
                     }, r]
                 }
             }
         },
-        43970: e => {
+        17861: e => {
             e.exports = function(e) {
                 const t = {
                         $pattern: /\.?\w+/,
                         keyword: "abstract add and array as asc aspect assembly async begin break block by case class concat const copy constructor continue create default delegate desc distinct div do downto dynamic each else empty end ensure enum equals event except exit extension external false final finalize finalizer finally flags for forward from function future global group has if implementation implements implies in index inherited inline interface into invariants is iterator join locked locking loop matching method mod module namespace nested new nil not notify nullable of old on operator or order out override parallel params partial pinned private procedure property protected public queryable raise read readonly record reintroduce remove repeat require result reverse sealed select self sequence set shl shr skip static step soft take then to true try tuple type union unit unsafe until uses using var virtual raises volatile where while with write xor yield await mapped deprecated stdcall cdecl pascal register safecall overload library platform reference packed strict published autoreleasepool selector strong weak unretained"
                     },
                     n = e.COMMENT(/\{/, /\}/, {
                         relevance: 0
@@ -15082,15 +15082,15 @@
                 var t = "string" == typeof e ? e.charCodeAt(0) : e;
                 return t >= 97 && t <= 102 || t >= 65 && t <= 70 || t >= 48 && t <= 57
             }
         },
         496: (e, t, n) => {
             "use strict";
             var a = n(47190);
-            e.exports = a, a.registerLanguage("1c", n(7075)), a.registerLanguage("abnf", n(64855)), a.registerLanguage("accesslog", n(31139)), a.registerLanguage("actionscript", n(74257)), a.registerLanguage("ada", n(84511)), a.registerLanguage("angelscript", n(10634)), a.registerLanguage("apache", n(43475)), a.registerLanguage("applescript", n(45019)), a.registerLanguage("arcade", n(93801)), a.registerLanguage("arduino", n(75269)), a.registerLanguage("armasm", n(27945)), a.registerLanguage("xml", n(74594)), a.registerLanguage("asciidoc", n(86322)), a.registerLanguage("aspectj", n(45153)), a.registerLanguage("autohotkey", n(85999)), a.registerLanguage("autoit", n(8602)), a.registerLanguage("avrasm", n(17891)), a.registerLanguage("awk", n(88689)), a.registerLanguage("axapta", n(10517)), a.registerLanguage("bash", n(82511)), a.registerLanguage("basic", n(16770)), a.registerLanguage("bnf", n(53053)), a.registerLanguage("brainfuck", n(14842)), a.registerLanguage("c-like", n(92901)), a.registerLanguage("c", n(74483)), a.registerLanguage("cal", n(46144)), a.registerLanguage("capnproto", n(39750)), a.registerLanguage("ceylon", n(54774)), a.registerLanguage("clean", n(23114)), a.registerLanguage("clojure", n(22508)), a.registerLanguage("clojure-repl", n(52314)), a.registerLanguage("cmake", n(3159)), a.registerLanguage("coffeescript", n(50871)), a.registerLanguage("coq", n(65706)), a.registerLanguage("cos", n(94361)), a.registerLanguage("cpp", n(52216)), a.registerLanguage("crmsh", n(9565)), a.registerLanguage("crystal", n(21300)), a.registerLanguage("csharp", n(16914)), a.registerLanguage("csp", n(83463)), a.registerLanguage("css", n(402)), a.registerLanguage("d", n(1352)), a.registerLanguage("markdown", n(17203)), a.registerLanguage("dart", n(44288)), a.registerLanguage("delphi", n(54599)), a.registerLanguage("diff", n(66158)), a.registerLanguage("django", n(45004)), a.registerLanguage("dns", n(67923)), a.registerLanguage("dockerfile", n(13080)), a.registerLanguage("dos", n(74445)), a.registerLanguage("dsconfig", n(76145)), a.registerLanguage("dts", n(79545)), a.registerLanguage("dust", n(19047)), a.registerLanguage("ebnf", n(33882)), a.registerLanguage("elixir", n(17648)), a.registerLanguage("elm", n(67375)), a.registerLanguage("ruby", n(79535)), a.registerLanguage("erb", n(27855)), a.registerLanguage("erlang-repl", n(24408)), a.registerLanguage("erlang", n(77473)), a.registerLanguage("excel", n(86784)), a.registerLanguage("fix", n(33561)), a.registerLanguage("flix", n(67327)), a.registerLanguage("fortran", n(38952)), a.registerLanguage("fsharp", n(54694)), a.registerLanguage("gams", n(56506)), a.registerLanguage("gauss", n(252)), a.registerLanguage("gcode", n(76187)), a.registerLanguage("gherkin", n(85442)), a.registerLanguage("glsl", n(72643)), a.registerLanguage("gml", n(72487)), a.registerLanguage("go", n(75818)), a.registerLanguage("golo", n(49718)), a.registerLanguage("gradle", n(98630)), a.registerLanguage("groovy", n(4822)), a.registerLanguage("haml", n(9547)), a.registerLanguage("handlebars", n(51247)), a.registerLanguage("haskell", n(28308)), a.registerLanguage("haxe", n(62338)), a.registerLanguage("hsp", n(52573)), a.registerLanguage("htmlbars", n(11022)), a.registerLanguage("http", n(94628)), a.registerLanguage("hy", n(17488)), a.registerLanguage("inform7", n(90541)), a.registerLanguage("ini", n(42937)), a.registerLanguage("irpf90", n(10026)), a.registerLanguage("isbl", n(42158)), a.registerLanguage("java", n(27381)), a.registerLanguage("javascript", n(23755)), a.registerLanguage("jboss-cli", n(24461)), a.registerLanguage("json", n(99247)), a.registerLanguage("julia", n(89328)), a.registerLanguage("julia-repl", n(2528)), a.registerLanguage("kotlin", n(25962)), a.registerLanguage("lasso", n(14243)), a.registerLanguage("latex", n(15599)), a.registerLanguage("ldif", n(33525)), a.registerLanguage("leaf", n(73287)), a.registerLanguage("less", n(99126)), a.registerLanguage("lisp", n(32807)), a.registerLanguage("livecodeserver", n(85630)), a.registerLanguage("livescript", n(92975)), a.registerLanguage("llvm", n(13797)), a.registerLanguage("lsl", n(38483)), a.registerLanguage("lua", n(49570)), a.registerLanguage("makefile", n(1910)), a.registerLanguage("mathematica", n(45407)), a.registerLanguage("matlab", n(21873)), a.registerLanguage("maxima", n(62985)), a.registerLanguage("mel", n(56885)), a.registerLanguage("mercury", n(41233)), a.registerLanguage("mipsasm", n(79402)), a.registerLanguage("mizar", n(8550)), a.registerLanguage("perl", n(21602)), a.registerLanguage("mojolicious", n(25544)), a.registerLanguage("monkey", n(57741)), a.registerLanguage("moonscript", n(10910)), a.registerLanguage("n1ql", n(2122)), a.registerLanguage("nginx", n(15901)), a.registerLanguage("nim", n(62619)), a.registerLanguage("nix", n(15182)), a.registerLanguage("node-repl", n(16965)), a.registerLanguage("nsis", n(47062)), a.registerLanguage("objectivec", n(61387)), a.registerLanguage("ocaml", n(31280)), a.registerLanguage("openscad", n(31871)), a.registerLanguage("oxygene", n(43970)), a.registerLanguage("parser3", n(3650)), a.registerLanguage("pf", n(62973)), a.registerLanguage("pgsql", n(95657)), a.registerLanguage("php", n(38171)), a.registerLanguage("php-template", n(31994)), a.registerLanguage("plaintext", n(82464)), a.registerLanguage("pony", n(81632)), a.registerLanguage("powershell", n(46313)), a.registerLanguage("processing", n(80344)), a.registerLanguage("profile", n(8055)), a.registerLanguage("prolog", n(88428)), a.registerLanguage("properties", n(63820)), a.registerLanguage("protobuf", n(21944)), a.registerLanguage("puppet", n(28278)), a.registerLanguage("purebasic", n(82217)), a.registerLanguage("python", n(83443)), a.registerLanguage("python-repl", n(61966)), a.registerLanguage("q", n(20821)), a.registerLanguage("qml", n(24631)), a.registerLanguage("r", n(84020)), a.registerLanguage("reasonml", n(61277)), a.registerLanguage("rib", n(98153)), a.registerLanguage("roboconf", n(65109)), a.registerLanguage("routeros", n(96608)), a.registerLanguage("rsl", n(99315)), a.registerLanguage("ruleslanguage", n(14474)), a.registerLanguage("rust", n(26805)), a.registerLanguage("sas", n(12914)), a.registerLanguage("scala", n(6489)), a.registerLanguage("scheme", n(78854)), a.registerLanguage("scilab", n(60551)), a.registerLanguage("scss", n(18960)), a.registerLanguage("shell", n(87201)), a.registerLanguage("smali", n(81958)), a.registerLanguage("smalltalk", n(32216)), a.registerLanguage("sml", n(6067)), a.registerLanguage("sqf", n(20333)), a.registerLanguage("sql_more", n(86787)), a.registerLanguage("sql", n(4829)), a.registerLanguage("stan", n(8072)), a.registerLanguage("stata", n(71807)), a.registerLanguage("step21", n(85799)), a.registerLanguage("stylus", n(34986)), a.registerLanguage("subunit", n(50776)), a.registerLanguage("swift", n(98722)), a.registerLanguage("taggerscript", n(34407)), a.registerLanguage("yaml", n(94920)), a.registerLanguage("tap", n(86360)), a.registerLanguage("tcl", n(32112)), a.registerLanguage("thrift", n(35214)), a.registerLanguage("tp", n(43620)), a.registerLanguage("twig", n(64436)), a.registerLanguage("typescript", n(59787)), a.registerLanguage("vala", n(718)), a.registerLanguage("vbnet", n(47863)), a.registerLanguage("vbscript", n(95174)), a.registerLanguage("vbscript-html", n(34340)), a.registerLanguage("verilog", n(84888)), a.registerLanguage("vhdl", n(52636)), a.registerLanguage("vim", n(40467)), a.registerLanguage("x86asm", n(37478)), a.registerLanguage("xl", n(163)), a.registerLanguage("xquery", n(56575)), a.registerLanguage("zephir", n(28884))
+            e.exports = a, a.registerLanguage("1c", n(7075)), a.registerLanguage("abnf", n(64855)), a.registerLanguage("accesslog", n(31139)), a.registerLanguage("actionscript", n(74257)), a.registerLanguage("ada", n(84511)), a.registerLanguage("angelscript", n(10634)), a.registerLanguage("apache", n(43475)), a.registerLanguage("applescript", n(45019)), a.registerLanguage("arcade", n(93801)), a.registerLanguage("arduino", n(75269)), a.registerLanguage("armasm", n(27945)), a.registerLanguage("xml", n(74594)), a.registerLanguage("asciidoc", n(86322)), a.registerLanguage("aspectj", n(45153)), a.registerLanguage("autohotkey", n(85999)), a.registerLanguage("autoit", n(8602)), a.registerLanguage("avrasm", n(17891)), a.registerLanguage("awk", n(88689)), a.registerLanguage("axapta", n(10517)), a.registerLanguage("bash", n(82511)), a.registerLanguage("basic", n(16770)), a.registerLanguage("bnf", n(53053)), a.registerLanguage("brainfuck", n(14842)), a.registerLanguage("c-like", n(92901)), a.registerLanguage("c", n(74483)), a.registerLanguage("cal", n(46144)), a.registerLanguage("capnproto", n(39750)), a.registerLanguage("ceylon", n(54774)), a.registerLanguage("clean", n(23114)), a.registerLanguage("clojure", n(22508)), a.registerLanguage("clojure-repl", n(52314)), a.registerLanguage("cmake", n(3159)), a.registerLanguage("coffeescript", n(50871)), a.registerLanguage("coq", n(65706)), a.registerLanguage("cos", n(94361)), a.registerLanguage("cpp", n(52216)), a.registerLanguage("crmsh", n(9565)), a.registerLanguage("crystal", n(21300)), a.registerLanguage("csharp", n(16914)), a.registerLanguage("csp", n(83463)), a.registerLanguage("css", n(402)), a.registerLanguage("d", n(1352)), a.registerLanguage("markdown", n(17203)), a.registerLanguage("dart", n(44288)), a.registerLanguage("delphi", n(54599)), a.registerLanguage("diff", n(66158)), a.registerLanguage("django", n(45004)), a.registerLanguage("dns", n(67923)), a.registerLanguage("dockerfile", n(13080)), a.registerLanguage("dos", n(74445)), a.registerLanguage("dsconfig", n(76145)), a.registerLanguage("dts", n(79545)), a.registerLanguage("dust", n(19047)), a.registerLanguage("ebnf", n(33882)), a.registerLanguage("elixir", n(17648)), a.registerLanguage("elm", n(67375)), a.registerLanguage("ruby", n(79535)), a.registerLanguage("erb", n(27855)), a.registerLanguage("erlang-repl", n(24408)), a.registerLanguage("erlang", n(77473)), a.registerLanguage("excel", n(86784)), a.registerLanguage("fix", n(33561)), a.registerLanguage("flix", n(67327)), a.registerLanguage("fortran", n(38952)), a.registerLanguage("fsharp", n(54694)), a.registerLanguage("gams", n(56506)), a.registerLanguage("gauss", n(252)), a.registerLanguage("gcode", n(76187)), a.registerLanguage("gherkin", n(85442)), a.registerLanguage("glsl", n(72643)), a.registerLanguage("gml", n(72487)), a.registerLanguage("go", n(75818)), a.registerLanguage("golo", n(49718)), a.registerLanguage("gradle", n(98630)), a.registerLanguage("groovy", n(4822)), a.registerLanguage("haml", n(9547)), a.registerLanguage("handlebars", n(51247)), a.registerLanguage("haskell", n(28308)), a.registerLanguage("haxe", n(62338)), a.registerLanguage("hsp", n(52573)), a.registerLanguage("htmlbars", n(11022)), a.registerLanguage("http", n(94628)), a.registerLanguage("hy", n(17488)), a.registerLanguage("inform7", n(90541)), a.registerLanguage("ini", n(42937)), a.registerLanguage("irpf90", n(10026)), a.registerLanguage("isbl", n(42158)), a.registerLanguage("java", n(27381)), a.registerLanguage("javascript", n(23755)), a.registerLanguage("jboss-cli", n(24461)), a.registerLanguage("json", n(99247)), a.registerLanguage("julia", n(89328)), a.registerLanguage("julia-repl", n(2528)), a.registerLanguage("kotlin", n(25962)), a.registerLanguage("lasso", n(14243)), a.registerLanguage("latex", n(15599)), a.registerLanguage("ldif", n(33525)), a.registerLanguage("leaf", n(73287)), a.registerLanguage("less", n(99126)), a.registerLanguage("lisp", n(32807)), a.registerLanguage("livecodeserver", n(85630)), a.registerLanguage("livescript", n(92975)), a.registerLanguage("llvm", n(13797)), a.registerLanguage("lsl", n(38483)), a.registerLanguage("lua", n(49570)), a.registerLanguage("makefile", n(1910)), a.registerLanguage("mathematica", n(45407)), a.registerLanguage("matlab", n(21873)), a.registerLanguage("maxima", n(62985)), a.registerLanguage("mel", n(56885)), a.registerLanguage("mercury", n(41233)), a.registerLanguage("mipsasm", n(79402)), a.registerLanguage("mizar", n(8550)), a.registerLanguage("perl", n(21602)), a.registerLanguage("mojolicious", n(25544)), a.registerLanguage("monkey", n(57741)), a.registerLanguage("moonscript", n(10910)), a.registerLanguage("n1ql", n(2122)), a.registerLanguage("nginx", n(15901)), a.registerLanguage("nim", n(62619)), a.registerLanguage("nix", n(15182)), a.registerLanguage("node-repl", n(16965)), a.registerLanguage("nsis", n(47062)), a.registerLanguage("objectivec", n(61387)), a.registerLanguage("ocaml", n(31280)), a.registerLanguage("openscad", n(31871)), a.registerLanguage("oxygene", n(17861)), a.registerLanguage("parser3", n(3650)), a.registerLanguage("pf", n(62973)), a.registerLanguage("pgsql", n(95657)), a.registerLanguage("php", n(38171)), a.registerLanguage("php-template", n(31994)), a.registerLanguage("plaintext", n(82464)), a.registerLanguage("pony", n(81632)), a.registerLanguage("powershell", n(46313)), a.registerLanguage("processing", n(80344)), a.registerLanguage("profile", n(8055)), a.registerLanguage("prolog", n(88428)), a.registerLanguage("properties", n(63820)), a.registerLanguage("protobuf", n(21944)), a.registerLanguage("puppet", n(28278)), a.registerLanguage("purebasic", n(82217)), a.registerLanguage("python", n(83443)), a.registerLanguage("python-repl", n(61966)), a.registerLanguage("q", n(20821)), a.registerLanguage("qml", n(24631)), a.registerLanguage("r", n(84020)), a.registerLanguage("reasonml", n(61277)), a.registerLanguage("rib", n(98153)), a.registerLanguage("roboconf", n(65109)), a.registerLanguage("routeros", n(96608)), a.registerLanguage("rsl", n(99315)), a.registerLanguage("ruleslanguage", n(14474)), a.registerLanguage("rust", n(26805)), a.registerLanguage("sas", n(12914)), a.registerLanguage("scala", n(6489)), a.registerLanguage("scheme", n(78854)), a.registerLanguage("scilab", n(60551)), a.registerLanguage("scss", n(18960)), a.registerLanguage("shell", n(87201)), a.registerLanguage("smali", n(81958)), a.registerLanguage("smalltalk", n(32216)), a.registerLanguage("sml", n(6067)), a.registerLanguage("sqf", n(20333)), a.registerLanguage("sql_more", n(86787)), a.registerLanguage("sql", n(4829)), a.registerLanguage("stan", n(8072)), a.registerLanguage("stata", n(71807)), a.registerLanguage("step21", n(85799)), a.registerLanguage("stylus", n(34986)), a.registerLanguage("subunit", n(50776)), a.registerLanguage("swift", n(98722)), a.registerLanguage("taggerscript", n(34407)), a.registerLanguage("yaml", n(94920)), a.registerLanguage("tap", n(86360)), a.registerLanguage("tcl", n(32112)), a.registerLanguage("thrift", n(35214)), a.registerLanguage("tp", n(43620)), a.registerLanguage("twig", n(64436)), a.registerLanguage("typescript", n(59787)), a.registerLanguage("vala", n(718)), a.registerLanguage("vbnet", n(47863)), a.registerLanguage("vbscript", n(95174)), a.registerLanguage("vbscript-html", n(34340)), a.registerLanguage("verilog", n(84888)), a.registerLanguage("vhdl", n(52636)), a.registerLanguage("vim", n(40467)), a.registerLanguage("x86asm", n(37478)), a.registerLanguage("xl", n(163)), a.registerLanguage("xquery", n(56575)), a.registerLanguage("zephir", n(28884))
         },
         47190: (e, t, n) => {
             "use strict";
             var a = n(71978),
                 r = n(41536);
             t.highlight = o, t.highlightAuto = function(e, t) {
                 var n, s, l, c, d = t || {},
@@ -16498,15 +16498,15 @@
                         ocaml: $("ocaml", (function() {
                             return Promise.resolve().then(n.t.bind(n, 31280, 23))
                         })),
                         openscad: $("openscad", (function() {
                             return Promise.resolve().then(n.t.bind(n, 31871, 23))
                         })),
                         oxygene: $("oxygene", (function() {
-                            return Promise.resolve().then(n.t.bind(n, 43970, 23))
+                            return Promise.resolve().then(n.t.bind(n, 17861, 23))
                         })),
                         parser3: $("parser3", (function() {
                             return Promise.resolve().then(n.t.bind(n, 3650, 23))
                         })),
                         perl: $("perl", (function() {
                             return Promise.resolve().then(n.t.bind(n, 21602, 23))
                         })),
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/5d53e70ad607c2352162.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/5e28753be717dac97f55.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/5e28753be717dac97f55.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/643.96795a98d50725eba5a4.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/643.96795a98d50725eba5a4.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/675.756cf111884ba023580a.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/675.756cf111884ba023580a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/68534840bcfdd2bffb6f.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/68e8c73ef42afd3ccec5.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/693.2c3da85cc10c904e2289.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/6ab6b62e9b62dae2c00d.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/6b47c40166b6dbe21a5d.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/703.0ff36d6afd3dad9af47a.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/70ee1f64a20f2048c219.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/71d517d67827787cfabd.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/73d591271b1604960cb1.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/74444efd593c005e3f45.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/787.e4b10d337857bc144420.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/7af58c5ec8f132a2ddde.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/819.5cf2eced87f9df904298.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/850c0af5c2238497feba.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/850c0af5c2238497feba.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/861.26d9704eaaf5fd6b5492.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/8a8d244581371912b8f3.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/900.e5afa91e5717cd8b1f97.js`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/9163df9c7122432e6495.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/91ee67500cc0129aa0ac.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/95b6d2f1a50173bfedb8.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/97479ca6cce906abc961.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/99cd42a3c072d918f2f4.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/99f9c6750b489c9462bf.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/9be7ceb88004ab8ad124.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/a4af7d414440a1c17908.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/a6b2099fb555c60e3a0d.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/a6f7ec0d846ac7ad975a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/c2342cd8b869e01752a9.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/c6368d87e8a1a3a5d337.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/c647367d1dd4e1624687.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/c76c5d696297d51b9cb1.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/c943cc986384f59e86be.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/c943cc986384f59e86be.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/d0332f52868370fd83ae.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/d04c54219f9eaec6d4d4.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/d96cdf2b3bdd4d64a8fd.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/dc47344dbb6cb5b655c8.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/de7701e42cf1f4cf0b76.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/e14fed02b1aba7ce9f5a.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/e99ae51144bf1232efcc.woff2`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/ece03cfd83e22c212cde.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/ed0b74372feefcbb9c06.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/f01f3e87d9c6a61c0c08.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/f1d6ef86f3b11a528bd5.woff`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/f36ea897e19f4a2e571d.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/f9377ab0271cda59af24.ttf`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/remoteEntry.9e618ad3e8b43b5c8553.js` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/remoteEntry.052677c5c981b7060dd0.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, o, n, i, l, f, d, u, c, s, b, p, h, m, v, y, g, j, P, w, k, _, O, S = {
+    var e, r, t, a, o, n, i, d, l, f, u, c, s, b, p, h, m, v, y, g, j, P, w, k, _, O, S = {
             22399: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(341), t.e(380), t.e(29), t.e(441), t.e(963), t.e(175)]).then((() => () => t(1175))),
-                        "./extension": () => Promise.all([t.e(341), t.e(380), t.e(29), t.e(441), t.e(963), t.e(175)]).then((() => () => t(1175))),
+                        "./index": () => Promise.all([t.e(341), t.e(380), t.e(29), t.e(557), t.e(963), t.e(175)]).then((() => () => t(1175))),
+                        "./extension": () => Promise.all([t.e(341), t.e(380), t.e(29), t.e(557), t.e(963), t.e(175)]).then((() => () => t(1175))),
                         "./style": () => t.e(643).then((() => () => t(76643)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     n = (e, r) => {
                         if (t.S) {
@@ -57,54 +57,54 @@
     }, x.d = (e, r) => {
         for (var t in r) x.o(r, t) && !x.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, x.f = {}, x.e = e => Promise.all(Object.keys(x.f).reduce(((r, t) => (x.f[t](e, r), r)), [])), x.u = e => e + "." + {
         29: "80b9383ab8d29923abb7",
-        136: "8884739eec39ebcdc16d",
-        175: "3ce83a66bfa8eca86e8a",
+        97: "ccbd53079954eddc756f",
+        136: "4d366ce861ce9febfd0e",
+        175: "90d6aaca4fe91c2928ea",
         296: "c1fab29ee6698d164796",
         341: "0605e2406474f3489b51",
         342: "133afdc0cac64ea6f3b3",
         380: "1d8633fd1460b6a300c6",
         397: "d17905aa3243f76edf83",
         407: "9450042a7a968f6bb1b2",
-        441: "9347f6eb739397b60725",
         527: "fbb5737cced749a84de3",
+        557: "c8dd843fdf49106e6ad6",
         560: "2fa7b4ae7a0d43e8eb1f",
         564: "33c26f2a6786700b29f6",
-        594: "2f263eb0838d44e04efe",
-        598: "8678074bee7747bafd9c",
+        598: "4f92e467887ba95a5a14",
         643: "96795a98d50725eba5a4",
         675: "756cf111884ba023580a",
         693: "2c3da85cc10c904e2289",
         703: "0ff36d6afd3dad9af47a",
         704: "ec24f0c6fea0adb81c6f",
         787: "e4b10d337857bc144420",
         819: "5cf2eced87f9df904298",
         861: "26d9704eaaf5fd6b5492",
         900: "e5afa91e5717cd8b1f97",
         963: "05e514b82d50ff870683"
     } [e] + ".js?v=" + {
         29: "80b9383ab8d29923abb7",
-        136: "8884739eec39ebcdc16d",
-        175: "3ce83a66bfa8eca86e8a",
+        97: "ccbd53079954eddc756f",
+        136: "4d366ce861ce9febfd0e",
+        175: "90d6aaca4fe91c2928ea",
         296: "c1fab29ee6698d164796",
         341: "0605e2406474f3489b51",
         342: "133afdc0cac64ea6f3b3",
         380: "1d8633fd1460b6a300c6",
         397: "d17905aa3243f76edf83",
         407: "9450042a7a968f6bb1b2",
-        441: "9347f6eb739397b60725",
         527: "fbb5737cced749a84de3",
+        557: "c8dd843fdf49106e6ad6",
         560: "2fa7b4ae7a0d43e8eb1f",
         564: "33c26f2a6786700b29f6",
-        594: "2f263eb0838d44e04efe",
-        598: "8678074bee7747bafd9c",
+        598: "4f92e467887ba95a5a14",
         643: "96795a98d50725eba5a4",
         675: "756cf111884ba023580a",
         693: "2c3da85cc10c904e2289",
         703: "0ff36d6afd3dad9af47a",
         704: "ec24f0c6fea0adb81c6f",
         787: "e4b10d337857bc144420",
         819: "5cf2eced87f9df904298",
@@ -117,34 +117,34 @@
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), x.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), t = {}, a = "@jupyter-ai/core:", x.l = (e, r, o, n) => {
         if (t[e]) t[e].push(r);
         else {
-            var i, l;
+            var i, d;
             if (void 0 !== o)
-                for (var f = document.getElementsByTagName("script"), d = 0; d < f.length; d++) {
-                    var u = f[d];
+                for (var l = document.getElementsByTagName("script"), f = 0; f < l.length; f++) {
+                    var u = l[f];
                     if (u.getAttribute("src") == e || u.getAttribute("data-webpack") == a + o) {
                         i = u;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
+            i || (d = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, x.nc && i.setAttribute("nonce", x.nc), i.setAttribute("data-webpack", a + o), i.src = e), t[e] = [r];
             var c = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(s);
                     var o = t[e];
                     if (delete t[e], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(a))), r) return r(a)
                 },
                 s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), d && document.head.appendChild(i)
         }
     }, x.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -156,25 +156,25 @@
             a || (a = []);
             var o = r[t];
             if (o || (o = r[t] = {}), !(a.indexOf(o) >= 0)) {
                 if (a.push(o), e[t]) return e[t];
                 x.o(x.S, t) || (x.S[t] = {});
                 var n = x.S[t],
                     i = "@jupyter-ai/core",
-                    l = (e, r, t, a) => {
+                    d = (e, r, t, a) => {
                         var o = n[e] = n[e] || {},
-                            l = o[r];
-                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (o[r] = {
+                            d = o[r];
+                        (!d || !d.loaded && (!a != !d.eager ? a : i > d.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
-                    f = [];
-                return "default" === t && (l("@emotion/react", "11.11.1", (() => Promise.all([x.e(296), x.e(527), x.e(29), x.e(342)]).then((() => () => x(26527))))), l("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(29), x.e(564), x.e(407), x.e(560)]).then((() => () => x(52675))))), l("@jupyter-ai/core", "2.0.0", (() => Promise.all([x.e(341), x.e(380), x.e(29), x.e(441), x.e(963), x.e(175)]).then((() => () => x(1175))))), l("@jupyter/collaboration", "1.0.1", (() => Promise.all([x.e(136), x.e(29), x.e(594), x.e(441)]).then((() => () => x(29136))))), l("@mui/material", "5.14.2", (() => Promise.all([x.e(296), x.e(787), x.e(341), x.e(29), x.e(564), x.e(963), x.e(704)]).then((() => () => x(34787))))), l("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(29)]).then((() => () => x(81861))))), l("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(29), x.e(397)]).then((() => () => x(95598))))), l("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), l("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
+                    l = [];
+                return "default" === t && (d("@emotion/react", "11.11.1", (() => Promise.all([x.e(296), x.e(527), x.e(29), x.e(342)]).then((() => () => x(26527))))), d("@emotion/styled", "11.11.0", (() => Promise.all([x.e(675), x.e(29), x.e(564), x.e(407), x.e(560)]).then((() => () => x(52675))))), d("@jupyter-ai/core", "2.0.1", (() => Promise.all([x.e(341), x.e(380), x.e(29), x.e(557), x.e(963), x.e(175)]).then((() => () => x(1175))))), d("@jupyter/collaboration", "1.0.1", (() => Promise.all([x.e(136), x.e(29), x.e(97), x.e(557)]).then((() => () => x(29136))))), d("@mui/material", "5.14.2", (() => Promise.all([x.e(296), x.e(787), x.e(341), x.e(29), x.e(564), x.e(963), x.e(704)]).then((() => () => x(34787))))), d("react-markdown", "8.0.7", (() => Promise.all([x.e(693), x.e(861), x.e(29)]).then((() => () => x(81861))))), d("react-syntax-highlighter", "15.5.0", (() => Promise.all([x.e(598), x.e(29), x.e(397)]).then((() => () => x(95598))))), d("rehype-katex", "6.0.3", (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))), d("remark-math", "5.1.1", (() => x.e(703).then((() => () => x(7703)))))), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         x.g.importScripts && (e = x.g.location + "");
         var r = x.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -193,140 +193,140 @@
         e = o(e), r = o(r);
         for (var t = 0;;) {
             if (t >= e.length) return t < r.length && "u" != (typeof r[t])[0];
             var a = e[t],
                 n = (typeof a)[0];
             if (t >= r.length) return "u" == n;
             var i = r[t],
-                l = (typeof i)[0];
-            if (n != l) return "o" == n && "n" == l || "s" == l || "u" == n;
+                d = (typeof i)[0];
+            if (n != d) return "o" == n && "n" == d || "s" == d || "u" == n;
             if ("o" != n && "u" != n && a != i) return a < i;
             t++
         }
     }, i = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(d = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, d);
             return t
         }
         var n = [];
         for (o = 1; o < e.length; o++) {
-            var l = e[o];
-            n.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? n.pop() + " " + n.pop() : i(l))
+            var d = e[o];
+            n.push(0 === d ? "not(" + l() + ")" : 1 === d ? "(" + l() + " || " + l() + ")" : 2 === d ? n.pop() + " " + n.pop() : i(d))
         }
-        return f();
+        return l();
 
-        function f() {
+        function l() {
             return n.pop().replace(/^\((.+)\)$/, "$1")
         }
-    }, l = (e, r) => {
+    }, d = (e, r) => {
         if (0 in e) {
             r = o(r);
             var t = e[0],
                 a = t < 0;
             a && (t = -t - 1);
-            for (var n = 0, i = 1, f = !0;; i++, n++) {
-                var d, u, c = i < e.length ? (typeof e[i])[0] : "";
-                if (n >= r.length || "o" == (u = (typeof(d = r[n]))[0])) return !f || ("u" == c ? i > t && !a : "" == c != a);
+            for (var n = 0, i = 1, l = !0;; i++, n++) {
+                var f, u, c = i < e.length ? (typeof e[i])[0] : "";
+                if (n >= r.length || "o" == (u = (typeof(f = r[n]))[0])) return !l || ("u" == c ? i > t && !a : "" == c != a);
                 if ("u" == u) {
-                    if (!f || "u" != c) return !1
-                } else if (f)
+                    if (!l || "u" != c) return !1
+                } else if (l)
                     if (c == u)
                         if (i <= t) {
-                            if (d != e[i]) return !1
+                            if (f != e[i]) return !1
                         } else {
-                            if (a ? d > e[i] : d < e[i]) return !1;
-                            d != e[i] && (f = !1)
+                            if (a ? f > e[i] : f < e[i]) return !1;
+                            f != e[i] && (l = !1)
                         }
                 else if ("s" != c && "n" != c) {
                     if (a || i <= t) return !1;
-                    f = !1, i--
+                    l = !1, i--
                 } else {
                     if (i <= t || u < c != a) return !1;
-                    f = !1
-                } else "s" != c && "n" != c && (f = !1, i--)
+                    l = !1
+                } else "s" != c && "n" != c && (l = !1, i--)
             }
         }
         var s = [],
             b = s.pop.bind(s);
         for (n = 1; n < e.length; n++) {
             var p = e[n];
-            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? l(p, r) : !b())
+            s.push(1 == p ? b() | b() : 2 == p ? b() & b() : p ? d(p, r) : !b())
         }
         return !!b()
-    }, f = (e, r) => {
+    }, l = (e, r) => {
         var t = x.S[e];
         if (!t || !x.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
-    }, d = (e, r) => {
+    }, f = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || n(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
     }, c = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(a) + ")", s = (e, r, t, a) => {
         var o = u(e, t);
-        return l(a, o) || h(c(e, t, o, a)), v(e[t][o])
+        return d(a, o) || h(c(e, t, o, a)), v(e[t][o])
     }, b = (e, r, t) => {
         var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !l(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
+        return (r = Object.keys(a).reduce(((e, r) => !d(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
     }, p = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + i(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, h = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, m = (e, r, t, a) => {
         h(p(e, r, t, a))
     }, v = e => (e.loaded = 1, e.get()), g = (y = e => function(r, t, a, o) {
         var n = x.I(r);
         return n && n.then ? n.then(e.bind(e, r, x.S[r], t, a, o)) : e(r, x.S[r], t, a, o)
-    })(((e, r, t, a) => r && x.o(r, t) ? v(d(r, t)) : a())), j = y(((e, r, t, a) => (f(e, t), v(b(r, t, a) || m(r, e, t, a) || d(r, t))))), P = y(((e, r, t, a) => (f(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
+    })(((e, r, t, a) => r && x.o(r, t) ? v(f(r, t)) : a())), j = y(((e, r, t, a) => (l(e, t), v(b(r, t, a) || m(r, e, t, a) || f(r, t))))), P = y(((e, r, t, a) => (l(e, t), s(r, 0, t, a)))), w = y(((e, r, t, a, o) => {
         var n = r && x.o(r, t) && b(r, t, a);
         return n ? v(n) : o()
     })), k = {}, _ = {
         66029: () => P("default", "react", [1, 18, 2, 0]),
-        5987: () => P("default", "@jupyterlab/coreutils", [1, 6, 0, 3]),
-        81580: () => P("default", "@jupyterlab/ui-components", [1, 4, 0, 3]),
-        93172: () => P("default", "@jupyterlab/apputils", [1, 4, 1, 3]),
+        8035: () => P("default", "@jupyterlab/ui-components", [1, 4, 0, 4]),
+        54151: () => P("default", "@jupyterlab/coreutils", [1, 6, 0, 4]),
+        68833: () => P("default", "@jupyterlab/apputils", [1, 4, 1, 4]),
         79510: () => w("default", "@emotion/react", [1, 11, 4, 1], (() => Promise.all([x.e(296), x.e(527), x.e(819)]).then((() => () => x(26527))))),
         92764: () => w("default", "@emotion/styled", [1, 11, 3, 0], (() => Promise.all([x.e(675), x.e(564), x.e(407)]).then((() => () => x(52675))))),
-        17861: () => P("default", "@jupyterlab/notebook", [1, 4, 0, 3]),
+        8220: () => P("default", "@jupyterlab/application", [1, 4, 0, 4]),
+        14543: () => P("default", "@jupyterlab/notebook", [1, 4, 0, 4]),
+        14745: () => P("default", "@jupyterlab/codemirror", [1, 4, 0, 4]),
         30535: () => w("default", "react-markdown", [1, 8, 0, 6], (() => Promise.all([x.e(693), x.e(861)]).then((() => () => x(81861))))),
-        32790: () => P("default", "@jupyterlab/services", [1, 7, 0, 3]),
         35048: () => w("default", "@mui/material", [1, 5, 11, 0], (() => Promise.all([x.e(296), x.e(787), x.e(564), x.e(704)]).then((() => () => x(34787))))),
-        36408: () => P("default", "@jupyterlab/codemirror", [1, 4, 0, 3]),
-        37785: () => P("default", "@jupyterlab/fileeditor", [1, 4, 0, 3]),
         40532: () => w("default", "rehype-katex", [1, 6, 0, 2], (() => Promise.all([x.e(693), x.e(900)]).then((() => () => x(94900))))),
-        48204: () => w("default", "@jupyter/collaboration", [1, 1], (() => Promise.all([x.e(136), x.e(594)]).then((() => () => x(29136))))),
+        48204: () => w("default", "@jupyter/collaboration", [1, 1], (() => Promise.all([x.e(136), x.e(97)]).then((() => () => x(29136))))),
         55351: () => w("default", "react-syntax-highlighter", [1, 15, 5, 0], (() => x.e(598).then((() => () => x(95598))))),
+        56041: () => P("default", "@jupyterlab/fileeditor", [1, 4, 0, 4]),
+        63150: () => j("default", "@jupyterlab/docregistry", [1, 4, 0, 4]),
+        70255: () => P("default", "@jupyterlab/services", [1, 7, 0, 4]),
         74901: () => P("default", "@lumino/signaling", [1, 2, 0, 0]),
-        91696: () => j("default", "@jupyterlab/docregistry", [1, 4, 0, 3]),
-        94004: () => P("default", "@jupyterlab/application", [1, 4, 0, 3]),
         96697: () => P("default", "@lumino/algorithm", [1, 2, 0, 0]),
         96707: () => w("default", "remark-math", [1, 5, 1, 1], (() => x.e(703).then((() => () => x(7703))))),
         17564: () => g("default", "@emotion/react", (() => Promise.all([x.e(296), x.e(527), x.e(819)]).then((() => () => x(26527))))),
         24407: () => w("default", "@emotion/react", [1, 11, 0, 0, , "rc", 0], (() => Promise.all([x.e(296), x.e(527)]).then((() => () => x(26527))))),
         18778: () => P("default", "@lumino/widgets", [1, 2, 0, 1]),
-        55354: () => P("default", "@jupyterlab/translation", [1, 4, 0, 3]),
+        48314: () => P("default", "@jupyterlab/translation", [1, 4, 0, 4]),
         66211: () => P("default", "@codemirror/view", [1, 6, 9, 6]),
         84059: () => P("default", "@lumino/virtualdom", [1, 2, 0, 0]),
         90981: () => P("default", "yjs", [1, 13, 5, 40]),
         97930: () => P("default", "@lumino/coreutils", [1, 2, 0, 0]),
         98204: () => P("default", "@codemirror/state", [1, 6, 2, 0]),
         37704: () => P("default", "react-dom", [1, 18, 2, 0])
     }, O = {
         29: [66029],
-        175: [17861, 30535, 32790, 35048, 36408, 37785, 40532, 48204, 55351, 74901, 91696, 94004, 96697, 96707],
+        97: [18778, 48314, 66211, 84059, 90981, 97930, 98204],
+        175: [8220, 14543, 14745, 30535, 35048, 40532, 48204, 55351, 56041, 63150, 70255, 74901, 96697, 96707],
         407: [24407],
-        441: [5987, 81580, 93172],
+        557: [8035, 54151, 68833],
         564: [17564],
-        594: [18778, 55354, 66211, 84059, 90981, 97930, 98204],
         704: [37704],
         963: [79510, 92764]
     }, x.f.consumes = (e, r) => {
         x.o(O, e) && O[e].forEach((e => {
             if (x.o(k, e)) return r.push(k[e]);
             var t = r => {
                     k[e] = 0, x.m[e] = t => {
@@ -350,15 +350,15 @@
         var e = {
             718: 0
         };
         x.f.j = (r, t) => {
             var a = x.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^((56|59|70)4|29|407|441|963)$/.test(r)) e[r] = 0;
+                else if (/^((40|55|9)7|29|564|704|963)$/.test(r)) e[r] = 0;
             else {
                 var o = new Promise(((t, o) => a = e[r] = [t, o]));
                 t.push(a[2] = o);
                 var n = x.p + x.u(r),
                     i = new Error;
                 x.l(n, (t => {
                     if (x.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
@@ -366,21 +366,21 @@
                             n = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + o + ": " + n + ")", i.name = "ChunkLoadError", i.type = o, i.request = n, a[1](i)
                     }
                 }), "chunk-" + r, r)
             }
         };
         var r = (r, t) => {
-                var a, o, [n, i, l] = t,
-                    f = 0;
+                var a, o, [n, i, d] = t,
+                    l = 0;
                 if (n.some((r => 0 !== e[r]))) {
                     for (a in i) x.o(i, a) && (x.m[a] = i[a]);
-                    l && l(x)
+                    d && d(x)
                 }
-                for (r && r(t); f < n.length; f++) o = n[f], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
+                for (r && r(t); l < n.length; l++) o = n[l], x.o(e, o) && e[o] && e[o][0](), e[o] = 0
             },
             t = self.webpackChunk_jupyter_ai_core = self.webpackChunk_jupyter_ai_core || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), x.nc = void 0;
     var T = x(22399);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@jupyter-ai/core"] = T
 })();
```

### Comparing `jupyter_ai-2.0.0/jupyter_ai/labextension/static/third-party-licenses.json` & `jupyter_ai-2.0.1/jupyter_ai/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/schema/plugin.json` & `jupyter_ai-2.0.1/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/chat_handler.ts` & `jupyter_ai-2.0.1/src/chat_handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/handler.ts` & `jupyter_ai-2.0.1/src/handler.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/icons.ts` & `jupyter_ai-2.0.1/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/index.ts` & `jupyter_ai-2.0.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/selection-watcher.ts` & `jupyter_ai-2.0.1/src/selection-watcher.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/theme-provider.ts` & `jupyter_ai-2.0.1/src/theme-provider.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/utils.ts` & `jupyter_ai-2.0.1/src/utils.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/chat-code-view.tsx` & `jupyter_ai-2.0.1/src/components/chat-code-view.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/chat-input.tsx` & `jupyter_ai-2.0.1/src/components/chat-input.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/chat-messages.tsx` & `jupyter_ai-2.0.1/src/components/chat-messages.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/chat-settings.tsx` & `jupyter_ai-2.0.1/src/components/chat-settings.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/chat.tsx` & `jupyter_ai-2.0.1/src/components/chat.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/expandable-text-field.tsx` & `jupyter_ai-2.0.1/src/components/expandable-text-field.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/jl-theme-provider.tsx` & `jupyter_ai-2.0.1/src/components/jl-theme-provider.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/scroll-container.tsx` & `jupyter_ai-2.0.1/src/components/scroll-container.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/select.tsx` & `jupyter_ai-2.0.1/src/components/select.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/components/settings/model-fields.tsx` & `jupyter_ai-2.0.1/src/components/settings/model-fields.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/contexts/collaborators-context.tsx` & `jupyter_ai-2.0.1/src/contexts/collaborators-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/contexts/selection-context.tsx` & `jupyter_ai-2.0.1/src/contexts/selection-context.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/widgets/chat-error.tsx` & `jupyter_ai-2.0.1/src/widgets/chat-error.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/src/widgets/chat-sidebar.tsx` & `jupyter_ai-2.0.1/src/widgets/chat-sidebar.tsx`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/style/icons/jupyternaut.svg` & `jupyter_ai-2.0.1/style/icons/jupyternaut.svg`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/ui-tests/README.md` & `jupyter_ai-2.0.1/ui-tests/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/ui-tests/jupyter_server_test_config.py` & `jupyter_ai-2.0.1/ui-tests/jupyter_server_test_config.py`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/ui-tests/tests/jupyter_ai.spec.ts` & `jupyter_ai-2.0.1/ui-tests/tests/jupyter_ai.spec.ts`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/.gitignore` & `jupyter_ai-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/LICENSE` & `jupyter_ai-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/README.md` & `jupyter_ai-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/pyproject.toml` & `jupyter_ai-2.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyter_ai-2.0.0/PKG-INFO` & `jupyter_ai-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyter_ai
-Version: 2.0.0
+Version: 2.0.1
 Summary: A generative AI extension for JupyterLab
 Project-URL: Homepage, https://github.com/jupyterlab/jupyter-ai
 Project-URL: Bug Tracker, https://github.com/jupyterlab/jupyter-ai/issues
 Project-URL: Repository, https://github.com/jupyterlab/jupyter-ai.git
 Author-email: Project Jupyter <jupyter@googlegroups.com>
 License: BSD 3-Clause License
```

