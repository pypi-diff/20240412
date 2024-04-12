# Comparing `tmp/jupyverse-0.4.2.tar.gz` & `tmp/jupyverse-0.5.0.tar.gz`

## Comparing `jupyverse-0.4.2.tar` & `jupyverse-0.5.0.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    75193 2020-02-02 00:00:00.000000 jupyverse-0.4.2/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.4.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.4.2/MANIFEST.in
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.4.2/config.yaml
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.4.2/mkdocs.yml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.4.2/pytest.ini
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.devcontainer/requirements.txt
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.github/workflows/check-release.yml
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.github/workflows/test.yml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.4.2/binder/environment.yml
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 jupyverse-0.4.2/binder/jupyter_notebook_config.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.4.2/binder/postBuild
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.4.2/binder/start
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/index.md
--rw-r--r--   0        0        0     5262 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/install.md
--rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/jupyter.svg
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/auth.md
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/contents.md
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/frontend.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/jupyterlab.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/kernels.md
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/lab.md
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/login.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/nbconvert.md
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/resource_usage.md
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/retrolab.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/terminals.md
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/plugins/yjs.md
--rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/tutorials/jupyterhub_jupyverse_deployment.md
--rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/tutorials/standalone_jupyverse_deployment.md
--rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/usage/microservices.md
--rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/usage/multi_user.md
--rw-r--r--   0        0        0     2472 2020-02-02 00:00:00.000000 jupyverse-0.4.2/docs/usage/single_user.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/COPYING.md
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/README.md
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/pyproject.toml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/__init__.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/cli.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/py.typed
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/app/__init__.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/auth/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/auth/models.py
--rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/contents/__init__.py
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/contents/models.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/frontend/__init__.py
--rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
--rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/kernels/__init__.py
--rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/kernels/models.py
--rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/lab/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/login/__init__.py
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/main/__init__.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/nbconvert/__init__.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/resource_usage/__init__.py
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/retrolab/__init__.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/terminals/__init__.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/terminals/models.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/yjs/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.4.2/jupyverse_api/jupyverse_api/yjs/models.py
--rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.4.2/notebooks/admin_users.ipynb
--rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.4.2/notebooks/admin_users.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/README.md
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/__init__.py
--rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/backends.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/config.py
--rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/db.py
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/main.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/py.typed
--rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth/fps_auth/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/MANIFEST.in
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/__init__.py
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/backend.py
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/config.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/main.py
--rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/COPYING.md
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/README.md
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/pyproject.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
--rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/README.md
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/fps_contents/__init__.py
--rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/fps_contents/fileid.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/fps_contents/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/fps_contents/py.typed
--rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/contents/fps_contents/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/MANIFEST.in
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/README.md
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/fps_frontend/__init__.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/fps_frontend/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/frontend/fps_frontend/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/MANIFEST.in
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/README.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6476 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/MANIFEST.in
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/README.md
--rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/main.py
--rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/routes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/__init__.py
--rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/connect.py
--rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/driver.py
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/message.py
--rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/paths.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_server/__init__.py
--rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_server/message.py
--rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_server/server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/MANIFEST.in
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/fps_lab/__init__.py
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/fps_lab/main.py
--rw-r--r--   0        0        0     7306 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/fps_lab/routes.py
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/lab/fps_lab/static/favicon.ico
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/COPYING.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/MANIFEST.in
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/README.md
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/main.py
--rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/routes.py
--rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/index.html
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-file.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-notebook.ico
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-terminal.ico
--rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon.ico
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/logo/github.svg
--rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/logo/logo.png
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/login/fps_login/static/style/index.css
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/README.md
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/fps_nbconvert/__init__.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/fps_nbconvert/main.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/nbconvert/fps_nbconvert/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/README.md
--rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/fps_noauth/__init__.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/fps_noauth/backends.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/fps_noauth/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/noauth/fps_noauth/py.typed
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/COPYING.md
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/README.md
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/fps_resource_usage/__init__.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/fps_resource_usage/main.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/resource_usage/fps_resource_usage/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/MANIFEST.in
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/README.md
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/fps_retrolab/__init__.py
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/fps_retrolab/main.py
--rw-r--r--   0        0        0     6382 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/retrolab/fps_retrolab/routes.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/MANIFEST.in
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/README.md
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/fps_terminals/__init__.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/fps_terminals/main.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/fps_terminals/routes.py
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/fps_terminals/server.py
--rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/terminals/fps_terminals/win_server.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/COPYING.md
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/README.md
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/fps_webdav/__init__.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/fps_webdav/config.py
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/fps_webdav/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/fps_webdav/py.typed
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/fps_webdav/routes.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/webdav/tests/test_webdav.py
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/COPYING.md
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/MANIFEST.in
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/README.md
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/pyproject.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/__init__.py
--rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/py.typed
--rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/routes.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/__init__.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/utils.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/yblob.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/yfile.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/ynotebook.py
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/yunicode.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/__init__.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/awareness.py
--rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket.py
--rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
--rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
--rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/yroom.py
--rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/ystore.py
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/yutils.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywidgets/__init__.py
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 jupyverse-0.4.2/plugins/yjs/fps_yjs/ywidgets/widgets.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/conftest.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_app.py
--rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_auth.py
--rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_contents.py
--rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_execute.py
--rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_kernels.py
--rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_server.py
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/test_settings.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/utils.py
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/data/notebook0.ipynb
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.4.2/tests/data/notebook1.ipynb
--rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.4.2/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.4.2/COPYING.md
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 jupyverse-0.4.2/README.md
--rw-r--r--   0        0        0     5401 2020-02-02 00:00:00.000000 jupyverse-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 jupyverse-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    76121 2020-02-02 00:00:00.000000 jupyverse-0.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 jupyverse-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.0/MANIFEST.in
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 jupyverse-0.5.0/config.yaml
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 jupyverse-0.5.0/mkdocs.yml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 jupyverse-0.5.0/pytest.ini
+-rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.devcontainer/requirements.txt
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.github/workflows/check-release.yml
+-rw-r--r--   0        0        0     1602 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/environment.yml
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/jupyter_notebook_config.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/postBuild
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 jupyverse-0.5.0/binder/start
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/install.md
+-rw-r--r--   0        0        0    11002 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/jupyter.svg
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/auth.md
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/contents.md
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/frontend.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/jupyterlab.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/kernels.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/lab.md
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/login.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/nbconvert.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/notebook.md
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/resource_usage.md
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/terminals.md
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/plugins/yjs.md
+-rw-r--r--   0        0        0     6551 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/tutorials/jupyterhub_jupyverse_deployment.md
+-rw-r--r--   0        0        0    11215 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/tutorials/standalone_jupyverse_deployment.md
+-rw-r--r--   0        0        0     4977 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/microservices.md
+-rw-r--r--   0        0        0     2943 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/multi_user.md
+-rw-r--r--   0        0        0     2480 2020-02-02 00:00:00.000000 jupyverse-0.5.0/docs/usage/single_user.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/COPYING.md
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/README.md
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/pyproject.toml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/__init__.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/cli.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/py.typed
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/app/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/models.py
+-rw-r--r--   0        0        0     5032 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/__init__.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/models.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/frontend/__init__.py
+-rw-r--r--   0        0        0     2164 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py
+-rw-r--r--   0        0        0     6988 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/__init__.py
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/models.py
+-rw-r--r--   0        0        0     5557 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/lab/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/login/__init__.py
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/main/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py
+-rw-r--r--   0        0        0     2151 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/notebook/__init__.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/__init__.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/models.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/models.py
+-rw-r--r--   0        0        0     4178 2020-02-02 00:00:00.000000 jupyverse-0.5.0/notebooks/admin_users.ipynb
+-rw-r--r--   0        0        0     3225 2020-02-02 00:00:00.000000 jupyverse-0.5.0/notebooks/admin_users.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/README.md
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/__init__.py
+-rw-r--r--   0        0        0    11618 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/backends.py
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/config.py
+-rw-r--r--   0        0        0     3297 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/db.py
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/main.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/py.typed
+-rw-r--r--   0        0        0     7819 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth/fps_auth/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/MANIFEST.in
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/__init__.py
+-rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/backend.py
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/config.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/main.py
+-rw-r--r--   0        0        0     7030 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/COPYING.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/README.md
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/pyproject.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/__init__.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/config.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py
+-rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/launch.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/models.py
+-rw-r--r--   0        0        0     8231 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/README.md
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/__init__.py
+-rw-r--r--   0        0        0     8568 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/fileid.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/py.typed
+-rw-r--r--   0        0        0    10064 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/contents/fps_contents/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/MANIFEST.in
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/README.md
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/__init__.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/frontend/fps_frontend/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/MANIFEST.in
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/README.md
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/MANIFEST.in
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/README.md
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/__init__.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/main.py
+-rw-r--r--   0        0        0    14142 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/routes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/__init__.py
+-rw-r--r--   0        0        0     2987 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/connect.py
+-rw-r--r--   0        0        0    12411 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/driver.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py
+-rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/message.py
+-rw-r--r--   0        0        0     2916 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/paths.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/__init__.py
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/message.py
+-rw-r--r--   0        0        0    11556 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/MANIFEST.in
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/README.md
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/__init__.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/main.py
+-rw-r--r--   0        0        0     7392 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/routes.py
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/lab/fps_lab/static/favicon.ico
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/COPYING.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/MANIFEST.in
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/__init__.py
+-rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/main.py
+-rw-r--r--   0        0        0      958 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/routes.py
+-rw-r--r--   0        0        0     3104 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/index.html
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-file.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico
+-rw-r--r--   0        0        0    32038 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon.ico
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/logo/github.svg
+-rw-r--r--   0        0        0     5922 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/logo/logo.png
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/login/fps_login/static/style/index.css
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/README.md
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/__init__.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/main.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/README.md
+-rw-r--r--   0        0        0      875 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/__init__.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/backends.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/noauth/fps_noauth/py.typed
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/MANIFEST.in
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/README.md
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/__init__.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/main.py
+-rw-r--r--   0        0        0     6222 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/notebook/fps_notebook/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/COPYING.md
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/README.md
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/__init__.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/main.py
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/routes.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/MANIFEST.in
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/README.md
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/__init__.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/main.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/routes.py
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/server.py
+-rw-r--r--   0        0        0     1877 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/terminals/fps_terminals/win_server.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/COPYING.md
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/README.md
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/__init__.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/config.py
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/py.typed
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/fps_webdav/routes.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/webdav/tests/test_webdav.py
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/COPYING.md
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/MANIFEST.in
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/README.md
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/pyproject.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/__init__.py
+-rw-r--r--   0        0        0     1030 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/py.typed
+-rw-r--r--   0        0        0    15341 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/routes.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/__init__.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/utils.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yblob.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yfile.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yunicode.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/__init__.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py
+-rw-r--r--   0        0        0     6278 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py
+-rw-r--r--   0        0        0     4517 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py
+-rw-r--r--   0        0        0     6900 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py
+-rw-r--r--   0        0        0     8547 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py
+-rw-r--r--   0        0        0    15528 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/__init__.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/widgets.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_app.py
+-rw-r--r--   0        0        0     4484 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_auth.py
+-rw-r--r--   0        0        0     2507 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_contents.py
+-rw-r--r--   0        0        0     4807 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_execute.py
+-rw-r--r--   0        0        0     3574 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_kernels.py
+-rw-r--r--   0        0        0     7219 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_server.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/utils.py
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/data/notebook0.ipynb
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 jupyverse-0.5.0/tests/data/notebook1.ipynb
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyverse-0.5.0/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 jupyverse-0.5.0/COPYING.md
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 jupyverse-0.5.0/README.md
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 jupyverse-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 jupyverse-0.5.0/PKG-INFO
```

### Comparing `jupyverse-0.4.2/.pre-commit-config.yaml` & `jupyverse-0.5.0/.pre-commit-config.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: end-of-file-fixer
       - id: check-case-conflict
       - id: check-executables-have-shebangs
       - id: requirements-txt-fixer
       - id: check-added-large-files
       - id: check-case-conflict
@@ -12,11 +12,11 @@
       - id: check-yaml
       - id: debug-statements
       - id: forbid-new-submodules
       - id: check-builtin-literals
       - id: trailing-whitespace
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.9
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `jupyverse-0.4.2/CHANGELOG.md` & `jupyverse-0.5.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 # Changes in Jupyverse {#changelog}
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 0.5.0
+
+([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.4.2...66aac71cf07cbc14c5196cc1c144b9965fec7d2c))
+
+### Merged PRs
+
+- Replace RetroLab with Notebook [#396](https://github.com/jupyter-server/jupyverse/pull/396) ([@davidbrochart](https://github.com/davidbrochart))
+- Update FastAPI-Users v13.0.0 [#395](https://github.com/jupyter-server/jupyverse/pull/395) ([@davidbrochart](https://github.com/davidbrochart))
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2024-01-02&to=2024-04-12&type=c))
+
+[@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2024-01-02..2024-04-12&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2024-01-02..2024-04-12&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 0.4.2
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.4.1...2f084c7c744bb2d2865bdad223c680eca5c8a2cb))
 
 ### Merged PRs
 
 - Update pycrdt >=0.8.2 [#379](https://github.com/jupyter-server/jupyverse/pull/379) ([@davidbrochart](https://github.com/davidbrochart))
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter-server/jupyverse/graphs/contributors?from=2023-12-18&to=2024-01-02&type=c))
 
 [@davidbrochart](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Adavidbrochart+updated%3A2023-12-18..2024-01-02&type=Issues) | [@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter-server%2Fjupyverse+involves%3Apre-commit-ci+updated%3A2023-12-18..2024-01-02&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 0.4.1
 
 ([Full Changelog](https://github.com/jupyter-server/jupyverse/compare/v0.4.0...8321cf2a280ebe5e4bb4b09571a5b11855db649a))
 
 ### Merged PRs
 
 - Make ypywidgets optional [#375](https://github.com/jupyter-server/jupyverse/pull/375) ([@davidbrochart](https://github.com/davidbrochart))
```

### Comparing `jupyverse-0.4.2/CONTRIBUTING.md` & `jupyverse-0.5.0/CONTRIBUTING.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 ```bash
 rm -rf dist; python setup.py sdist bdist_wheel
 cd plugins/auth       ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/contents   ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/lab        ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/jupyterlab ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
-cd plugins/retrolab   ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
+cd plugins/notebook   ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/kernels    ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/nbconvert  ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/terminals  ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 cd plugins/yjs        ; rm -rf dist && python setup.py sdist bdist_wheel ; cp dist/* ../../dist/ ; cd ../..
 
 twine upload dist/*
 ```
```

### Comparing `jupyverse-0.4.2/config.yaml` & `jupyverse-0.5.0/config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -23,16 +23,16 @@
     login:
       type: login
     nbconvert:
       type: nbconvert
     resource_usage:
       type: resource_usage
       track_cpu_percent: true
-    #retrolab:
-    #  type: retrolab
+    #notebook:
+    #  type: notebook
     terminals:
       type: terminals
     yjs:
       type: yjs
 
 logging:
   version: 1
```

### Comparing `jupyverse-0.4.2/mkdocs.yml` & `jupyverse-0.5.0/mkdocs.yml`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
   - tutorials/jupyterhub_jupyverse_deployment.md
 - Plugins:
   - 'auth': plugins/auth.md
   - 'contents': plugins/contents.md
   - 'frontend': plugins/frontend.md
   - 'lab': plugins/lab.md
   - 'jupyterlab': plugins/jupyterlab.md
-  - 'retrolab': plugins/retrolab.md
+  - 'notebook': plugins/notebook.md
   - 'nbconvert': plugins/nbconvert.md
   - 'login': plugins/login.md
   - 'kernels': plugins/kernels.md
   - 'terminals': plugins/terminals.md
   - 'yjs': plugins/yjs.md
   - 'resource-usage': plugins/resource_usage.md
```

### Comparing `jupyverse-0.4.2/.devcontainer/devcontainer.json` & `jupyverse-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/.github/workflows/check-release.yml` & `jupyverse-0.5.0/.github/workflows/check-release.yml`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
           pip install --upgrade pip setuptools wheel --user
       - name: Install Dependencies
         run: |
           pip install -e . --no-deps
           pip install -e jupyverse_api
           pip install -e plugins/frontend
           pip install -e plugins/jupyterlab
-          pip install -e plugins/retrolab
+          pip install -e plugins/notebook
           pip install -e plugins/contents
           pip install -e plugins/kernels
           pip install -e plugins/terminals
           pip install -e plugins/nbconvert
           pip install -e plugins/yjs
           pip install -e plugins/auth
           pip install -e plugins/noauth
```

### Comparing `jupyverse-0.4.2/.github/workflows/test.yml` & `jupyverse-0.5.0/.github/workflows/test.yml`

 * *Files 10% similar despite different names*

```diff
@@ -17,37 +17,37 @@
     name: Types
     runs-on: ubuntu-latest
     steps:
     - name: Checkout
       uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
-        python-version: '3.11'
+        python-version: '3.12'
         cache: 'pip'
     - name: Install hatch
       run: |
         python3 -m pip install --upgrade pip
         python3 -m pip install hatch
     - name: Check types
       run: |
         hatch run dev.jupyterlab-noauth:typecheck
         hatch run dev.jupyterlab-auth:typecheck
         hatch run dev.jupyterlab-auth_fief:typecheck
-        hatch run dev.retrolab-noauth:typecheck
-        hatch run dev.retrolab-auth:typecheck
-        hatch run dev.retrolab-auth_fief:typecheck
+        hatch run dev.notebook-noauth:typecheck
+        hatch run dev.notebook-auth:typecheck
+        hatch run dev.notebook-auth_fief:typecheck
 
   test:
     name: Tests
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [ '3.8', '3.9', '3.10', '3.11' ]
+        python-version: [ '3.8', '3.9', '3.10', '3.11', '3.12' ]
 
     steps:
     - name: Checkout
       uses: actions/checkout@v3
 
     - uses: actions/setup-python@v4
       with:
```

### Comparing `jupyverse-0.4.2/binder/jupyter_notebook_config.py` & `jupyverse-0.5.0/binder/jupyter_notebook_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-jupyverse_jlab_command = " ".join(
+jupyverse_jupyterlab_command = " ".join(
     [
         "jupyverse",
         "--set auth.mode=noauth",
         "--set frontend.collaborative=true",
-        "--set frontend.base_url={base_url}jupyverse-jlab/",
-        "--disable retrolab",
+        "--set frontend.base_url={base_url}jupyverse-jupyterlab/",
+        "--disable notebook",
         "--port={port}",
     ]
-    + [">jupyverse_jlab.log 2>&1"]
+    + [">jupyverse_jupyterlab.log 2>&1"]
 )
 
 
-jupyverse_rlab_command = " ".join(
+jupyverse_notebook_command = " ".join(
     [
         "jupyverse",
         "--set auth.mode=noauth",
         "--set frontend.collaborative=true",
-        "--set frontend.base_url={base_url}jupyverse-rlab/",
+        "--set frontend.base_url={base_url}jupyverse-notebook/",
         "--disable jupyterlab",
         "--port={port}",
     ]
-    + [">jupyverse_rlab.log 2>&1"]
+    + [">jupyverse_notebook.log 2>&1"]
 )
 
 
 c.ServerProxy.servers = {
-    "jupyverse-jlab": {
-        "command": ["/bin/bash", "-c", jupyverse_jlab_command],
+    "jupyverse-jupyterlab": {
+        "command": ["/bin/bash", "-c", jupyverse_jupyterlab_command],
         "timeout": 60,
         "absolute_url": False,
     },
-    "jupyverse-rlab": {
-        "command": ["/bin/bash", "-c", jupyverse_rlab_command],
+    "jupyverse-notebook": {
+        "command": ["/bin/bash", "-c", jupyverse_notebook_command],
         "timeout": 60,
         "absolute_url": False,
     },
 }
 
-c.NotebookApp.default_url = "/jupyverse-jlab"
+c.NotebookApp.default_url = "/jupyverse-jupyterlab"
 
 import logging
 
 c.NotebookApp.log_level = logging.DEBUG
```

### Comparing `jupyverse-0.4.2/docs/index.md` & `jupyverse-0.5.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/install.md` & `jupyverse-0.5.0/docs/install.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Jupyverse can be installed to run either [JupyterLab](https://jupyterlab.readthedocs.io) or [RetroLab](https://github.com/jupyterlab/retrolab).
+Jupyverse can be installed to run either [JupyterLab](https://jupyterlab.readthedocs.io) or [Jupyter Notebook](https://jupyter-notebook.readthedocs.io).
 
 ## With `pip`
 
 For the JupyterLab frontend:
 ```bash
 pip install "jupyverse[jupyterlab,auth]"
 ```
-Or for the RetroLab frontend:
+Or for the Jupyter Notebook frontend:
 ```bash
-pip install "jupyverse[retrolab,auth]"
+pip install "jupyverse[notebook,auth]"
 ```
 
 ## With `micromamba`
 
 We recommend using `micromamba` to manage [conda-forge](https://conda-forge.org) environments
 (see `micromamba`'s
 [installation instructions](https://mamba.readthedocs.io/en/latest/installation.html#micromamba)).
@@ -23,17 +23,17 @@
 ```
 Then install Jupyverse and the desired plugins.
 
 For the JupyterLab frontend:
 ```bash
 micromamba install -c conda-forge jupyverse fps-jupyterlab fps-auth
 ```
-Or for the RetroLab frontend:
+Or for the Jupyter Notebook frontend:
 ```bash
-micromamba install -c conda-forge jupyverse fps-retrolab fps-auth
+micromamba install -c conda-forge jupyverse fps-notebook fps-auth
 ```
 
 ## Development install
 
 You first need to clone the repository:
 ```bash
 git clone https://github.com/jupyter-server/jupyverse.git
@@ -65,26 +65,26 @@
                               Matrices
 ┏━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━┳━━━━━━━━━━━┓
 ┃ Name ┃ Type    ┃ Envs                     ┃ Features ┃ Scripts   ┃
 ┡━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━╇━━━━━━━━━━━┩
 │ dev  │ virtual │ dev.jupyterlab-noauth    │ test     │ lint      │
 │      │         │ dev.jupyterlab-auth      │          │ test      │
 │      │         │ dev.jupyterlab-auth_fief │          │ typecheck │
-│      │         │ dev.retrolab-noauth      │          │           │
-│      │         │ dev.retrolab-auth        │          │           │
-│      │         │ dev.retrolab-auth_fief   │          │           │
+│      │         │ dev.notebook-noauth      │          │           │
+│      │         │ dev.notebook-auth        │          │           │
+│      │         │ dev.notebook-auth_fief   │          │           │
 └──────┴─────────┴──────────────────────────┴──────────┴───────────┘
 ```
 !!! note
     The `default` environment will install all the plugins from PyPI, **not** from
     your local repository. The `dev` environment installs all plugins in editable mode
     from your local repository. So you want to use the `dev` environment.
 
 Currently, the `dev` environment matrix consists of all combinations of frontends
-(`jupyterlab`, `retrolab`) and authentication methods (`noauth`, `auth`, `auth_fief`),
+(`jupyterlab`, `notebook`) and authentication methods (`noauth`, `auth`, `auth_fief`),
 which leads to six environments.
 
 A number of scripts are available in the `dev` environments. They can be
 executed using `hatch run {env}:{script}`. You can also execute anything that you would
 execute in your shell. For instance, to run Jupyverse for the `jupyterlab` frontend and
 without authentication, enter:
 ```bash
```

### Comparing `jupyverse-0.4.2/docs/jupyter.svg` & `jupyverse-0.5.0/docs/jupyter.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/plugins/auth.md` & `jupyverse-0.5.0/docs/plugins/auth.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/tutorials/jupyterhub_jupyverse_deployment.md` & `jupyverse-0.5.0/docs/tutorials/jupyterhub_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/tutorials/standalone_jupyverse_deployment.md` & `jupyverse-0.5.0/docs/tutorials/standalone_jupyverse_deployment.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/usage/microservices.md` & `jupyverse-0.5.0/docs/usage/microservices.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/usage/multi_user.md` & `jupyverse-0.5.0/docs/usage/multi_user.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/docs/usage/single_user.md` & `jupyverse-0.5.0/docs/usage/single_user.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ## Token authentication
 
 This is the default mode when launching Jupyverse, just enter in a terminal:
 ```bash
 jupyverse --open-browser
 # same as: jupyverse --set auth.mode=token --open-browser
 ```
-This should open a new window in a browser, and load JupyterLab or RetroLab, depending on the front-end you chose to install (see [Install](../../install)).
+This should open a new window in a browser, and load JupyterLab or Jupyter Notebook, depending on the front-end you chose to install (see [Install](../../install)).
 
 If you look at the terminal, you should see among other things:
 ```
 [2023-04-05 16:22:39,137 INFO] To access the server, copy and paste this URL:
 [2023-04-05 16:22:39,137 INFO] http://127.0.0.1:8000/?token=69ce8ccee10d4388b00b3df0d9849700
 ```
 This is the URL the browser window was opened with, and you can see that a `token` was passed as a query parameter. When the request is made to the server, the token is checked and a cookie is set in the browser. The user is now authenticated and doesn't need to pass the token again in other requests.
```

### Comparing `jupyverse-0.4.2/jupyverse_api/COPYING.md` & `jupyverse-0.5.0/jupyverse_api/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/pyproject.toml` & `jupyverse-0.5.0/jupyverse_api/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+  "importlib_metadata >=3.6; python_version<'3.10'",
   "pydantic >=2,<3",
   "fastapi >=0.95.0,<1",
   "rich-click >=1.6.1,<2",
   "asphalt >=4.11.0,<5",
   "asphalt-web[fastapi] >=1.1.0,<2",
 ]
 dynamic = ["version"]
```

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Dict
 
 from pydantic import BaseModel
 
 from .app import App
 
-__version__ = "0.4.2"
+__version__ = "0.5.0"
 
 
 class Singleton(type):
     _instances: Dict = {}
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances:
```

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/cli.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import sys
 from typing import List, Tuple
 
-import pkg_resources
 import rich_click as click
 from asphalt.core.cli import run
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 
 @click.command()  # type: ignore
 @click.option(
     "--open-browser",
     is_flag=True,
     show_default=True,
     default=False,
@@ -68,15 +73,15 @@
         configfile=[config],
     )  # type: ignore
 
 
 def get_config(disable: Tuple[str, ...]) -> str:
     jupyverse_components = [
         ep.name
-        for ep in pkg_resources.iter_entry_points(group="jupyverse.components")
+        for ep in entry_points(group="jupyverse.components")
         if ep.name not in disable
     ]
 
     config = ["component:\n  type: jupyverse\n  components:\n"]
     for component in jupyverse_components:
         config.append(f"    {component}:\n      type: {component}\n")
```

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/app/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/app/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/auth/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/contents/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/contents/models.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/contents/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/jupyterlab/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/jupyterlab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/kernels/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/kernels/models.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/kernels/models.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/lab/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/lab/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/main/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/main/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/nbconvert/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/nbconvert/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/resource_usage/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/resource_usage/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/retrolab/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/notebook/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,48 +6,48 @@
 from jupyverse_api import Router
 
 from ..app import App
 from ..auth import Auth, User
 from ..lab import Lab
 
 
-class RetroLab(Router, ABC):
+class Notebook(Router, ABC):
     def __init__(self, app: App, auth: Auth, lab: Lab):
         super().__init__(app=app)
 
         router = APIRouter()
 
-        @router.get("/retro/tree", response_class=HTMLResponse)
+        @router.get("/tree", response_class=HTMLResponse)
         async def get_tree(
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_tree(user)
 
-        @router.get("/retro/notebooks/{path:path}", response_class=HTMLResponse)
+        @router.get("/notebooks/{path:path}", response_class=HTMLResponse)
         async def get_notebook(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_notebook(path, user)
 
-        @router.get("/retro/edit/{path:path}", response_class=HTMLResponse)
+        @router.get("/edit/{path:path}", response_class=HTMLResponse)
         async def edit_file(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.edit_file(path, user)
 
-        @router.get("/retro/consoles/{path:path}", response_class=HTMLResponse)
+        @router.get("/consoles/{path:path}", response_class=HTMLResponse)
         async def get_console(
             path,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_console(path, user)
 
-        @router.get("/retro/terminals/{name}", response_class=HTMLResponse)
+        @router.get("/terminals/{name}", response_class=HTMLResponse)
         async def get_terminal(
             name: str,
             user: User = Depends(auth.current_user()),
         ):
             return await self.get_terminal(name, user)
 
         self.include_router(router)
```

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/terminals/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/terminals/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/jupyverse_api/jupyverse_api/yjs/__init__.py` & `jupyverse-0.5.0/jupyverse_api/jupyverse_api/yjs/__init__.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/notebooks/admin_users.ipynb` & `jupyverse-0.5.0/notebooks/admin_users.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/notebooks/admin_users.py` & `jupyverse-0.5.0/notebooks/admin_users.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/COPYING.md` & `jupyverse-0.5.0/plugins/auth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/pyproject.toml` & `jupyverse-0.5.0/plugins/auth/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "fps_auth"
 description = "An FPS plugin for the authentication API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 dynamic = ["version"]
 requires-python = ">=3.8"
 dependencies = [
     "aiosqlite",
-    "fastapi-users[sqlalchemy,oauth] >=12,<13",
+    "fastapi-users[sqlalchemy,oauth] >=13.0.0,<14.0.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `jupyverse-0.4.2/plugins/auth/fps_auth/backends.py` & `jupyverse-0.5.0/plugins/auth/fps_auth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/fps_auth/config.py` & `jupyverse-0.5.0/plugins/auth/fps_auth/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/fps_auth/db.py` & `jupyverse-0.5.0/plugins/auth/fps_auth/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/fps_auth/main.py` & `jupyverse-0.5.0/plugins/auth/fps_auth/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth/fps_auth/routes.py` & `jupyverse-0.5.0/plugins/auth/fps_auth/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/COPYING.md` & `jupyverse-0.5.0/plugins/auth_fief/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/pyproject.toml` & `jupyverse-0.5.0/plugins/auth_fief/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/backend.py` & `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/backend.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/config.py` & `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/config.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/main.py` & `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_fief/fps_auth_fief/routes.py` & `jupyverse-0.5.0/plugins/auth_fief/fps_auth_fief/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_jupyterhub/COPYING.md` & `jupyverse-0.5.0/plugins/auth_jupyterhub/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_jupyterhub/pyproject.toml` & `jupyverse-0.5.0/plugins/auth_jupyterhub/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py` & `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/db.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py` & `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py` & `jupyverse-0.5.0/plugins/auth_jupyterhub/fps_auth_jupyterhub/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/contents/COPYING.md` & `jupyverse-0.5.0/plugins/contents/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/contents/pyproject.toml` & `jupyverse-0.5.0/plugins/contents/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/contents/fps_contents/fileid.py` & `jupyverse-0.5.0/plugins/contents/fps_contents/fileid.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/contents/fps_contents/routes.py` & `jupyverse-0.5.0/plugins/contents/fps_contents/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/frontend/COPYING.md` & `jupyverse-0.5.0/plugins/frontend/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/frontend/pyproject.toml` & `jupyverse-0.5.0/plugins/frontend/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/jupyterlab/COPYING.md` & `jupyverse-0.5.0/plugins/jupyterlab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/jupyterlab/pyproject.toml` & `jupyverse-0.5.0/plugins/jupyterlab/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/index.py` & `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/main.py` & `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/jupyterlab/fps_jupyterlab/routes.py` & `jupyverse-0.5.0/plugins/jupyterlab/fps_jupyterlab/routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
         self.jupyterlab_config = jupyterlab_config
         self.frontend_config = frontend_config
         self.lab = lab
         lab.redirect_after_root = "lab"
 
         extensions_dir = lab.prefix_dir / "share" / "jupyter" / "labextensions"
-        self.federated_extensions, self.disabled_extension = lab.get_federated_extensions(
+        self.federated_extensions, self.disabled_extensions = lab.get_federated_extensions(
             extensions_dir
         )
         jupyterlab_dir = Path(jupyterlab_module.__file__).parents[1]
 
         if jupyterlab_config.dev_mode:
             self.static_lab_dir = jupyterlab_dir / "dev_mode" / "static"
         else:
@@ -122,15 +122,15 @@
             "appUrl": "/lab",
             "appVersion": jupyterlab_module.__version__,
             "baseUrl": base_url,
             "cacheFiles": False,
             "collaborative": collaborative,
             "serverSideExecution": server_side_execution,
             "devMode": dev_mode,
-            "disabledExtensions": self.disabled_extension,
+            "disabledExtensions": self.disabled_extensions,
             "exposeAppInBrowser": False,
             "extraLabextensionsPath": [],
             "federated_extensions": self.federated_extensions,
             "fullAppUrl": f"{base_url}lab",
             "fullLabextensionsUrl": f"{base_url}lab/extensions",
             "fullLicensesUrl": f"{base_url}lab/api/licenses",
             "fullListingsUrl": f"{base_url}lab/api/listings",
```

### Comparing `jupyverse-0.4.2/plugins/kernels/COPYING.md` & `jupyverse-0.5.0/plugins/kernels/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/pyproject.toml` & `jupyverse-0.5.0/plugins/kernels/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/main.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/routes.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/connect.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/connect.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/driver.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/driver.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/kernelspec.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/message.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_driver/paths.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_driver/paths.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_server/message.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/message.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/kernels/fps_kernels/kernel_server/server.py` & `jupyverse-0.5.0/plugins/kernels/fps_kernels/kernel_server/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/lab/COPYING.md` & `jupyverse-0.5.0/plugins/lab/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/lab/pyproject.toml` & `jupyverse-0.5.0/plugins/lab/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
 name = "fps_lab"
-description = "An FPS plugin for the JupyterLab/RetroLab API"
+description = "An FPS plugin for the JupyterLab/Notebook API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
+  "importlib_metadata >=3.6; python_version<'3.10'",
   "babel",
   "json5",
   "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
```

### Comparing `jupyverse-0.4.2/plugins/lab/fps_lab/main.py` & `jupyverse-0.5.0/plugins/lab/fps_lab/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/lab/fps_lab/routes.py` & `jupyverse-0.5.0/plugins/lab/fps_lab/routes.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import json
 import logging
 import os
+import sys
 from glob import glob
 from http import HTTPStatus
 from pathlib import Path
 from typing import List, Optional, Tuple
 
 import json5  # type: ignore
-import pkg_resources
 from babel import Locale
 from fastapi import Response, status
 from fastapi.responses import FileResponse, RedirectResponse
 from starlette.requests import Request
 
 from jupyverse_api.app import App
 from jupyverse_api.auth import Auth, User
 from jupyverse_api.frontend import FrontendConfig
 from jupyverse_api.jupyterlab import JupyterLabConfig
 from jupyverse_api.lab import Lab
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 logger = logging.getLogger("lab")
 
 
 class _Lab(Lab):
     def __init__(
         self,
         app: App,
@@ -75,15 +80,15 @@
         native_name = (locale.get_display_name() or "").capitalize()
         data = {
             "en": {
                 "displayName": display_name,
                 "nativeName": native_name,
             }
         }
-        for ep in pkg_resources.iter_entry_points(group="jupyterlab.languagepack"):
+        for ep in entry_points(group="jupyterlab.languagepack"):
             locale = Locale.parse(ep.name)
             data[ep.name] = {
                 "displayName": display_name,
                 "nativeName": native_name,
             }
         return {"data": data, "message": ""}
 
@@ -92,15 +97,15 @@
         language,
         user: User,
     ):
         if language == "en":
             self.locale = language
             return {}
 
-        for ep in pkg_resources.iter_entry_points(group="jupyterlab.languagepack"):
+        for ep in entry_points(group="jupyterlab.languagepack"):
             if ep.name == language:
                 break
         else:
             return {"data": {}, "message": f"Language pack '{language}' not installed!"}
         self.locale = language
         package = ep.load()
         data = {}
@@ -116,15 +121,15 @@
         name0,
         name1,
         name2,
         user: User,
     ):
         with open(self.jlab_dir / "static" / "package.json") as f:
             package = json.load(f)
-        if name0 in ["@jupyterlab", "@retrolab"]:
+        if name0 in ["@jupyterlab", "@notebook"]:
             schemas_parent = self.jlab_dir
         else:
             schemas_parent = self.extensions_dir / name0 / name1
         with open(schemas_parent / "schemas" / name0 / name1 / f"{name2}.json") as f:
             schema = json.load(f)
         key = f"{name1}:{name2}"
         setting = {
```

### Comparing `jupyverse-0.4.2/plugins/lab/fps_lab/static/favicon.ico` & `jupyverse-0.5.0/plugins/lab/fps_lab/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/COPYING.md` & `jupyverse-0.5.0/plugins/login/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/pyproject.toml` & `jupyverse-0.5.0/plugins/login/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/routes.py` & `jupyverse-0.5.0/plugins/login/fps_login/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/index.html` & `jupyverse-0.5.0/plugins/login/fps_login/static/index.html`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-1.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-2.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-busy-3.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-file.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-notebook.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon-terminal.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/favicons/favicon.ico` & `jupyverse-0.5.0/plugins/login/fps_login/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/logo/github.svg` & `jupyverse-0.5.0/plugins/login/fps_login/static/logo/github.svg`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/logo/logo.png` & `jupyverse-0.5.0/plugins/login/fps_login/static/logo/logo.png`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/login/fps_login/static/style/index.css` & `jupyverse-0.5.0/plugins/login/fps_login/static/style/index.css`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/nbconvert/COPYING.md` & `jupyverse-0.5.0/plugins/nbconvert/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/nbconvert/pyproject.toml` & `jupyverse-0.5.0/plugins/nbconvert/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/nbconvert/fps_nbconvert/routes.py` & `jupyverse-0.5.0/plugins/nbconvert/fps_nbconvert/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/noauth/COPYING.md` & `jupyverse-0.5.0/plugins/noauth/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/noauth/pyproject.toml` & `jupyverse-0.5.0/plugins/noauth/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/noauth/fps_noauth/backends.py` & `jupyverse-0.5.0/plugins/noauth/fps_noauth/backends.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/resource_usage/COPYING.md` & `jupyverse-0.5.0/plugins/resource_usage/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/resource_usage/pyproject.toml` & `jupyverse-0.5.0/plugins/resource_usage/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/resource_usage/fps_resource_usage/main.py` & `jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/resource_usage/fps_resource_usage/routes.py` & `jupyverse-0.5.0/plugins/resource_usage/fps_resource_usage/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/retrolab/COPYING.md` & `jupyverse-0.5.0/plugins/notebook/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/retrolab/pyproject.toml` & `jupyverse-0.5.0/plugins/terminals/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_retrolab"
-description = "An FPS plugin for the RetroLab API"
+name = "fps_terminals"
+description = "An FPS plugin for the terminals API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
-    "retrolab",
+    "websockets",
+    "pywinpty;platform_system=='Windows'",
     "jupyverse-api >=0.1.2,<1",
+    "anyio >=4,<5",
 ]
-dynamic = [ "version",]
+dynamic = ["version"]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -29,12 +31,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {retrolab = "fps_retrolab.main:RetroLabComponent"}
-"jupyverse.components" = {retrolab = "fps_retrolab.main:RetroLabComponent"}
+"asphalt.components"   = {terminals = "fps_terminals.main:TerminalsComponent"}
+"jupyverse.components" = {terminals = "fps_terminals.main:TerminalsComponent"}
 
 [tool.hatch.version]
-path = "fps_retrolab/__init__.py"
+path = "fps_terminals/__init__.py"
```

### Comparing `jupyverse-0.4.2/plugins/terminals/COPYING.md` & `jupyverse-0.5.0/plugins/terminals/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/terminals/pyproject.toml` & `jupyverse-0.5.0/plugins/notebook/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 [build-system]
 requires = [ "hatchling",]
 build-backend = "hatchling.build"
 
 [project]
-name = "fps_terminals"
-description = "An FPS plugin for the terminals API"
+name = "fps_notebook"
+description = "An FPS plugin for the Notebook API"
 keywords = ["jupyter", "server", "fastapi", "plugins"]
 requires-python = ">=3.8"
 dependencies = [
-    "websockets",
-    "pywinpty;platform_system=='Windows'",
+    "notebook >=7.1.2,<8.0.0",
     "jupyverse-api >=0.1.2,<1",
-    "anyio >=4,<5",
 ]
-dynamic = ["version"]
+dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
 
 [project.readme]
 file = "README.md"
 content-type = "text/markdown"
@@ -31,12 +29,12 @@
 [tool.check-manifest]
 ignore = [ ".*",]
 
 [tool.jupyter-releaser]
 skip = [ "check-links",]
 
 [project.entry-points]
-"asphalt.components"   = {terminals = "fps_terminals.main:TerminalsComponent"}
-"jupyverse.components" = {terminals = "fps_terminals.main:TerminalsComponent"}
+"asphalt.components"   = {notebook = "fps_notebook.main:NotebookComponent"}
+"jupyverse.components" = {notebook = "fps_notebook.main:NotebookComponent"}
 
 [tool.hatch.version]
-path = "fps_terminals/__init__.py"
+path = "fps_notebook/__init__.py"
```

### Comparing `jupyverse-0.4.2/plugins/terminals/fps_terminals/main.py` & `jupyverse-0.5.0/plugins/terminals/fps_terminals/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/terminals/fps_terminals/routes.py` & `jupyverse-0.5.0/plugins/terminals/fps_terminals/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/terminals/fps_terminals/server.py` & `jupyverse-0.5.0/plugins/terminals/fps_terminals/server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/terminals/fps_terminals/win_server.py` & `jupyverse-0.5.0/plugins/terminals/fps_terminals/win_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/webdav/COPYING.md` & `jupyverse-0.5.0/plugins/webdav/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/webdav/pyproject.toml` & `jupyverse-0.5.0/plugins/webdav/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/webdav/fps_webdav/routes.py` & `jupyverse-0.5.0/plugins/webdav/fps_webdav/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/webdav/tests/test_webdav.py` & `jupyverse-0.5.0/plugins/webdav/tests/test_webdav.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/COPYING.md` & `jupyverse-0.5.0/plugins/yjs/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/pyproject.toml` & `jupyverse-0.5.0/plugins/yjs/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-    "pycrdt >=0.8.2,<0.9.0",
+    "importlib_metadata >=3.6; python_version<'3.10'",
+    "pycrdt >=0.8.16,<0.9.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/main.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/routes.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/utils.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/ybasedoc.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ybasedoc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from abc import ABC, abstractmethod
 from typing import Any, Callable, Dict, Optional
 
-from pycrdt import Doc, Map
+from pycrdt import Doc, Map, Subscription
 
 
 class YBaseDoc(ABC):
     def __init__(self, ydoc: Optional[Doc] = None):
         if ydoc is None:
             self._ydoc = Doc()
         else:
             self._ydoc = ydoc
         self._ystate = Map()
         self._ydoc["state"] = self._ystate
-        self._subscriptions: Dict[Any, str] = {}
+        self._subscriptions: Dict[Any, Subscription] = {}
 
     @property
     @abstractmethod
     def version(self) -> str:
         ...
 
     @property
```

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/yblob.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yblob.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/ynotebook.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/ynotebook.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ydocs/yunicode.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ydocs/yunicode.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/asgi_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/awareness.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/awareness.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/django_channels_consumer.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_provider.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/websocket_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/yroom.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yroom.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/ystore.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/ystore.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywebsocket/yutils.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywebsocket/yutils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/plugins/yjs/fps_yjs/ywidgets/widgets.py` & `jupyverse-0.5.0/plugins/yjs/fps_yjs/ywidgets/widgets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,37 @@
+import sys
 from typing import Any
 
-import pkg_resources
 from pycrdt import TransactionEvent
 
 try:
     from ypywidgets.utils import (  # type: ignore
         YMessageType,
         YSyncMessageType,
         create_update_message,
         process_sync_message,
         sync,
     )
     ypywidgets_installed = True
 except ImportError:
     ypywidgets_installed = False
 
+if sys.version_info < (3, 10):
+    from importlib_metadata import entry_points
+else:
+    from importlib.metadata import entry_points
+
 
 Widgets: Any
 
 if ypywidgets_installed:
     class Widgets:  # type: ignore
         def __init__(self):
             self.ydocs = {
-                ep.name: ep.load() for ep in pkg_resources.iter_entry_points(group="ypywidgets")
+                ep.name: ep.load() for ep in entry_points(group="ypywidgets")
             }
             self.widgets = {}
 
         def comm_open(self, msg, comm) -> None:
             target_name = msg["content"]["target_name"]
             if target_name != "ywidget":
                 return
```

### Comparing `jupyverse-0.4.2/tests/conftest.py` & `jupyverse-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_app.py` & `jupyverse-0.5.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_auth.py` & `jupyverse-0.5.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_contents.py` & `jupyverse-0.5.0/tests/test_contents.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_execute.py` & `jupyverse-0.5.0/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_kernels.py` & `jupyverse-0.5.0/tests/test_kernels.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_server.py` & `jupyverse-0.5.0/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/test_settings.py` & `jupyverse-0.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/utils.py` & `jupyverse-0.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/data/notebook0.ipynb` & `jupyverse-0.5.0/tests/data/notebook0.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/tests/data/notebook1.ipynb` & `jupyverse-0.5.0/tests/data/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/.gitignore` & `jupyverse-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/COPYING.md` & `jupyverse-0.5.0/COPYING.md`

 * *Files identical despite different names*

### Comparing `jupyverse-0.4.2/README.md` & `jupyverse-0.5.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/test/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 
 # jupyverse
 
 A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
-- JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jlab)
-- RetroLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-rlab)
+- JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jupyterlab)
+- Jupyter Notebook frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-notebook)
 
 Documentation is available [here](https://davidbrochart.github.io/jupyverse).
 
 ## Motivation
 
 For the motivations behind this project, please refer to this issue in the
 [Jupyter server team compass](https://github.com/jupyter-server/team-compass/issues/11).
```

### Comparing `jupyverse-0.4.2/pyproject.toml` & `jupyverse-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 text = "BSD 3-Clause License"
 
 [project.urls]
 Homepage = "https://jupyter.org"
 
 [project.optional-dependencies]
 jupyterlab = ["fps-jupyterlab >=0.1.2,<1"]
-retrolab = ["fps-retrolab >=0.1.2,<1"]
+notebook = ["fps-notebook>=0.1.2,<1"]
 auth = ["fps-auth >=0.1.2,<1", "fps-login >=0.1.2,<1"]
 auth-fief = ["fps-auth-fief >=0.1.2,<1"]
 auth-jupyterhub = ["fps-auth-jupyterhub >=0.1.2,<1"]
 noauth = ["fps-noauth >=0.1.2,<1"]
 test = [
     "ruff >=0.1.2",
     "mypy",
@@ -76,37 +76,37 @@
   "pip install -e ./plugins/webdav[test]",
 ]
 features = ["test"]
 
 [tool.hatch.envs.dev.overrides]
 matrix.frontend.post-install-commands = [
   { value = "pip install -e ./plugins/jupyterlab", if = ["jupyterlab"]},
-  { value = "pip install -e ./plugins/retrolab", if = ["retrolab"]},
+  { value = "pip install -e ./plugins/notebook", if = ["notebook"]},
+]
+
+matrix.frontend.scripts = [
+  { key = "typecheck1", value = "typecheck0 ./plugins/jupyterlab", if = ["jupyterlab"] },
+  { key = "typecheck1", value = "typecheck0 ./plugins/notebook", if = ["notebook"] },
 ]
 matrix.auth.post-install-commands = [
   { value = "pip install -e ./plugins/noauth", if = ["noauth"] },
   { value = "pip install -e ./plugins/auth -e ./plugins/login", if = ["auth"] },
   { value = "pip install -e ./plugins/auth_fief", if = ["auth_fief"] },
   { value = "pip install -e ./plugins/auth_jupyterhub", if = ["auth_jupyterhub"] },
 ]
 
-matrix.frontend.scripts = [
-  { key = "typecheck1", value = "typecheck0 ./plugins/jupyterlab", if = ["jupyterlab"] },
-  { key = "typecheck1", value = "typecheck0 ./plugins/retrolab", if = ["retrolab"] },
-]
-
 matrix.auth.scripts = [
   { key = "typecheck", value = "typecheck1 ./plugins/noauth", if = ["noauth"] },
   { key = "typecheck", value = "typecheck1 ./plugins/auth ./plugins/login", if = ["auth"] },
   { key = "typecheck", value = "typecheck1 ./plugins/auth_fief", if = ["auth_fief"] },
   { key = "typecheck", value = "typecheck1 ./plugins/auth_jupyterhub", if = ["auth_jupyterhub"] },
 ]
 
 [[tool.hatch.envs.dev.matrix]]
-frontend = ["jupyterlab", "retrolab"]
+frontend = ["jupyterlab", "notebook"]
 auth = ["noauth", "auth", "auth_fief", "auth_jupyterhub"]
 
 [tool.hatch.envs.dev.scripts]
 test = "pytest ./tests plugins/webdav/tests -v --reruns 5 --timeout=60 --color=yes"
 lint = [
   "ruff format jupyverse jupyverse_api notebooks plugins tests",
   "ruff check jupyverse jupyverse_api notebooks plugins tests --fix",
@@ -166,21 +166,30 @@
     "plugins/auth_jupyterhub:fps-auth-jupyterhub",
     "plugins/contents:fps-contents",
     "plugins/frontend:fps-frontend",
     "plugins/jupyterlab:fps-jupyterlab",
     "plugins/kernels:fps-kernels",
     "plugins/lab:fps-lab",
     "plugins/nbconvert:fps-nbconvert",
-    "plugins/retrolab:fps-retrolab",
+    "plugins/notebook:fps-notebook",
     "plugins/terminals:fps-terminals",
     "plugins/yjs:fps-yjs",
     "plugins/resource_usage:fps-resource-usage",
     "plugins/login:fps-login",
     "plugins/webdav:fps-webdav",
-    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-auth-jupyterhub,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-retrolab,fps-terminals,fps-yjs,fps-resource-usage,fps-webdav"
+    ".:jupyverse:jupyverse_api,fps-noauth,fps-auth,fps-auth-fief,fps-auth-jupyterhub,fps-contents,fps-jupyterlab,fps-kernels,fps-lab,fps-frontend,fps-nbconvert,fps-notebook,fps-terminals,fps-yjs,fps-resource-usage,fps-webdav"
 ]
 
 [tool.hatch.version]
 path = "jupyverse/__init__.py"
 
 [tool.pytest.ini_options]
 asyncio_mode = "strict"
+
+[tool.pixi.project]
+name = ""
+channels = ["conda-forge"]
+platforms = ["linux-64"]
+
+[tool.pixi.dependencies]
+pip = ">=24.0,<25"
+python = "<3.12"
```

### Comparing `jupyverse-0.4.2/PKG-INFO` & `jupyverse-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: jupyverse
-Version: 0.4.2
+Version: 0.5.0
 Summary: A set of FPS plugins implementing a Jupyter server
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
@@ -26,16 +26,16 @@
 Provides-Extra: docs
 Requires-Dist: mkdocs; extra == 'docs'
 Requires-Dist: mkdocs-material; extra == 'docs'
 Provides-Extra: jupyterlab
 Requires-Dist: fps-jupyterlab<1,>=0.1.2; extra == 'jupyterlab'
 Provides-Extra: noauth
 Requires-Dist: fps-noauth<1,>=0.1.2; extra == 'noauth'
-Provides-Extra: retrolab
-Requires-Dist: fps-retrolab<1,>=0.1.2; extra == 'retrolab'
+Provides-Extra: notebook
+Requires-Dist: fps-notebook<1,>=0.1.2; extra == 'notebook'
 Provides-Extra: test
 Requires-Dist: httpx; extra == 'test'
 Requires-Dist: httpx-ws>=0.4.1; extra == 'test'
 Requires-Dist: ipykernel; extra == 'test'
 Requires-Dist: mypy; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Requires-Dist: pytest-asyncio; extra == 'test'
@@ -53,16 +53,16 @@
 [![Build Status](https://github.com/jupyter-server/jupyverse/workflows/test/badge.svg)](https://github.com/jupyter-server/jupyverse/actions)
 
 # jupyverse
 
 A set of [Asphalt](https://asphalt.readthedocs.io) components implementing a Jupyter server.
 
 Try it online:
-- JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jlab)
-- RetroLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-rlab)
+- JupyterLab frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-jupyterlab)
+- Jupyter Notebook frontend: [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter-server/jupyverse/HEAD?urlpath=jupyverse-notebook)
 
 Documentation is available [here](https://davidbrochart.github.io/jupyverse).
 
 ## Motivation
 
 For the motivations behind this project, please refer to this issue in the
 [Jupyter server team compass](https://github.com/jupyter-server/team-compass/issues/11).
```

