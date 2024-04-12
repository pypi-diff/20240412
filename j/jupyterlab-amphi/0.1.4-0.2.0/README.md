# Comparing `tmp/jupyterlab_amphi-0.1.4.tar.gz` & `tmp/jupyterlab_amphi-0.2.0.tar.gz`

## Comparing `jupyterlab_amphi-0.1.4.tar` & `jupyterlab_amphi-0.2.0.tar`

### file list

```diff
@@ -1,118 +1,131 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/.yarnrc.yml
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/MANIFEST.in
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/lerna.json
--rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/output.json
--rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/package.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/setup.py
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/tsconfig.eslint.json
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/tsconfigbase.json
--rw-r--r--   0        0        0   431825 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/yarn.lock
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/_version.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/package.json
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js
--rw-r--r--   0        0        0    91530 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/581.303d96e32a4c90e28d98.js
--rw-r--r--   0        0        0   542386 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/713.672682fff3504f6c1da4.js
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/713.672682fff3504f6c1da4.js.LICENSE.txt
--rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/remoteEntry.b2c83b834b57cd054825.js
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/style.js
--rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/third-party-licenses.json
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/2.5ff850f38644d809e786.js
--rw-r--r--   0        0        0    30859 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/298.73d1171d6e28e5430245.js
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/432.0488919b1f7178c806d4.js
--rw-r--r--   0        0        0      656 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/621.8e6964da49a7b28e9978.js
--rw-r--r--   0        0        0   122686 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/649.6d49d9cc69cbb76697fb.js
--rw-r--r--   0        0        0    88399 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/969.848e74820ca03d893303.js
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/969.848e74820ca03d893303.js.LICENSE.txt
--rw-r--r--   0        0        0     7886 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/remoteEntry.3ff8b1671edf3719adc7.js
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/style.js
--rw-r--r--   0        0        0    28120 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/third-party-licenses.json
--rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/package.json
--rw-r--r--   0        0        0   152538 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js
--rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt
--rw-r--r--   0        0        0    36515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/378.8d63007918eb0fb399f9.js
--rw-r--r--   0        0        0    38689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/550.fc24af3aaabe117c3a69.js
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/631.2e42de0a30aaca0133f5.js
--rw-r--r--   0        0        0     8454 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/remoteEntry.4ac616cbeaf9f2f09472.js
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/style.js
--rw-r--r--   0        0        0    23348 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/third-party-licenses.json
--rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/package.json
--rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/432.34312e1a7db2f3637c41.js
--rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/534.b949d24467a749a658b1.js
--rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/remoteEntry.957754cc111445ec7cb1.js
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/third-party-licenses.json
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/package.json
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/432.85c783ba5ff02c0acd68.js
--rw-r--r--   0        0        0    22967 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/732.b7777d3d4826271f6ab3.js
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/remoteEntry.1751f4c48e4c86d64c78.js
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/style.js
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi_extension/_version.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
--rw-r--r--   0        0        0     2779 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/package.json
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/tsconfig.json
--rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/CustomHandle.tsx
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/PipelineComponent.tsx
--rw-r--r--   0        0        0    25407 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/configUtils.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/declarations.d.ts
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/icons.ts
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/index.ts
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/rendererUtils.tsx
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
--rw-r--r--   0        0        0     4111 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/forms/singleInputCreatableSelectForm.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/base.css
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/index.css
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/index.js
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/crosshair-16.svg
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/minus-16.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/play-16.svg
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/play-circle-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/plus-16.svg
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/plus-24.svg
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/search-16.svg
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/search-24.svg
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/settings-16.svg
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/settings-24.svg
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/trash-16.svg
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/trash-24.svg
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/x-16.svg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/x-square-16.svg
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/package.json
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/pipeline-16.svg
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/pipeline-24.svg
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/tailwind.config.js
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/tsconfig.json
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/schema/extension.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/schema/plugin copy.json
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/schema/plugin.json
--rw-r--r--   0        0        0     5975 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/CodeGenerator.tsx
--rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/Dropzone.tsx
--rw-r--r--   0        0        0    19408 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/PipelineService.tsx
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/customEdge.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/declarations.d.ts
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/icons.ts
--rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/index.ts
--rw-r--r--   0        0        0     2834 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/canvas.css
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/index.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/index.js
--rw-r--r--   0        0        0    32960 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/output.css
--rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/pipeline-category-icon.svg
--rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/react-icon.svg
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/tailwinds_preflight.css
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/api-24.svg
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/file-plus-24.svg
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/file-text-24.svg
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/monitor-24.svg
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/.gitignore
--rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/LICENSE
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/README.md
--rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/.yarnrc.yml
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/MANIFEST.in
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/lerna.json
+-rw-r--r--   0        0        0    61977 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/output.json
+-rw-r--r--   0        0        0     3365 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/package.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/setup.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/tsconfig.eslint.json
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/tsconfigbase.json
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/_version.py
+-rw-r--r--   0        0        0     2689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/package.json
+-rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js
+-rw-r--r--   0        0        0   542676 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt
+-rw-r--r--   0        0        0   115117 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/736.61ace78c7785abf59833.js
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/remoteEntry.3f9ee25d572774e2a4f2.js
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/style.js
+-rw-r--r--   0        0        0    24579 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0    34980 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/12.e1b4412a18535c560cd1.js
+-rw-r--r--   0        0        0    24459 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/143.c7653d290fba1605b212.js.LICENSE.txt
+-rw-r--r--   0        0        0   142152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/379.1427c0520c9ac5a71632.js.LICENSE.txt
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js
+-rw-r--r--   0        0        0    15919 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/454.b60aaa09eed0e7e4a124.js
+-rw-r--r--   0        0        0      835 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/85.227e3aea03a3014cd80a.js.LICENSE.txt
+-rw-r--r--   0        0        0    43275 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/893.7652ea10634779c3ef2f.js
+-rw-r--r--   0        0        0  1436498 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/974.866b25e149fe0014eb94.js
+-rw-r--r--   0        0        0    32808 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/974.866b25e149fe0014eb94.js.LICENSE.txt
+-rw-r--r--   0        0        0     8338 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/remoteEntry.ab2053fa193201a8aa0a.js
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/style.js
+-rw-r--r--   0        0        0   122507 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/package.json
+-rw-r--r--   0        0        0     3510 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/121.8c540e5dd43820941920.js
+-rw-r--r--   0        0        0    22378 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/219.660cd7be25b20ac30f25.js
+-rw-r--r--   0        0        0   152553 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js
+-rw-r--r--   0        0        0      535 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt
+-rw-r--r--   0        0        0    23568 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/550.7ad263262b92cbc9bbee.js
+-rw-r--r--   0        0        0   184979 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/756.cbe8df68f480d40f4c7e.js
+-rw-r--r--   0        0        0     4374 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/756.cbe8df68f480d40f4c7e.js.LICENSE.txt
+-rw-r--r--   0        0        0     8404 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/remoteEntry.c3796f919885e692bcd0.js
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/style.js
+-rw-r--r--   0        0        0    44588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3210 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/package.json
+-rw-r--r--   0        0        0     7640 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/432.34312e1a7db2f3637c41.js
+-rw-r--r--   0        0        0     7241 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/534.8692c2c01fee4d696319.js
+-rw-r--r--   0        0        0     6917 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/remoteEntry.a3e4311f433709c80b81.js
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/third-party-licenses.json
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/package.json
+-rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/432.85c783ba5ff02c0acd68.js
+-rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/732.cb2b06b77f00d8ec6e69.js
+-rw-r--r--   0        0        0     6994 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/remoteEntry.c4969e0c2f708b845d0d.js
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/style.js
+-rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/third-party-licenses.json
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi_extension/_version.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/amphi_venv/lib/python3.11/site-packages/amphi/_version.py
+-rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/package.json
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/tsconfig.json
+-rw-r--r--   0        0        0     6574 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/BrowseFileDialog.tsx
+-rw-r--r--   0        0        0    10137 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/CodeGenerator.tsx
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/CustomHandle.tsx
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/PipelineComponent.tsx
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/PipelineService.tsx
+-rw-r--r--   0        0        0    17880 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/configUtils.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/declarations.d.ts
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/icons.ts
+-rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/index.ts
+-rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/rendererUtils.tsx
+-rw-r--r--   0        0        0     7944 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/keyValueColumns.tsx
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/keyValueForm.tsx
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectColumn.tsx
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectColumns.tsx
+-rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectCustomizable.tsx
+-rw-r--r--   0        0        0     1438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectMultiple.tsx
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectRegular.tsx
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/selectTokenization.tsx
+-rw-r--r--   0        0        0     9743 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/transferData.tsx
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/valuesListForm.tsx
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/base.css
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/index.css
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/index.js
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-16.svg
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/crosshair-16.svg
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/minus-16.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/play-16.svg
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/play-circle-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/plus-16.svg
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/plus-24.svg
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/search-16.svg
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/search-24.svg
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/settings-16.svg
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/settings-24.svg
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/trash-16.svg
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/trash-24.svg
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/x-16.svg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/x-square-16.svg
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/package.json
+-rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/pipeline-16.svg
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/pipeline-24.svg
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/tailwind.config.js
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/tsconfig.json
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/schema/extension.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/schema/plugin copy.json
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/schema/plugin.json
+-rw-r--r--   0        0        0     2213 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/Dropzone.tsx
+-rw-r--r--   0        0        0    18505 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/PipelineEditorWidget.tsx
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/customEdge.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/declarations.d.ts
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/icons.ts
+-rw-r--r--   0        0        0    17975 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/index.ts
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/canvas.css
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/index.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/index.js
+-rw-r--r--   0        0        0    21779 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/output.css
+-rw-r--r--   0        0        0     2211 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/pipeline-category-icon.svg
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/react-icon.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/tailwinds_preflight.css
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/api-24.svg
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/file-plus-24.svg
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/file-text-24.svg
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/monitor-24.svg
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/pipeline-brand-16.svg
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/pipeline-brand-24.svg
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/.gitignore
+-rw-r--r--   0        0        0     3795 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/README.md
+-rw-r--r--   0        0        0     2438 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6964 2020-02-02 00:00:00.000000 jupyterlab_amphi-0.2.0/PKG-INFO
```

### Comparing `jupyterlab_amphi-0.1.4/output.json` & `jupyterlab_amphi-0.2.0/output.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/package.json` & `jupyterlab_amphi-0.2.0/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9615384615384616%*

 * *Differences: {"'version'": "'0.2.0'"}*

```diff
@@ -66,15 +66,15 @@
         "prettier:base": "prettier \"**/*{.ts,.tsx,.js,.jsx,.css,.json,.md,.yml,.yaml}\"",
         "prettier:check": "jlpm prettier:base --check",
         "quickstart": "npm run setup:py && jlpm && jlpm deduplicate && jlpm clean:all && jlpm lint && jlpm build:prod && jlpm dist && jlpm docs && jlpm test",
         "setup:py": "python -m pip install -e \".[dev,lint,test,docs]\"",
         "test": "jlpm test:py",
         "test:py": "pytest"
     },
-    "version": "0.1.4",
+    "version": "0.2.0",
     "workspaces": {
         "packages": [
             "packages/pipeline-editor",
             "packages/pipeline-components-manager",
             "packages/pipeline-components-core",
             "packages/pipeline-console",
             "packages/pipeline-metadata-panel"
```

### Comparing `jupyterlab_amphi-0.1.4/tsconfigbase.json` & `jupyterlab_amphi-0.2.0/tsconfigbase.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/package.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9694791666666666%*

 * *Differences: {"'dependencies'": "{'antd': '^5.16.0'}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.3f9ee25d572774e2a4f2.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -6,14 +6,15 @@
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
         "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
         "@jupyterlab/application": "^4.1.5",
         "@lumino/widgets": "^2.0.0",
+        "antd": "^5.16.0",
         "reactflow": "11.9.4"
     },
     "description": "Amphi Pipeline Core Components",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
@@ -38,15 +39,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.b2c83b834b57cd054825.js",
+            "load": "static/remoteEntry.3f9ee25d572774e2a4f2.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-core",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -82,9 +83,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.6"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/432.df81fd96e756f14c54d0.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/581.303d96e32a4c90e28d98.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/736.61ace78c7785abf59833.js`

 * *Files 16% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 "use strict";
 (self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || []).push([
-    [581], {
-        581: (e, t, n) => {
+    [736], {
+        736: (e, t, n) => {
             n.r(t), n.d(t, {
-                default: () => Oe
+                default: () => Je
             });
-            var a = n(254),
-                o = n(345),
-                s = n.n(o),
+            var o = n(254),
+                a = n(345),
+                s = n.n(a),
                 r = n(473),
-                d = n(153);
+                d = n(664);
             const l = new d.LabIcon({
                     name: "amphi:file-text-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M7.75 12a.75.75 0 000 1.5h8a.75.75 0 000-1.5h-8zM7 16.75a.75.75 0 01.75-.75h6a.75.75 0 010 1.5h-6a.75.75 0 01-.75-.75zM7.75 8a.75.75 0 000 1.5h2a.75.75 0 000-1.5h-2z"/><path fill-rule="evenodd" d="M3 3.75A2.75 2.75 0 015.75 1h7.586c.464 0 .909.184 1.237.513l5.914 5.914c.329.328.513.773.513 1.237V20.25A2.75 2.75 0 0118.25 23H5.75A2.75 2.75 0 013 20.25V3.75zM5.75 2.5c-.69 0-1.25.56-1.25 1.25v16.5c0 .69.56 1.25 1.25 1.25h12.5c.69 0 1.25-.56 1.25-1.25V9h-5.75a.75.75 0 01-.75-.75V2.5H5.75zm8.75 1.06l3.94 3.94H14.5V3.56z" clip-rule="evenodd"/></g></svg>'
                 }),
                 i = new d.LabIcon({
                     name: "amphi:file-plus-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M11.75 10.75a.75.75 0 01.75.75V14H15a.75.75 0 010 1.5h-2.5V18a.75.75 0 01-1.5 0v-2.5H8.5a.75.75 0 010-1.5H11v-2.5a.75.75 0 01.75-.75z"/><path fill-rule="evenodd" d="M5.75 1A2.75 2.75 0 003 3.75v16.5A2.75 2.75 0 005.75 23h12.5A2.75 2.75 0 0021 20.25V8.664c0-.464-.184-.909-.513-1.237l-5.914-5.914A1.75 1.75 0 0013.336 1H5.75zM4.5 3.75c0-.69.56-1.25 1.25-1.25H13v5.75c0 .414.336.75.75.75h5.75v11.25c0 .69-.56 1.25-1.25 1.25H5.75c-.69 0-1.25-.56-1.25-1.25V3.75zM18.44 7.5L14.5 3.56V7.5h3.94z" clip-rule="evenodd"/></g></svg>'
@@ -30,94 +30,104 @@
                     name: "amphi:api-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M2 5a3 3 0 115.585 1.524l1.79 1.79.68-.68a2.75 2.75 0 013.89 0l.68.68 1.79-1.79a3 3 0 111.06 1.06l-1.79 1.791.681.68a2.75 2.75 0 010 3.89l-.68.68 1.79 1.79a3 3 0 11-1.06 1.06l-1.791-1.79-.68.681a2.75 2.75 0 01-3.89 0l-.68-.68-1.79 1.79a3 3 0 11-1.06-1.06l1.79-1.791-.681-.68a2.75 2.75 0 010-3.89l.68-.68-1.79-1.79A3 3 0 012 5zm3-1.5a1.5 1.5 0 100 3 1.5 1.5 0 000-3zm0 14a1.5 1.5 0 100 3 1.5 1.5 0 000-3zM17.5 19a1.5 1.5 0 113 0 1.5 1.5 0 01-3 0zM19 3.5a1.5 1.5 0 100 3 1.5 1.5 0 000-3zm-7.884 5.195a1.25 1.25 0 011.768 0l2.421 2.421a1.25 1.25 0 010 1.768l-2.421 2.421a1.25 1.25 0 01-1.768 0l-2.421-2.421a1.25 1.25 0 010-1.768l2.421-2.421z" clip-rule="evenodd"/></svg>'
                 }),
                 u = new d.LabIcon({
                     name: "amphi:code-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M14.447 3.026a.75.75 0 00-.92.527l-4.5 16.5a.75.75 0 001.447.394l4.5-16.5a.75.75 0 00-.527-.92zM16.207 6.232a.75.75 0 011.06-.025l5.5 5.25a.75.75 0 010 1.085l-5.5 5.25a.75.75 0 01-1.035-1.085L21.164 12l-4.932-4.707a.75.75 0 01-.024-1.06zM7.768 7.293a.75.75 0 00-1.036-1.086l-5.5 5.25a.75.75 0 000 1.085l5.5 5.25a.75.75 0 101.036-1.085L2.836 12l4.932-4.707z"/></g></svg>'
                 }),
-                h = new d.LabIcon({
+                g = new d.LabIcon({
                     name: "amphi:filter-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3 6.75A.75.75 0 013.75 6h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 6.75zM6 11.75a.75.75 0 01.75-.75h10.5a.75.75 0 010 1.5H6.75a.75.75 0 01-.75-.75zM9.75 16a.75.75 0 000 1.5h4.5a.75.75 0 000-1.5h-4.5z"/></g></svg>'
                 }),
-                g = new d.LabIcon({
+                h = new d.LabIcon({
                     name: "amphi:aggregateIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M5 6.75A.75.75 0 015.75 6h6.5a.75.75 0 010 1.5h-6.5A.75.75 0 015 6.75zM5.75 9a.75.75 0 000 1.5h4.5a.75.75 0 000-1.5h-4.5z"/><path fill-rule="evenodd" d="M1 4.75A2.75 2.75 0 013.75 2h10.5c.854 0 1.617.39 2.121 1h.879c.854 0 1.617.39 2.121 1h.879A2.75 2.75 0 0123 6.75v10.5A2.75 2.75 0 0120.25 20h-.879c-.504.61-1.267 1-2.121 1h-.879c-.504.61-1.267 1-2.121 1H3.75A2.75 2.75 0 011 19.25V4.75zM19.989 18.5h.261c.69 0 1.25-.56 1.25-1.25V6.75c0-.69-.56-1.25-1.25-1.25h-.261c.007.082.011.166.011.25v12.5c0 .084-.004.168-.011.25zM17 4.75c0-.084-.004-.168-.011-.25h.261c.69 0 1.25.56 1.25 1.25v12.5c0 .69-.56 1.25-1.25 1.25h-.261c.007-.082.011-.166.011-.25V4.75zM3.75 3.5c-.69 0-1.25.56-1.25 1.25v14.5c0 .69.56 1.25 1.25 1.25h10.5c.69 0 1.25-.56 1.25-1.25V4.75c0-.69-.56-1.25-1.25-1.25H3.75z" clip-rule="evenodd"/></g></svg>'
                 }),
-                f = (new d.LabIcon({
+                f = new d.LabIcon({
                     name: "amphi:mergeIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M3.5 6.5a3.5 3.5 0 114.096 3.45c.102.41.284.886.551 1.406a11.743 11.743 0 001.81 2.54c1.35 1.456 3.014 2.56 4.635 2.804a3.502 3.502 0 016.908.8 3.5 3.5 0 01-6.928.71c-2.178-.252-4.217-1.677-5.716-3.294A13.885 13.885 0 017.5 13.202v7.548a.75.75 0 01-1.5 0V9.855A3.502 3.502 0 013.5 6.5zm3.5-2a2 2 0 100 4 2 2 0 000-4zm9 13a2 2 0 104 0 2 2 0 00-4 0z" clip-rule="evenodd"/></svg>'
-                }), new d.LabIcon({
+                }),
+                v = new d.LabIcon({
                     name: "amphi:expandIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M23 12a.75.75 0 00-.232-.543l-5.5-5.25a.75.75 0 00-1.036 1.086L21.164 12l-4.932 4.707a.75.75 0 001.036 1.085l5.5-5.25A.75.75 0 0023 12zM1 12a.75.75 0 01.232-.543l5.5-5.25a.75.75 0 111.036 1.086L2.836 12l4.932 4.707a.75.75 0 01-1.036 1.085l-5.5-5.25A.75.75 0 011 12z"/><path d="M8 11a1 1 0 100 2h.01a1 1 0 100-2H8zM11 12a1 1 0 011-1h.01a1 1 0 110 2H12a1 1 0 01-1-1zM16 11a1 1 0 100 2h.01a1 1 0 100-2H16z"/></g></svg>'
-                })),
+                }),
                 C = new d.LabIcon({
                     name: "amphi:dedupIcon",
-                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3.75 4a.75.75 0 000 1.5h2.5a.75.75 0 000-1.5h-2.5zM3 9.75A.75.75 0 013.75 9h6.5a.75.75 0 010 1.5h-6.5A.75.75 0 013 9.75zM3.75 14a.75.75 0 000 1.5h6.5a.75.75 0 000-1.5h-6.5zM3.75 19a.75.75 0 000 1.5H20a.75.75 0 000-1.5H3.75zM12.952 12.238a.75.75 0 011.06-.036l2.488 2.322V8.75a3.25 3.25 0 00-3.25-3.25h-2a.75.75 0 010-1.5h2A4.75 4.75 0 0118 8.75v5.774l2.488-2.322a.75.75 0 011.024 1.096l-3.75 3.5a.75.75 0 01-1.024 0l-3.75-3.5a.75.75 0 01-.036-1.06z"/></g></svg>'
-                }),
-                v = new d.LabIcon({
-                    name: "amphi:splitIcon",
-                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M18.265 5.455a.75.75 0 00-1.03 1.09L20.364 9.5H11.75a.75.75 0 000 1.5h8.614l-3.129 2.955a.75.75 0 001.03 1.09l4.5-4.25a.75.75 0 000-1.09l-4.5-4.25zM3.636 13l3.129-2.955a.75.75 0 00-1.03-1.09l-4.5 4.25a.75.75 0 000 1.09l4.5 4.25a.75.75 0 001.03-1.09L3.636 14.5h8.614a.75.75 0 000-1.5H3.636z"/></g></svg>'
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3.75 1A2.75 2.75 0 001 3.75v10.5A2.75 2.75 0 003.75 17h1a.75.75 0 000-1.5h-1c-.69 0-1.25-.56-1.25-1.25V3.75c0-.69.56-1.25 1.25-1.25h10.5c.69 0 1.25.56 1.25 1.25v1a.75.75 0 001.5 0v-1A2.75 2.75 0 0014.25 1H3.75z"/><path fill-rule="evenodd" d="M9.75 7A2.75 2.75 0 007 9.75v10.5A2.75 2.75 0 009.75 23h10.5A2.75 2.75 0 0023 20.25V9.75A2.75 2.75 0 0020.25 7H9.75zM8.5 9.75c0-.69.56-1.25 1.25-1.25h10.5c.69 0 1.25.56 1.25 1.25v10.5c0 .69-.56 1.25-1.25 1.25H9.75c-.69 0-1.25-.56-1.25-1.25V9.75z" clip-rule="evenodd"/></g></svg>'
                 }),
                 I = (new d.LabIcon({
                     name: "amphi:globeIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M12 1C5.925 1 1 5.925 1 12s4.925 11 11 11 11-4.925 11-11S18.075 1 12 1zm-1.673 1.647A9.506 9.506 0 002.552 11h4.747a16.673 16.673 0 013.028-8.353zm3.346 0A16.673 16.673 0 0116.701 11h4.747a9.506 9.506 0 00-7.775-8.353zM15.196 11A15.149 15.149 0 0012 2.916 15.149 15.149 0 008.804 11h6.392zm-6.427 1.5h6.462A15.16 15.16 0 0112 21.084 15.16 15.16 0 018.769 12.5zm-1.502 0H2.513c.23 4.45 3.525 8.091 7.814 8.853a16.683 16.683 0 01-3.06-8.853zm6.406 8.853a16.683 16.683 0 003.06-8.853h4.754c-.23 4.45-3.525 8.091-7.814 8.853z" clip-rule="evenodd"/></svg>'
                 }), new d.LabIcon({
                     name: "amphi:sortIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path d="M3 5.75A.75.75 0 013.75 5h16.5a.75.75 0 010 1.5H3.75A.75.75 0 013 5.75zM3.75 9a.75.75 0 000 1.5h9.5a.75.75 0 000-1.5h-9.5zM16.963 20.443a.747.747 0 00.817-.163l4-4a.75.75 0 10-1.06-1.06L18 17.94V9.75a.75.75 0 00-1.5 0v8.19l-2.72-2.72a.75.75 0 10-1.06 1.06l4 4a.748.748 0 00.243.163zM3.75 13a.75.75 0 000 1.5h5.5a.75.75 0 000-1.5h-5.5zM3 17.75a.75.75 0 01.75-.75h3.5a.75.75 0 010 1.5h-3.5a.75.75 0 01-.75-.75z"/></g></svg>'
                 })),
-                x = new d.LabIcon({
+                b = new d.LabIcon({
                     name: "amphi:editIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path fill-rule="evenodd" d="M17.055 2.884a2.75 2.75 0 013.89 0l.171.171a2.75 2.75 0 010 3.89l-9.005 9.005A4.75 4.75 0 0110.516 17L6.28 18.696a.75.75 0 01-.975-.975l1.695-4.237a4.749 4.749 0 011.051-1.595l9.005-9.005zm2.829 1.06a1.25 1.25 0 00-1.768 0l-.555.556L19.5 6.44l.555-.556a1.25 1.25 0 000-1.768l-.171-.172zM18.439 7.5L16.5 5.56l-7.39 7.39a3.25 3.25 0 00-.719 1.09l-1.045 2.614 2.613-1.046a3.25 3.25 0 001.091-.719L18.44 7.5z" clip-rule="evenodd"/><path d="M3.75 4.5c-.69 0-1.25.56-1.25 1.25v14.5c0 .69.56 1.25 1.25 1.25h14.5c.69 0 1.25-.56 1.25-1.25V13a.75.75 0 011.5 0v7.25A2.75 2.75 0 0118.25 23H3.75A2.75 2.75 0 011 20.25V5.75A2.75 2.75 0 013.75 3H11a.75.75 0 010 1.5H3.75z"/></g></svg>'
                 }),
-                y = new d.LabIcon({
+                _ = new d.LabIcon({
                     name: "amphi:typeIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" d="M3 3.75A.75.75 0 013.75 3h16a.75.75 0 01.75.75v2.5a.75.75 0 01-1.5 0V4.5h-6.5v15h2a.75.75 0 010 1.5H9a.75.75 0 010-1.5h2v-15H4.5v1.75a.75.75 0 01-1.5 0v-2.5z"/></svg>'
                 }),
-                _ = new d.LabIcon({
+                y = new d.LabIcon({
                     name: "amphi:extractIcon",
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M6.5 1.25a.75.75 0 00-1.5 0V5H1.25a.75.75 0 000 1.5H5v9.75A2.75 2.75 0 007.75 19h9.75v3.75a.75.75 0 001.5 0V19h3.75a.75.75 0 000-1.5H19V7.75A2.75 2.75 0 0016.25 5H6.5V1.25zm0 5.25v9.75a1.25 1.25 0 001.25 1.25h9.75V7.75a1.25 1.25 0 00-1.25-1.25H6.5z" clip-rule="evenodd"/></svg>'
+                }),
+                x = new d.LabIcon({
+                    name: "amphi:splitIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor"><path fill-rule="evenodd" d="M5.5 2a3.5 3.5 0 101.99 6.38l3.346 3.12-3.346 3.12a3.5 3.5 0 101.023 1.097l3.93-3.664.009-.008 8.31-7.746A.75.75 0 0019.739 3.2l-7.803 7.274-3.424-3.192A3.5 3.5 0 005.5 2zm-2 3.5a2 2 0 114 0 2 2 0 01-4 0zm0 12a2 2 0 114 0 2 2 0 01-4 0z" clip-rule="evenodd"/><path d="M20.763 18.703a.75.75 0 01-1.026 1.095l-5.5-5.15a.75.75 0 011.026-1.095l5.5 5.15z"/></g></svg>'
                 }),
-                b = new d.LabIcon({
+                w = new d.LabIcon({
                     name: "amphi:googleSheetsIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="#188038" d="M14.266 2l4.984 5h-4.984V2z"/><path fill="#34A853" d="M14.266 7V2H6.109c-.75 0-1.359.61-1.359 1.364v17.272c0 .754.608 1.364 1.36 1.364h11.78c.752 0 1.36-.61 1.36-1.364V7h-4.984z"/><path fill="#FDFFFF" d="M7.469 9.727v6.591h9.062v-6.59H7.47zm3.965 5.455H8.602V13.59h2.832v1.59zm0-2.727H8.602v-1.591h2.832v1.59zm3.964 2.727h-2.832V13.59h2.832v1.59zm0-2.727h-2.832v-1.591h2.832v1.59z"/></svg>'
                 }),
                 N = new d.LabIcon({
                     name: "amphi:mySQLIcon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="64" height="64" viewBox="0 0 25.6 25.6"><path d="M179.076 94.886c-3.568-.1-6.336.268-8.656 1.25-.668.27-1.74.27-1.828 1.116.357.355.4.936.713 1.428.535.893 1.473 2.096 2.32 2.72l2.855 2.053c1.74 1.07 3.703 1.695 5.398 2.766.982.625 1.963 1.428 2.945 2.098.5.357.803.938 1.428 1.16v-.135c-.312-.4-.402-.98-.713-1.428l-1.34-1.293c-1.293-1.74-2.9-3.258-4.64-4.506-1.428-.982-4.55-2.32-5.13-3.97l-.088-.1c.98-.1 2.14-.447 3.078-.715 1.518-.4 2.9-.312 4.46-.713l2.143-.625v-.4c-.803-.803-1.383-1.874-2.23-2.632-2.275-1.963-4.775-3.882-7.363-5.488-1.383-.892-3.168-1.473-4.64-2.23-.537-.268-1.428-.402-1.74-.848-.805-.98-1.25-2.275-1.83-3.436l-3.658-7.763c-.803-1.74-1.295-3.48-2.275-5.086-4.596-7.585-9.594-12.18-17.268-16.687-1.65-.937-3.613-1.34-5.7-1.83l-3.346-.18c-.715-.312-1.428-1.16-2.053-1.562-2.543-1.606-9.102-5.086-10.977-.5-1.205 2.9 1.785 5.755 2.8 7.228.76 1.026 1.74 2.186 2.277 3.346.3.758.4 1.562.713 2.365.713 1.963 1.383 4.15 2.32 5.98.5.937 1.025 1.92 1.65 2.767.357.5.982.714 1.115 1.517-.625.893-.668 2.23-1.025 3.347-1.607 5.042-.982 11.288 1.293 15 .715 1.115 2.4 3.57 4.686 2.632 2.008-.803 1.56-3.346 2.14-5.577.135-.535.045-.892.312-1.25v.1l1.83 3.703c1.383 2.186 3.793 4.462 5.8 5.98 1.07.803 1.918 2.187 3.256 2.677v-.135h-.088c-.268-.4-.67-.58-1.027-.892-.803-.803-1.695-1.785-2.32-2.677-1.873-2.498-3.523-5.265-4.996-8.12-.715-1.383-1.34-2.9-1.918-4.283-.27-.536-.27-1.34-.715-1.606-.67.98-1.65 1.83-2.143 3.034-.848 1.918-.936 4.283-1.248 6.737-.18.045-.1 0-.18.1-1.426-.356-1.918-1.83-2.453-3.078-1.338-3.168-1.562-8.254-.402-11.913.312-.937 1.652-3.882 1.117-4.774-.27-.848-1.16-1.338-1.652-2.008-.58-.848-1.203-1.918-1.605-2.855-1.07-2.5-1.605-5.265-2.766-7.764-.537-1.16-1.473-2.365-2.232-3.435-.848-1.205-1.783-2.053-2.453-3.48-.223-.5-.535-1.294-.178-1.83.088-.357.268-.5.623-.58.58-.5 2.232.134 2.812.4 1.65.67 3.033 1.294 4.416 2.23.625.446 1.295 1.294 2.098 1.518h.938c1.428.312 3.033.1 4.37.5 2.365.76 4.506 1.874 6.426 3.08 5.844 3.703 10.664 8.968 13.92 15.26.535 1.026.758 1.963 1.25 3.034.938 2.187 2.098 4.417 3.033 6.56.938 2.097 1.83 4.24 3.168 5.98.67.937 3.346 1.427 4.55 1.918.893.4 2.275.76 3.08 1.25 1.516.937 3.033 2.008 4.46 3.034.713.534 2.945 1.65 3.078 2.54zm-45.5-38.772a7.09 7.09 0 0 0-1.828.223v.1h.088c.357.714.982 1.205 1.428 1.83l1.027 2.142.088-.1c.625-.446.938-1.16.938-2.23-.268-.312-.312-.625-.535-.937-.268-.446-.848-.67-1.206-1.026z" transform="matrix(.390229 0 0 .38781 -46.300037 -16.856717)" fill-rule="evenodd" fill="#00678c"/></svg>'
                 }),
-                w = new d.LabIcon({
+                F = new d.LabIcon({
                     name: "amphi:box-icon",
                     svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" fill="none" viewBox="0 0 16 16"><path fill="currentColor" fill-rule="evenodd" d="M6.98.678a2.25 2.25 0 012.04 0l5.297 2.696c.42.214.683.644.683 1.114v6.717c0 .658-.37 1.261-.956 1.56L9.02 15.322a2.25 2.25 0 01-2.042 0l-5.023-2.557A1.75 1.75 0 011 11.205V4.488c0-.47.264-.9.683-1.114L6.979.678zm1.36 1.337a.75.75 0 00-.68 0L3.224 4.273 8 6.661l4.776-2.388L8.34 2.015zm-5.84 9.19V5.588l4.75 2.375v5.814l-4.613-2.35a.25.25 0 01-.137-.222zm6.25 2.572l4.613-2.35a.25.25 0 00.137-.222V5.588L8.75 7.963v5.814z" clip-rule="evenodd"/></svg>'
+                }),
+                S = new d.LabIcon({
+                    name: "amphi:redditIcon",
+                    svgstr: '<svg viewBox="0 0 800 800" xmlns="http://www.w3.org/2000/svg" width="2500" height="2500"><circle cx="400" cy="400" fill="#ff4500" r="400"/><path d="M666.8 400c.08 5.48-.6 10.95-2.04 16.24s-3.62 10.36-6.48 15.04c-2.85 4.68-6.35 8.94-10.39 12.65s-8.58 6.83-13.49 9.27c.11 1.46.2 2.93.25 4.4a107.268 107.268 0 0 1 0 8.8c-.05 1.47-.14 2.94-.25 4.4 0 89.6-104.4 162.4-233.2 162.4S168 560.4 168 470.8c-.11-1.46-.2-2.93-.25-4.4a107.268 107.268 0 0 1 0-8.8c.05-1.47.14-2.94.25-4.4a58.438 58.438 0 0 1-31.85-37.28 58.41 58.41 0 0 1 7.8-48.42 58.354 58.354 0 0 1 41.93-25.4 58.4 58.4 0 0 1 46.52 15.5 286.795 286.795 0 0 1 35.89-20.71c12.45-6.02 25.32-11.14 38.51-15.3s26.67-7.35 40.32-9.56 27.45-3.42 41.28-3.63L418 169.6c.33-1.61.98-3.13 1.91-4.49.92-1.35 2.11-2.51 3.48-3.4 1.38-.89 2.92-1.5 4.54-1.8 1.61-.29 3.27-.26 4.87.09l98 19.6c9.89-16.99 30.65-24.27 48.98-17.19s28.81 26.43 24.71 45.65c-4.09 19.22-21.55 32.62-41.17 31.61-19.63-1.01-35.62-16.13-37.72-35.67L440 186l-26 124.8c13.66.29 27.29 1.57 40.77 3.82a284.358 284.358 0 0 1 77.8 24.86A284.412 284.412 0 0 1 568 360a58.345 58.345 0 0 1 29.4-15.21 58.361 58.361 0 0 1 32.95 3.21 58.384 58.384 0 0 1 25.91 20.61A58.384 58.384 0 0 1 666.8 400zm-396.96 55.31c2.02 4.85 4.96 9.26 8.68 12.97 3.71 3.72 8.12 6.66 12.97 8.68A40.049 40.049 0 0 0 306.8 480c16.18 0 30.76-9.75 36.96-24.69 6.19-14.95 2.76-32.15-8.68-43.59s-28.64-14.87-43.59-8.68c-14.94 6.2-24.69 20.78-24.69 36.96 0 5.25 1.03 10.45 3.04 15.31zm229.1 96.02c2.05-2 3.22-4.73 3.26-7.59.04-2.87-1.07-5.63-3.07-7.68s-4.73-3.22-7.59-3.26c-2.87-.04-5.63 1.07-7.94 2.8a131.06 131.06 0 0 1-19.04 11.35 131.53 131.53 0 0 1-20.68 7.99c-7.1 2.07-14.37 3.54-21.72 4.39-7.36.85-14.77 1.07-22.16.67-7.38.33-14.78.03-22.11-.89a129.01 129.01 0 0 1-21.64-4.6c-7.08-2.14-13.95-4.88-20.56-8.18s-12.93-7.16-18.89-11.53c-2.07-1.7-4.7-2.57-7.38-2.44s-5.21 1.26-7.11 3.15c-1.89 1.9-3.02 4.43-3.15 7.11s.74 5.31 2.44 7.38c7.03 5.3 14.5 9.98 22.33 14s16 7.35 24.4 9.97 17.01 4.51 25.74 5.66c8.73 1.14 17.54 1.53 26.33 1.17 8.79.36 17.6-.03 26.33-1.17A153.961 153.961 0 0 0 476.87 564c7.83-4.02 15.3-8.7 22.33-14zm-7.34-68.13c5.42.06 10.8-.99 15.81-3.07 5.01-2.09 9.54-5.17 13.32-9.06s6.72-8.51 8.66-13.58A39.882 39.882 0 0 0 532 441.6c0-16.18-9.75-30.76-24.69-36.96-14.95-6.19-32.15-2.76-43.59 8.68s-14.87 28.64-8.68 43.59c6.2 14.94 20.78 24.69 36.96 24.69z" fill="#fff"/></svg>'
+                }),
+                $ = new d.LabIcon({
+                    name: "amphi:crosshairIcon",
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><path fill="currentColor" fill-rule="evenodd" d="M1 12C1 5.925 5.925 1 12 1s11 4.925 11 11-4.925 11-11 11S1 18.075 1 12zm11.75 9.47v-2.72a.75.75 0 00-1.5 0v2.72a9.502 9.502 0 01-8.72-8.72h2.72a.75.75 0 000-1.5H2.53a9.502 9.502 0 018.72-8.72v2.72a.75.75 0 001.5 0V2.53a9.502 9.502 0 018.72 8.72h-2.72a.75.75 0 000 1.5h2.72a9.502 9.502 0 01-8.72 8.72z" clip-rule="evenodd"/></svg>'
+                }),
+                E = new d.LabIcon({
+                    name: "amphi:randomIcon",
+                    svgstr: '<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" fill="none" viewBox="0 0 24 24"><g fill="currentColor" fill-rule="evenodd" clip-rule="evenodd"><path d="M12 9.5a2.5 2.5 0 100 5 2.5 2.5 0 000-5zM11 12a1 1 0 112 0 1 1 0 01-2 0zM5 7.5a2.5 2.5 0 115 0 2.5 2.5 0 01-5 0zm2.5-1a1 1 0 100 2 1 1 0 000-2zM16.5 14a2.5 2.5 0 100 5 2.5 2.5 0 000-5zm-1 2.5a1 1 0 112 0 1 1 0 01-2 0z"/><path d="M4.75 2A2.75 2.75 0 002 4.75v14.5A2.75 2.75 0 004.75 22h14.5A2.75 2.75 0 0022 19.25V4.75A2.75 2.75 0 0019.25 2H4.75zM3.5 4.75c0-.69.56-1.25 1.25-1.25h14.5c.69 0 1.25.56 1.25 1.25v14.5c0 .69-.56 1.25-1.25 1.25H4.75c-.69 0-1.25-.56-1.25-1.25V4.75z"/></g></svg>'
                 });
-            var F, $, E, k, P, S, T, H, V, O, D, A, M, U, z, L, j, R, q, B, G, Q, J, W, Z, K, X, Y, ee, te, ne;
-            class ae extends((0, a.PipelineComponent)()) {
+            var P, T, k, H, A, V, D, M, O, z, U, L, j, R, q, B, G, J, Q, W, K, Z, X, Y, ee, te, ne, oe, ae, se, re, de, le, ie, me;
+            class ce extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "CSV File Input", this._id = "csvFileInput", this._type = "pandas_df_input", this._fileDrop = ["csv", "tsv"], this._category = "input", this._icon = l, this._default = {
                         csvOptions: {
                             sep: ","
                         }
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
                             placeholder: "Type file name",
-                            validation: "\\.(csv|tsv|txt)$",
-                            validationMessage: "This field expects a file with a csv, tsv or txt extension such as input.csv."
+                            tooltip: "This field expects a file path with a csv, tsv or txt extension such as input.csv.",
+                            validation: "\\.(csv|tsv|txt)$"
                         }, {
-                            type: "singleInputCreatableSelect",
+                            type: "selectCustomizable",
                             label: "Separator",
                             id: "csvOptions.sep",
                             placeholder: "default: ,",
+                            tooltip: "Select or provide a custom deilimiter.",
                             options: [{
-                                value: "null",
-                                label: "Select or type delimiter",
-                                isDisabled: !0
-                            }, {
                                 value: ",",
                                 label: "comma (,)"
                             }, {
                                 value: ";",
                                 label: "semicolon (;)"
                             }, {
                                 value: " ",
@@ -129,21 +139,39 @@
                                 value: "|",
                                 label: "pipe (|)"
                             }, {
                                 value: "infer",
                                 label: "infer (tries to auto detect)"
                             }]
                         }, {
-                            type: "input",
+                            type: "selectCustomizable",
+                            tooltip: "Row number containing column labels and marking the start of the data (zero-indexed).",
                             label: "Header",
                             id: "csvOptions.header",
-                            placeholder: "infer",
+                            options: [{
+                                value: "None",
+                                label: "None"
+                            }, {
+                                value: "0",
+                                label: "First line"
+                            }, {
+                                value: "1",
+                                label: "Second Line"
+                            }],
+                            advanced: !0
+                        }, {
+                            type: "selectTokenization",
+                            tooltip: "Sequence of column labels to apply.",
+                            label: "Column names",
+                            id: "csvOptions.names",
+                            placeholder: "Type header fields (ordered and comma-separated)",
+                            options: [],
                             advanced: !0
                         }, {
-                            type: "singleInputSelect",
+                            type: "select",
                             label: "On Bad Lines",
                             id: "csvOptions.on_bad_lines",
                             placeholder: "error",
                             options: [{
                                 value: "error",
                                 label: "Error: raise an Exception when a bad line is encountered"
                             }, {
@@ -157,152 +185,162 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ae.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ce.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ae.Name,
-                        ConfigForm: ae.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ce.Name,
+                        ConfigForm: ce.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ae.Icon,
+                        Icon: ce.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     let n = {
                         ...e.csvOptions
                     };
-                    "infer" === n.sep && (n.sep = "None", n.engine = "python");
-                    let a = Object.entries(n).filter((([e, t]) => null !== t && "" !== t && !("sep" === e && "infer" === t))).map((([e, t]) => "None" === t ? `${e}=${t}` : `${e}='${t}'`)).join(", ");
-                    return `\n# Reading data from ${e.filePath}\n${t} = pd.read_csv('${e.filePath}'${a?`, ${a}`:""}).convert_dtypes()\n`
+                    "infer" === n.sep && (n.sep = "None", n.engine = "python"), "number" != typeof e.header && "None" !== e.header || (n.header = e.header), e.names && Array.isArray(e.names) && (n.names = `['${e.names.join("', '")}']`, n.header = 0);
+                    let o = Object.entries(n).filter((([e, t]) => null !== t && "" !== t && !("sep" === e && "infer" === t))).map((([e, t]) => "header" !== e || "number" != typeof t && "None" !== t ? "names" === e ? `${e}=${t}` : "string" == typeof t && "None" !== t ? `${e}='${t}'` : `${e}=${t}` : `${e}=${t}`)).join(", ");
+                    return `\n# Reading data from ${e.filePath}\n${t} = pd.read_csv('${e.filePath}'${o?`, ${o}`:""}).convert_dtypes()\n`
                 }
             }
-            F = ae, ae.ConfigForm = ({
+            P = ce, ce.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = F.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = P.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: F.Type,
-                    name: F.Name,
-                    form: F.Form,
+                    type: P.Type,
+                    name: P.Name,
+                    form: P.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class oe extends((0, a.PipelineComponent)()) {
+            class pe extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "JSON File Input", this._id = "jsonFileInput", this._type = "pandas_df_input", this._fileDrop = ["json", "jsonl"], this._category = "input", this._icon = l, this._default = {
                         jsonOptions: {}
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
                             placeholder: "Type file name",
                             validation: ".(json|jsonl)$",
                             validationMessage: "This field expects a file with a json extension such as input.json."
                         }, {
-                            type: "datalist",
+                            type: "select",
                             label: "Orientation",
                             id: "jsonOptions.orient",
                             placeholder: "default: columns",
                             options: [{
-                                key: "columns",
                                 value: "columns",
-                                text: "Columns - JSON object with column labels as keys"
+                                label: "Columns - JSON object with column labels as keys"
                             }, {
-                                key: "records",
                                 value: "records",
-                                text: "Records - List of rows as JSON objects"
+                                label: "Records - List of rows as JSON objects"
                             }, {
-                                key: "index",
                                 value: "index",
-                                text: "Index - Dict with index labels as keys"
+                                label: "Index - Dict with index labels as keys"
                             }, {
-                                key: "split",
                                 value: "split",
-                                text: 'Split - Dict with "index", "columns", and "data" keys'
+                                label: 'Split - Dict with "index", "columns", and "data" keys'
                             }, {
-                                key: "table",
                                 value: "table",
-                                text: 'Table - Dict with "schema" and "data" keys, following the Table Schema'
+                                label: 'Table - Dict with "schema" and "data" keys, following the Table Schema'
                             }]
                         }, {
                             type: "boolean",
                             label: "Infer Data Types",
                             id: "jsonOptions.dtype",
                             advanced: !0
                         }, {
@@ -313,157 +351,169 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: oe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: pe.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: oe.Name,
-                        ConfigForm: oe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: pe.Name,
+                        ConfigForm: pe.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: oe.Icon,
+                        Icon: pe.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     let n = Object.entries(e.jsonOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
-                    const a = n ? `, ${n}` : "";
-                    return `\n${t} = pd.read_json('${e.filePath}'${a}).convert_dtypes()\n`
+                    const o = n ? `, ${n}` : "";
+                    return `\n${t} = pd.read_json('${e.filePath}'${o}).convert_dtypes()\n`
                 }
             }
-            $ = oe, oe.ConfigForm = ({
+            T = pe, pe.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = $.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = T.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: $.Type,
-                    name: $.Name,
-                    form: $.Form,
+                    type: T.Type,
+                    name: T.Name,
+                    form: T.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class se extends((0, a.PipelineComponent)()) {
+            class ue extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Excel File Input", this._id = "excelfileInput", this._type = "pandas_df_input", this._category = "input", this._icon = l, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
                             placeholder: "Type file name",
                             validation: "\\.(xlsx)$",
                             validationMessage: "This field expects a file with a xlsx extension such as input.xlsx."
                         }, {
-                            type: "datalist",
+                            type: "selectCustomizable",
                             label: "Sheets",
                             id: "excelOptions.sheet",
-                            placeholder: "default: 0 (1st sheet)",
+                            placeholder: "Default: O (first sheet)",
                             options: [{
-                                key: "0",
                                 value: "0",
-                                text: "1st sheet"
+                                label: "0"
                             }, {
-                                key: "1",
                                 value: "1",
-                                text: "2nd sheet"
+                                label: "1t"
                             }, {
-                                key: "dict",
                                 value: "[0, 1, 'Sheet5']",
-                                text: "Load first, second and sheet named 'Sheet5'"
+                                label: "[0, 1, 'Sheet5']"
                             }, {
-                                key: "none",
                                 value: "None",
-                                text: "All worksheets"
+                                label: "All"
                             }]
                         }, {
-                            type: "datalist",
+                            type: "selectCustomizable",
                             label: "Header",
                             id: "excelOptions.header",
                             placeholder: "default: 0 (first row)",
                             options: [{
-                                key: "0",
                                 value: "0",
-                                text: "1st row"
+                                label: "0 (1st row)"
+                            }, {
+                                value: "1",
+                                label: "1 (2nd row)"
                             }, {
-                                key: "none",
                                 value: "None",
-                                text: "None if there is no header."
+                                label: "None (No header)"
                             }],
                             advanced: !0
                         }, {
                             type: "boolean",
                             label: "Verbose",
                             id: "excelOptions.verbose",
                             placeholder: "false",
@@ -471,53 +521,66 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: se.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ue.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: se.Name,
-                        ConfigForm: se.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ue.Name,
+                        ConfigForm: ue.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: se.Icon,
+                        Icon: ue.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
@@ -525,57 +588,59 @@
                     config: e,
                     outputName: t
                 }) {
                     let n = e.excelOptions ? Object.entries(e.excelOptions).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ") : null;
                     return n ? `${t} = pd.read_excel('${e.filePath}', ${n}).convert_dtypes()\n` : `${t} = pd.read_excel('${e.filePath}').convert_dtypes()\n`
                 }
             }
-            E = se, se.ConfigForm = ({
+            k = ue, ue.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = E.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = k.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: E.Type,
-                    name: E.Name,
-                    form: E.Form,
+                    type: k.Type,
+                    name: k.Name,
+                    form: k.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class re extends((0, a.PipelineComponent)()) {
+            class ge extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "REST Input", this._id = "restInput", this._type = "pandas_df_input", this._category = "input", this._icon = p, this._default = {
                         method: "GET",
                         headers: []
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
@@ -584,29 +649,25 @@
                             id: "url",
                             placeholder: "Endpoint URL"
                         }, {
                             type: "radio",
                             label: "Method",
                             id: "method",
                             options: [{
-                                key: "GET",
                                 value: "GET",
-                                text: "GET"
+                                label: "GET"
                             }, {
-                                key: "PUT",
                                 value: "PUT",
-                                text: "PUT"
+                                label: "PUT"
                             }, {
-                                key: "POST",
                                 value: "POST",
-                                text: "POST"
+                                label: "POST"
                             }, {
-                                key: "DELETE",
                                 value: "DELETE",
-                                text: "DELETE"
+                                label: "DELETE"
                             }],
                             advanced: !0
                         }, {
                             type: "keyvalue",
                             label: "Headers",
                             id: "headers",
                             advanced: !0
@@ -625,118 +686,133 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: re.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ge.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: re.Name,
-                        ConfigForm: re.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ge.Name,
+                        ConfigForm: ge.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: re.Icon,
+                        Icon: ge.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import json", "import requests", "from jsonpath_ng import parse"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     let n = "";
                     e.body && "" !== e.body.trim() && (n = `json=${e.body.trim()}, `);
-                    let a = "";
-                    e.headers && e.headers.length > 0 && (a = "headers={" + e.headers.map((e => `"${e.key}": "${e.value}"`)).join(", ") + "}, ");
                     let o = "";
-                    o = e.jsonPath && "" !== e.jsonPath.trim() ? `jsonpath_expr = parse('${e.jsonPath}')\nselected_data = [match.value for match in jsonpath_expr.find(data)] if jsonpath_expr.find(data) else []\n${t} = pd.DataFrame(selected_data).convert_dtypes() if selected_data else pd.DataFrame()\n` : `${t} = pd.DataFrame([data]).convert_dtypes() if isinstance(data, dict) else pd.DataFrame(data).convert_dtypes()\n`;
-                    const s = `${a}${n}`,
+                    e.headers && e.headers.length > 0 && (o = "headers={" + e.headers.map((e => `"${e.key}": "${e.value}"`)).join(", ") + "}, ");
+                    let a = "";
+                    a = e.jsonPath && "" !== e.jsonPath.trim() ? `jsonpath_expr = parse('${e.jsonPath}')\nselected_data = [match.value for match in jsonpath_expr.find(data)] if jsonpath_expr.find(data) else []\n${t} = pd.DataFrame(selected_data).convert_dtypes() if selected_data else pd.DataFrame()\n` : `${t} = pd.DataFrame([data]).convert_dtypes() if isinstance(data, dict) else pd.DataFrame(data).convert_dtypes()\n`;
+                    const s = `${o}${n}`,
                         r = s.endsWith(", ") ? s.slice(0, -2) : s;
-                    return `\nimport requests\nfrom jsonpath_ng import parse\nresponse = requests.request(\n  method="${e.method}",\n  url="${e.url}"${r?", "+r:""}\n)\ndata = response.json()\n${o}\n`
+                    return `\nimport requests\nfrom jsonpath_ng import parse\nresponse = requests.request(\n  method="${e.method}",\n  url="${e.url}"${r?", "+r:""}\n)\ndata = response.json()\n${a}\n`
                 }
             }
-            k = re, re.ConfigForm = ({
+            H = ge, ge.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = k.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = H.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: k.Type,
-                    name: k.Name,
-                    form: k.Form,
+                    type: H.Type,
+                    name: H.Name,
+                    form: H.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class de extends((0, a.PipelineComponent)()) {
+            class he extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Parquet File Input", this._id = "parquetFileInput", this._type = "pandas_df_input", this._category = "input", this._icon = l, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -746,112 +822,127 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: de.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: he.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: de.Name,
-                        ConfigForm: de.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: he.Name,
+                        ConfigForm: he.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: de.Icon,
+                        Icon: he.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import pyarrow"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     return `\n# Reading data from ${e.filePath}\n${t} = pd.read_parquet('${e.filePath}').convert_dtypes()\n`
                 }
             }
-            P = de, de.ConfigForm = ({
+            A = he, he.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = P.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = A.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: P.Type,
-                    name: P.Name,
-                    form: P.Form,
+                    type: A.Type,
+                    name: A.Name,
+                    form: A.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class le extends((0, a.PipelineComponent)()) {
+            class fe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "XML File Input", this._id = "xmlFileInput", this._type = "xml_input", this._fileDrop = ["xml"], this._category = "input", this._icon = l, this._default = {
+                    super(...arguments), this._name = "XML File Input", this._id = "xmlFileInput", this._type = "pandas_df_input", this._fileDrop = ["xml"], this._category = "input", this._icon = l, this._default = {
                         xmlOptions: {
                             xpath: ""
                         }
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
@@ -868,128 +959,144 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: le.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: fe.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: le.Name,
-                        ConfigForm: le.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: fe.Name,
+                        ConfigForm: fe.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: le.Icon,
+                        Icon: fe.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import xml.etree.ElementTree as ET"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     const n = `${t}_tree`,
-                        a = `${t}_root`;
-                    let o = e.xmlOptions.xpath ? `"${e.xmlOptions.xpath}"` : "'.'";
-                    return `\n${n} = ET.parse('${e.filePath}')\n${a} = ${n}.getroot()\n${t} = ${a}.findall(${o})\n    `
+                        o = `${t}_root`;
+                    let a = e.xmlOptions.xpath ? `"${e.xmlOptions.xpath}"` : "'.'";
+                    return `\n${n} = ET.parse('${e.filePath}')\n${o} = ${n}.getroot()\n${t} = ${o}.findall(${a})\n    `
                 }
             }
-            S = le, le.ConfigForm = ({
+            V = fe, fe.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = S.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = V.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: S.Type,
-                    name: S.Name,
-                    form: S.Form,
+                    type: V.Type,
+                    name: V.Name,
+                    form: V.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ie extends((0, a.PipelineComponent)()) {
+            class ve extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "G. Sheets Input", this._id = "googleSheetsInput", this._type = "pandas_df_input", this._category = "input", this._icon = b, this._default = {
+                    super(...arguments), this._name = "G. Sheets Input", this._id = "googleSheetsInput", this._type = "pandas_df_input", this._category = "input", this._icon = w, this._default = {
                         sheetOptions: {
                             spreadsheetId: "",
                             range: "Sheet1"
                         }
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "Service Account Key",
                             id: "filePath",
                             placeholder: "Type file name",
                             validation: "\\.(json)$",
-                            validationMessage: "This field expects a file with a .json extension such as your-service-account-file.json."
+                            validationMessage: "This field expects a file with a .json extension such as your-service-account-file.json.",
+                            advanced: !0
                         }, {
                             type: "input",
                             label: "Spreadsheet ID",
                             id: "sheetOptions.spreadsheetId",
                             placeholder: "Enter Google Sheets' name or ID",
                             validation: "^[a-zA-Z0-9-_]+$",
                             validationMessage: "Invalid Spreadsheet ID."
@@ -1003,117 +1110,132 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ie.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ve.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ie.Name,
-                        ConfigForm: ie.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ve.Name,
+                        ConfigForm: ve.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ie.Icon,
+                        Icon: ve.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import gspread", "from oauth2client.service_account import ServiceAccountCredentials"]
                 }
                 generateComponentCode({
                     config: e,
                     outputName: t
                 }) {
                     let n = {
                         ...e.sheetOptions
                     };
-                    const a = e.filePath ? `'${e.filePath}'` : "None";
+                    const o = !!e.filePath && "" !== e.filePath.trim();
                     Object.entries(n).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
-                    const o = `${t}Client`,
+                    const a = `${t}Client`,
                         s = `${t}Sheet`;
-                    return `\n# Reading data from Google Sheets\nscope = ['https://spreadsheets.google.com/feeds','https://www.googleapis.com/auth/drive']\ncreds = ServiceAccountCredentials.from_json_keyfile_name(${a}, scope)\n${o} = gspread.authorize(creds)\n\n# Open the spreadsheet\n${s} = ${o}.open_by_key(${n.spreadsheetId?`'${n.spreadsheetId}'`:"None"}).worksheet(${n.range?`'${n.range.split("!")[0]}'`:"None"})\n\n# Convert to DataFrame\n${t} = pd.DataFrame(${s}.get_all_records())\n`
+                    return `\n# Reading data from Google Sheets\n${o?`# Authentication with service account\nscope = ['https://spreadsheets.google.com/feeds','https://www.googleapis.com/auth/drive']\ncreds = ServiceAccountCredentials.from_json_keyfile_name('${e.filePath}', scope)\n${a} = gspread.authorize(creds)\n`:`# Accessing public sheet without authentication\n${a} = gspread.service_account()\n`}\n# Open the spreadsheet\n${s} = ${a}.open_by_key(${n.spreadsheetId?`'${n.spreadsheetId}'`:"None"}).worksheet(${n.range?`'${n.range.split("!")[0]}'`:"None"})\n  \n# Convert to DataFrame\n${t} = pd.DataFrame(${s}.get_all_records())\n`
                 }
             }
-            T = ie, ie.ConfigForm = ({
+            D = ve, ve.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = T.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = D.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: T.Type,
-                    name: T.Name,
-                    form: T.Form,
+                    type: D.Type,
+                    name: D.Name,
+                    form: D.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class me extends((0, a.PipelineComponent)()) {
+            class Ce extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "MySQL Input", this._id = "mySQLInput", this._type = "pandas_df_input", this._category = "input", this._icon = N, this._default = {
                         dbOptions: {
                             host: "localhost",
                             port: "3306",
                             databaseName: "",
                             username: "",
@@ -1159,53 +1281,66 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: me.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ce.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: me.Name,
-                        ConfigForm: me.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ce.Name,
+                        ConfigForm: Ce.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: me.Icon,
+                        Icon: Ce.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import sqlalchemy", "import pymysql"]
                 }
@@ -1213,57 +1348,59 @@
                     config: e,
                     outputName: t
                 }) {
                     const n = `${t}_Engine`;
                     return `\n# Connect to the MySQL database\n${n} = sqlalchemy.create_engine('mysql+pymysql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}')\n${t} = pd.read_sql_table('${e.dbOptions.tableName}', ${n}).convert_dtypes()\n`
                 }
             }
-            H = me, me.ConfigForm = ({
+            M = Ce, Ce.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = H.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = M.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: H.Type,
-                    name: H.Name,
-                    form: H.Form,
+                    type: M.Type,
+                    name: M.Name,
+                    form: M.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ce extends((0, a.PipelineComponent)()) {
+            class Ie extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "HTML File Input", this._id = "htmlInput", this._type = "pandas_df_input", this._fileDrop = ["html", "htm"], this._category = "input", this._icon = l, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
@@ -1273,53 +1410,66 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ce.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ie.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ce.Name,
-                        ConfigForm: ce.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ie.Name,
+                        ConfigForm: Ie.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ce.Icon,
+                        Icon: Ie.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     let t = [];
                     return t.push("import pandas as pd"), t.push("from unstructured.partition.html import partition_html"), t.push("from unstructured.staging.base import convert_to_dataframe"), t
@@ -1328,130 +1478,145 @@
                     config: e,
                     outputName: t
                 }) {
                     let n = "";
                     return Object.entries(e.jsonOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", "), n += `\n# Retrieve raw HTML from ${e.filePath}\n${t}_elements = partition_html(filename="${e.filePath}")\n${t} = convert_to_dataframe(${t}_elements)\n`, n
                 }
             }
-            V = ce, ce.ConfigForm = ({
+            O = Ie, Ie.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = V.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = O.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: V.Type,
-                    name: V.Name,
-                    form: V.Form,
+                    type: O.Type,
+                    name: O.Name,
+                    form: O.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class pe extends((0, a.PipelineComponent)()) {
+            class be extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "PDF File Input", this._id = "pdfInput", this._type = "pandas_df_input", this._fileDrop = ["pdf"], this._category = "input", this._icon = l, this._default = {
                         strategy: "fast"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "file",
                             label: "File path",
                             id: "filePath",
                             placeholders: "Select or type file",
                             validation: "\\.(pdf)$",
                             validationMessage: "This field expects a file with a pdf extension such as file.pdf."
                         }, {
-                            type: "singleInputSelect",
+                            type: "select",
                             label: "Strategy",
                             id: "strategy",
                             options: [{
                                 value: "fast",
                                 label: "Fast"
                             }]
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: pe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: be.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: pe.Name,
-                        ConfigForm: pe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: be.Name,
+                        ConfigForm: be.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: pe.Icon,
+                        Icon: be.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideDependencies({
                     config: e
                 }) {
                     let t = [];
-                    return t.push("pdf2image"), t.push("pdfminer.six"), t.push("pillow_heif"), t.push("opencv-python"), t.push("pypdf"), t.push("pikepdf"), t
+                    return t.push("pdf2image"), t.push("pdfminer.six"), t.push("pillow_heif"), t.push("opencv-python"), t.push("pikepdf"), t
                 }
                 provideImports({
                     config: e
                 }) {
                     let t = [];
                     return t.push("import pandas as pd"), t.push("from unstructured.partition.pdf import partition_pdf"), t.push("from unstructured.staging.base import convert_to_dataframe"), t
                 }
@@ -1459,1527 +1624,2180 @@
                     config: e,
                     outputName: t
                 }) {
                     let n = "";
                     return n += `\n# Read PDF and retrieve text from ${e.filePath}\n${t}_elements = partition_pdf(\n  filename="${e.filePath}",\n  strategy="${e.strategy}",\n  extract_images_in_pdf=False\n)\n${t} = convert_to_dataframe(${t}_elements)\n`, n
                 }
             }
-            O = pe, pe.ConfigForm = ({
+            z = be, be.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = O.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = z.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: O.Type,
-                    name: O.Name,
-                    form: O.Form,
+                    type: z.Type,
+                    name: z.Name,
+                    form: z.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ue extends((0, a.PipelineComponent)()) {
+            class _e extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "CSV File Output", this._id = "csvFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
-                        csvOptions: {}
+                    super(...arguments), this._name = "Reddit Input", this._id = "redditInput", this._type = "pandas_df_input", this._category = "input", this._icon = S, this._default = {
+                        submission: "all",
+                        limit: 20,
+                        sort: "hot",
+                        userAgent: "Sumbission extraction by Amphi"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "File path",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: "\\.(csv|tsv|txt)$",
-                            validationMessage: "This field expects a file with a csv, tsv or txt extension such as output.csv."
+                            type: "input",
+                            label: "Submission",
+                            id: "submission",
+                            placeholder: "URL or id"
                         }, {
-                            type: "datalist",
-                            label: "Separator",
-                            id: "csvOptions.sep",
-                            placeholder: "auto",
-                            options: [{
-                                key: "comma",
-                                value: ",",
-                                text: "comma (,)"
-                            }, {
-                                key: "semicolon",
-                                value: ";",
-                                text: "semicolon (;)"
-                            }, {
-                                key: "space",
-                                value: " ",
-                                text: "space"
-                            }, {
-                                key: "tab",
-                                value: "  ",
-                                text: "tab"
-                            }, {
-                                key: "pipe",
-                                value: "|",
-                                text: "pipe (|)"
-                            }]
+                            type: "input",
+                            label: "Limit",
+                            id: "limit",
+                            placeholder: "Number of posts to fetch",
+                            advanced: !0
                         }, {
-                            type: "radio",
-                            label: "Mode",
-                            id: "csvOptions.mode",
-                            options: [{
-                                key: "w",
-                                value: "w",
-                                text: "Write"
-                            }, {
-                                key: "x",
-                                value: "x",
-                                text: "Exclusive Creation"
-                            }, {
-                                key: "a",
-                                value: "a",
-                                text: "Append"
-                            }],
+                            type: "input",
+                            label: "Client ID",
+                            id: "clientId",
+                            placeholder: "Reddit Client ID",
                             advanced: !0
                         }, {
-                            type: "boolean",
-                            label: "Header",
-                            id: "csvOptions.header",
+                            type: "input",
+                            label: "Secret ID",
+                            id: "secretId",
+                            placeholder: "Reddit Secret ID",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "User Agent",
+                            id: "userAgent",
+                            placeholder: "Sumbission extraction by username",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ue.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: _e.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ue.Name,
-                        ConfigForm: ue.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: _e.Name,
+                        ConfigForm: _e.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ue.Icon,
+                        Icon: _e.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd"]
+                    return ["import pandas as pd", "import praw", "from praw.models import MoreComments"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    outputName: t
                 }) {
-                    let n = Object.entries(e.csvOptions).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
-                    return n = n ? `, ${n}` : "", `\n${t}.to_csv('${e.filePath}', index=False${n})\n`
+                    const n = e.submission,
+                        o = e.limit || 10,
+                        a = n.startsWith("http") || n.startsWith("www") ? `${t}_submission = ${t}_reddit.submission(url='${n}')` : `${t}_submission = ${t}_reddit.submission('${n}')`;
+                    return `\n${t}_reddit = praw.Reddit(client_id='${e.clientId}', client_secret='${e.secretId}', user_agent='${e.userAgent}')\n${a}\n\n${t}_comments_data = []\n${t}_submission.comments.replace_more(limit=${o})\nfor comment in ${t}_submission.comments.list():\n    ${t}_comments_data.append({\n        'comment_id': comment.id,\n        'comment_body': comment.body,\n        'comment_author': comment.author.name if comment.author else None,\n        'comment_score': comment.score,\n        'comment_created_utc': comment.created_utc,\n        'parent_id': comment.parent_id\n    })\n\n${t} = pd.DataFrame(${t}_comments_data)\n`
                 }
             }
-            D = ue, ue.ConfigForm = ({
+            U = _e, _e.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = D.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = U.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: D.Type,
-                    name: D.Name,
-                    form: D.Form,
+                    type: U.Type,
+                    name: U.Name,
+                    form: U.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class he extends((0, a.PipelineComponent)()) {
+            class ye extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "JSON File Output", this._id = "jsonFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
-                        jsonOptions: {
-                            orient: "records"
+                    super(...arguments), this._name = "Schema Modeler", this._id = "schemaModeler", this._type = "pandas_df_processor", this._category = "transform", this._icon = $, this._default = {
+                        mapping: {
+                            sourceData: [],
+                            targetKeys: []
                         }
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "File path",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: ".(json|jsonl)$",
-                            validationMessage: "This field expects a file with a json or jsonl extension such as output.json."
-                        }, {
-                            type: "singleInputSelect",
-                            label: "Orientation",
-                            id: "jsonOptions.orient",
-                            placeholder: "default: columns",
-                            options: [{
-                                value: "null",
-                                label: "Select orientation",
-                                isDisabled: !0
-                            }, {
-                                value: "columns",
-                                label: "columns (JSON object with column labels as keys)"
-                            }, {
-                                value: "records",
-                                label: "records (List of rows as JSON objects)"
-                            }, {
-                                value: "index",
-                                label: "index (Dict with index labels as keys)"
-                            }, {
-                                value: "split",
-                                label: "split (Dict with 'index', 'columns', and 'data' keys)"
-                            }, {
-                                value: "table",
-                                label: "table (Dict with 'schema' and 'data' keys, following the Table Schema)"
-                            }]
+                            type: "transferData",
+                            label: "Mapping",
+                            id: "mapping",
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: he.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ye.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: he.Name,
-                        ConfigForm: he.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ye.Name,
+                        ConfigForm: ye.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: he.Icon,
+                        Icon: ye.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    let n = Object.entries(e.jsonOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
-                    const a = n ? `, ${n}` : "";
-                    return `\n${t}.to_json('${e.filePath}'${a})\n`
+                    return `\n# Schema modeling (filtering and ordering)\n${n} = ${t}[[${e.mapping.targetKeys.map((e=>`'${e.trim()}'`)).join(", ")}]]\n`
                 }
             }
-            A = he, he.ConfigForm = ({
+            L = ye, ye.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = A.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = L.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: A.Type,
-                    name: A.Name,
-                    form: A.Form,
+                    type: L.Type,
+                    name: L.Name,
+                    form: L.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ge extends((0, a.PipelineComponent)()) {
+            class xe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Excel File Output", this._id = "excelFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
-                        excelOptions: {}
-                    }, this._form = {
+                    super(...arguments), this._name = "Rename Columns", this._id = "rename", this._type = "pandas_df_processor", this._category = "transform", this._icon = b, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "File path",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: "\\.(xlsx)$",
-                            validationMessage: "This field expects a file with a xlsx extension such as output.xlsx."
-                        }, {
-                            type: "input",
-                            label: "Sheet",
-                            id: "excelOptions.sheet",
-                            placeholder: "default: Sheet1"
+                            type: "keyvalueColumns",
+                            label: "Columns",
+                            id: "columns",
+                            placeholders: {
+                                key: "column name",
+                                value: "new column name"
+                            },
+                            advanced: !0
                         }, {
-                            type: "radio",
-                            label: "Mode",
-                            id: "mode",
-                            options: [{
-                                key: "write",
-                                value: "WRITE",
-                                text: "WRITE",
-                                selected: !0
-                            }, {
-                                key: "append",
-                                value: "APPEND",
-                                text: "APPEND"
-                            }],
+                            type: "boolean",
+                            label: "Numeric indexes",
+                            id: "indexes",
+                            placeholder: "false",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ge.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: xe.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ge.Name,
-                        ConfigForm: ge.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: xe.Name,
+                        ConfigForm: xe.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ge.Icon,
+                        Icon: xe.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    let n = {
-                        ...e.excelOptions
-                    };
-                    const a = "['https://spreadsheets.google.com/feeds','https://www.googleapis.com/auth/drive']",
-                        o = `ServiceAccountCredentials.from_json_keyfile_name(${e.filePath?`'${e.filePath}'`:"None"}, ${a})`,
-                        s = `gspread.authorize(${o})`,
-                        r = `open_by_key(${n.spreadsheetId?`'${n.spreadsheetId}'`:"None"})`,
-                        d = `.worksheet(${n.range?`'${n.range.split("!")[0]}'`:"None"})`,
-                        l = `${t}Client`,
-                        i = `${t}Sheet`;
-                    let m;
-                    return m = "APPEND" === e.mode ? `${i}.append_rows(${t}.values.tolist(), value_input_option='RAW', insert_data_option='INSERT_ROWS', table_range='${n.range}')` : `${i}.update([${t}.columns.values.tolist()] + ${t}.values.tolist())`, `\n# Setting up the Google Sheets client\nscope = ${a}\ncreds = ${o}\n${l} = ${s}\n\n# Opening the spreadsheet and selecting the correct worksheet\n${i} = ${l}.${r}.${d}\n\n# Performing the selected operation on the sheet\n${m}\n`
+                    const o = e.indexes;
+                    let a = "";
+                    return e.columns && e.columns.length > 0 && (a = o ? "columns={" + e.columns.map((e => `${e.key}: '${e.value}'`)).join(", ") + "}" : "columns={" + e.columns.map((e => `'${e.key}': '${e.value}'`)).join(", ") + "}"), `\n# Rename columns\n${n} = ${t}.rename(${a})\n`
                 }
             }
-            M = ge, ge.ConfigForm = ({
+            j = xe, xe.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = M.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = j.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: M.Type,
-                    name: M.Name,
-                    form: M.Form,
+                    type: j.Type,
+                    name: j.Name,
+                    form: j.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class fe extends((0, a.PipelineComponent)()) {
+            class we extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Parquet File Output", this._id = "parquetFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Filter Rows", this._id = "filter", this._type = "pandas_df_processor", this._category = "transform", this._icon = g, this._default = {
+                        condition: "=="
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "File path",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: "\\.(parquet)$",
-                            validationMessage: "This field expects a file with a .parquet extension such as output.parquet."
+                            type: "column",
+                            label: "Column name",
+                            id: "columnName",
+                            placeholder: "Column name"
                         }, {
-                            type: "radio",
-                            label: "Compression",
-                            id: "parquetOptions.compression",
+                            type: "select",
+                            label: "Condition",
+                            id: "condition",
+                            placeholder: "Select condition",
                             options: [{
-                                key: "snappy",
-                                value: "snappy",
-                                text: "Snappy",
-                                selected: !0
+                                value: "==",
+                                label: "=="
                             }, {
-                                key: "gzip",
-                                value: "gzip",
-                                text: "GZip"
+                                value: "!=",
+                                label: "!="
                             }, {
-                                key: "brotli",
-                                value: "brotli",
-                                text: "Brotli"
+                                value: ">",
+                                label: ">"
                             }, {
-                                key: "none",
-                                value: "None",
-                                text: "None"
-                            }],
+                                value: "<",
+                                label: "<"
+                            }, {
+                                value: ">=",
+                                label: ">="
+                            }, {
+                                value: "<=",
+                                label: "<="
+                            }, {
+                                value: "notnull",
+                                label: "Not Null"
+                            }, {
+                                value: "notempty",
+                                label: "Not Empty"
+                            }, {
+                                value: "contains",
+                                label: "Contains (string)"
+                            }, {
+                                value: "not contains",
+                                label: "Not contains (string)"
+                            }, {
+                                value: "startswith",
+                                label: "Starts With (string)"
+                            }, {
+                                value: "endswith",
+                                label: "Ends With (string)"
+                            }, {
+                                value: "is NaN",
+                                label: "Is Not a Number (Leave value field empty)"
+                            }, {
+                                value: "is not N",
+                                label: "Is a Number (Leave value field empty)"
+                            }]
+                        }, {
+                            type: "input",
+                            label: "Value",
+                            id: "conditionValue",
+                            placeholder: "Any string of characters (enforce numbers if needed)"
+                        }, {
+                            type: "boolean",
+                            label: "Enforce value as string",
+                            id: "enforceString",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: fe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: we.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: fe.Name,
-                        ConfigForm: fe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: we.Name,
+                        ConfigForm: we.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: fe.Icon,
+                        Icon: we.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    let n = Object.entries(e.parquetOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
-                    return n = n ? `, ${n}` : "", `\n${t}.to_parquet('${e.filePath}'${n})\n`
+                    const o = e.columnName,
+                        a = e.condition,
+                        s = e.conditionValue;
+                    let r, d;
+                    switch (r = e.enforceNumber || isNaN(Number(s)) ? `'${s.toString().replace(/'/g,"\\'")}'` : s.toString(), a) {
+                        case "==":
+                        case "!=":
+                        default:
+                            d = `\`${o}\` ${a} ${r}`;
+                            break;
+                        case "contains":
+                            d = `\`${o}\`.str.contains(${r})`;
+                            break;
+                        case "not contains":
+                            d = `~\`${o}\`.str.contains(${r})`;
+                            break;
+                        case "startswith":
+                        case "endswith":
+                            d = `\`${o}\`.str.${a}(${r})`;
+                            break;
+                        case "isna":
+                        case "notna":
+                            d = `\`${o}\`.${a}()`
+                    }
+                    return `\n# Filter rows\n${n} = ${t}.query("${d}")\n`
                 }
             }
-            U = fe, fe.ConfigForm = ({
+            R = we, we.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = U.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = R.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: U.Type,
-                    name: U.Name,
-                    form: U.Form,
+                    type: R.Type,
+                    name: R.Name,
+                    form: R.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Ce extends((0, a.PipelineComponent)()) {
+            class Ne extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "XML File Output", this._id = "xmlFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Aggregate", this._id = "aggregate", this._type = "pandas_df_processor", this._icon = h, this._category = "transform", this._default = {
+                        csvOptions: {
+                            header: "infer"
+                        }
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "File path",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: "\\.xml$",
-                            validationMessage: "This field expects a file with an xml extension such as output.xml."
+                            type: "columns",
+                            label: "Columns to group by",
+                            id: "groupColumn",
+                            placeholder: "Select columns"
+                        }, {
+                            type: "columns",
+                            label: "Columns to apply operation",
+                            id: "aggColumns",
+                            placeholder: "column(s) name"
+                        }, {
+                            type: "select",
+                            label: "Operation function(s)",
+                            id: "aggFunctions",
+                            placeholder: "Select function(s) (comma separated for multiple functions",
+                            options: [{
+                                key: "min",
+                                value: "min",
+                                text: "Minimum of each group"
+                            }, {
+                                key: "max",
+                                value: "max",
+                                text: "Maximum of each group"
+                            }, {
+                                key: "sum",
+                                value: "sum",
+                                text: "Sum of each group"
+                            }, {
+                                key: "count",
+                                value: "count",
+                                text: "Count of each group"
+                            }, {
+                                key: "mean",
+                                value: "mean",
+                                text: "Mean"
+                            }, {
+                                key: "minmaxsummin",
+                                value: "min, max, sum, mean",
+                                text: "Multiple functions example"
+                            }]
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Ce.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ne.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Ce.Name,
-                        ConfigForm: Ce.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ne.Name,
+                        ConfigForm: Ne.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Ce.Icon,
+                        Icon: Ne.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import xml.etree.ElementTree as ET", "import pandas as pd"]
+                    return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    const n = `${t}_xml_output`,
-                        a = `${t}_file`;
-                    return `\n# Output the XML content to a file\n${n} = ${t}.to_xml()\nwith open('${e.filePath}', 'w') as ${a}:\n    ${a}.write(${n})\n`
+                    const o = e.groupColumn.split(",").map((e => e.trim())),
+                        a = e.aggColumns.split(",").map((e => e.trim())),
+                        s = e.aggFunctions.split(",").map((e => e.trim()));
+                    let r = {};
+                    a.forEach(((e, t) => {
+                        r[e] = s[t]
+                    }));
+                    let d = `\n${n} = ${t}.groupby([`;
+                    return o.forEach((e => {
+                        d += `\n'${e}',`
+                    })), d += `\n]).agg(${JSON.stringify(r)}).reset_index()\n`, d
                 }
             }
-            z = Ce, Ce.ConfigForm = ({
+            q = Ne, Ne.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = z.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = q.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: z.Type,
-                    name: z.Name,
-                    form: z.Form,
+                    type: q.Type,
+                    name: q.Name,
+                    form: q.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ve extends((0, a.PipelineComponent)()) {
+            class Fe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "G. Sheets Output", this._id = "googleSheetsOutput", this._type = "pandas_df_output", this._category = "output", this._icon = b, this._default = {
-                        sheetOptions: {
-                            spreadsheetId: "",
-                            range: "Sheet1"
-                        }
+                    super(...arguments), this._name = "Join Datasets", this._id = "join", this._type = "pandas_df_double_processor", this._category = "transform", this._icon = f, this._default = {
+                        condition: "=="
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "file",
-                            label: "Service Account Key",
-                            id: "filePath",
-                            placeholder: "Type file name",
-                            validation: "\\.(json)$",
-                            validationMessage: "This field expects a file with a .json extension such as your-service-account-file.json."
-                        }, {
-                            type: "input",
-                            label: "Spreadsheet ID",
-                            id: "sheetOptions.spreadsheetId",
-                            placeholder: "Enter Google Sheets' name or ID",
-                            validation: "^[a-zA-Z0-9-_]+$",
-                            validationMessage: "Invalid Spreadsheet ID."
-                        }, {
-                            type: "input",
-                            label: "Range",
-                            id: "sheetOptions.range",
-                            placeholder: "e.g., Sheet1 or Sheet1!A1:D5",
-                            validation: "^[a-zA-Z0-9-_!]+$",
-                            validationMessage: "Invalid Range."
-                        }, {
-                            type: "",
-                            label: "Range",
-                            id: "sheetOptions.range",
-                            placeholder: "e.g., Sheet1 or Sheet1!A1:D5",
-                            validation: "^[a-zA-Z0-9-_!]+$",
-                            validationMessage: "Invalid Range."
+                            type: "column",
+                            label: "First Input Column",
+                            id: "leftKeyColumn",
+                            placeholder: "Column name",
+                            inputNb: 1
+                        }, {
+                            type: "column",
+                            label: "Second Input Column",
+                            id: "rightKeyColumn",
+                            placeholder: "Column name",
+                            inputNb: 2
+                        }, {
+                            type: "select",
+                            label: "Join type",
+                            id: "how",
+                            placeholder: "Default: Inner",
+                            options: [{
+                                value: "inner",
+                                label: "Inner: return only the rows with matching keys in both data frames (intersection)."
+                            }, {
+                                value: "left",
+                                label: "Left: return all rows from the left data frame and matched rows from the right data frame (including NaN for no match)."
+                            }, {
+                                value: "right",
+                                label: "Right: return all rows from the right data frame and matched rows from the left data frame (including NaN for no match)."
+                            }, {
+                                value: "outer",
+                                label: "Outer: return all rows from both data frames, with matches where available and NaN for no match (union)."
+                            }],
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ve.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Fe.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ve.Name,
-                        ConfigForm: ve.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Fe.Name,
+                        ConfigForm: Fe.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ve.Icon,
+                        Icon: Fe.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd", "import gspread", "from oauth2client.service_account import ServiceAccountCredentials"]
+                    return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName1: t,
+                    inputName2: n,
+                    outputName: o
                 }) {
-                    let n = {
-                        ...e.sheetOptions
-                    };
-                    const a = `${t}Client`,
-                        o = `${t}Sheet`;
-                    return `\n# Outputting data to Google Sheets\nscope = ['https://spreadsheets.google.com/feeds','https://www.googleapis.com/auth/drive']\ncreds = ServiceAccountCredentials.from_json_keyfile_name(${e.filePath?`'${e.filePath}'`:"None"}, scope)\n${a} = gspread.authorize(creds)\n\n# Open the spreadsheet and select the right worksheet\n${o} = ${a}.open_by_key(${n.spreadsheetId?`'${n.spreadsheetId}'`:"None"}).worksheet(${n.range?`'${n.range.split("!")[0]}'`:"None"})\n\n# Update the sheet with dataframe's data\n${o}.update([${t}.columns.values.tolist()] + ${t}.values.tolist())\n`
+                    const a = e.how ? `, how='${e.how}'` : "";
+                    return `\n# Merge two datasets\n${o} = pd.merge(${t}, ${n}, left_on='${e.leftKeyColumn}', right_on='${e.rightKeyColumn}'${a})\n`
                 }
             }
-            L = ve, ve.ConfigForm = ({
+            B = Fe, Fe.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = L.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = B.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: L.Type,
-                    name: L.Name,
-                    form: L.Form,
+                    type: B.Type,
+                    name: B.Name,
+                    form: B.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Ie extends((0, a.PipelineComponent)()) {
+            class Se extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "MySQL Output", this._id = "mySQLOutput", this._type = "pandas_df_output", this._category = "output", this._icon = N, this._default = {
-                        dbOptions: {
-                            host: "localhost",
-                            port: "3306",
-                            databaseName: "",
-                            tableName: "",
-                            username: "",
-                            password: ""
-                        }
+                    super(...arguments), this._name = "Type Converter", this._id = "typeConverter", this._type = "pandas_df_processor", this._category = "transform", this._icon = _, this._default = {
+                        dataType: "string"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Host",
-                            id: "dbOptions.host",
-                            placeholder: "Enter database host",
-                            advanced: !0
-                        }, {
-                            type: "input",
-                            label: "Port",
-                            id: "dbOptions.port",
-                            placeholder: "Enter database port",
-                            advanced: !0
-                        }, {
-                            type: "input",
-                            label: "Database Name",
-                            id: "dbOptions.databaseName",
-                            placeholder: "Enter database name"
-                        }, {
-                            type: "input",
-                            label: "Table Name",
-                            id: "dbOptions.tableName",
-                            placeholder: "Enter table name"
-                        }, {
-                            type: "input",
-                            label: "Username",
-                            id: "dbOptions.username",
-                            placeholder: "Enter username",
-                            advanced: !0
+                            type: "column",
+                            label: "Column name",
+                            id: "columnName",
+                            placeholder: "Column name"
                         }, {
-                            type: "input",
-                            label: "Password",
-                            id: "dbOptions.password",
-                            placeholder: "Enter password",
-                            advanced: !0
+                            type: "cascader",
+                            label: "Data Type to convert to",
+                            id: "dataType",
+                            placeholder: "Select column type to convert to",
+                            options: [{
+                                value: "numeric",
+                                label: "Numeric",
+                                children: [{
+                                    value: "int",
+                                    label: "Integer",
+                                    children: [{
+                                        value: "int64",
+                                        label: "int64: Standard integer type."
+                                    }, {
+                                        value: "int32",
+                                        label: "int32: For optimized memory usage."
+                                    }, {
+                                        value: "int16",
+                                        label: "int16: For more optimized memory usage."
+                                    }]
+                                }, {
+                                    value: "float",
+                                    label: "Float",
+                                    children: [{
+                                        value: "float64",
+                                        label: "float64: Standard floating-point type."
+                                    }, {
+                                        value: "float32",
+                                        label: "float32: For optimized memory usage."
+                                    }]
+                                }]
+                            }, {
+                                value: "datetime",
+                                label: "Datetime",
+                                children: [{
+                                    value: "datetime64[ns]",
+                                    label: "datetime64[ns]: For datetime values."
+                                }, {
+                                    value: "datetime64[ns, tz]",
+                                    label: "datetime64[ns, tz]: For datetime values with timezone."
+                                }, {
+                                    value: "datetime64[ms]",
+                                    label: "datetime64[ms]: For datetime values in milliseconds."
+                                }, {
+                                    value: "datetime64[s]",
+                                    label: "datetime64[s]: For datetime values in seconds."
+                                }, {
+                                    value: "datetime32[ns]",
+                                    label: "datetime32[ns]: For compact datetime storage in nanoseconds."
+                                }, {
+                                    value: "datetime32[ms]",
+                                    label: "datetime32[ms]: For compact datetime storage in milliseconds."
+                                }]
+                            }, {
+                                value: "timedelta",
+                                label: "Timedelta",
+                                children: [{
+                                    value: "timedelta[ns]",
+                                    label: "timedelta[ns]: For differences between two datetimes."
+                                }]
+                            }, {
+                                value: "boolean",
+                                label: "Boolean",
+                                children: [{
+                                    value: "bool",
+                                    label: "bool: For boolean values (True or False)."
+                                }]
+                            }, {
+                                value: "object",
+                                label: "Object",
+                                children: [{
+                                    value: "object",
+                                    label: "object: For generic objects (strings, timestamps, mixed types)."
+                                }]
+                            }, {
+                                value: "category",
+                                label: "Category",
+                                children: [{
+                                    value: "category",
+                                    label: "category: For categorical variables."
+                                }]
+                            }, {
+                                value: "string",
+                                label: "String",
+                                children: [{
+                                    value: "string",
+                                    label: "string: For string data."
+                                }]
+                            }]
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Ie.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Se.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Ie.Name,
-                        ConfigForm: Ie.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Se.Name,
+                        ConfigForm: Se.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Ie.Icon,
+                        Icon: Se.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd", "import sqlalchemy"]
+                    return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    const n = `${t}Engine`;
-                    return `\n# Connect to MySQL and output into table\n${n} = sqlalchemy.create_engine('mysql+pymysql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}')\n${t}.to_sql(name='${e.dbOptions.tableName}', con=${n}, if_exists='replace', index=False)\n`
+                    const {
+                        columnName: o,
+                        dataType: a
+                    } = e;
+                    return `\n# Convert ${o} to ${a}\n${n} = ${t}.assign(${o}=${t}['${o}'].astype('${a}'))\n`
                 }
             }
-            j = Ie, Ie.ConfigForm = ({
+            G = Se, Se.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = j.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = G.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: j.Type,
-                    name: j.Name,
-                    form: j.Form,
+                    type: G.Type,
+                    name: G.Name,
+                    form: G.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class xe extends((0, a.PipelineComponent)()) {
+            class $e extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Console", this._id = "console", this._type = "pandas_df_output", this._category = "output", this._icon = m, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Split Column", this._id = "splitColumn", this._type = "pandas_df_processor", this._category = "transform", this._icon = x, this._default = {
+                        keepOriginalColumn: !1
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Records limit",
-                            id: "limit",
-                            placeholder: "Number of records to print in console"
+                            type: "column",
+                            label: "Column",
+                            id: "column",
+                            placeholder: "Type column name"
+                        }, {
+                            type: "selectCustomizable",
+                            label: "Delimiter",
+                            id: "delimiter",
+                            placeholder: "Select or type delimiter",
+                            options: [{
+                                value: ",",
+                                label: "comma (,)"
+                            }, {
+                                value: ";",
+                                label: "semicolon (;)"
+                            }, {
+                                value: " ",
+                                label: "space"
+                            }, {
+                                value: "  ",
+                                label: "tab"
+                            }, {
+                                value: "|",
+                                label: "pipe (|)"
+                            }]
+                        }, {
+                            type: "selectTokenization",
+                            label: "Column names",
+                            id: "columnNames",
+                            placeholder: "Optional: provide names for created columns",
+                            advanced: !0
+                        }, {
+                            type: "boolean",
+                            label: "Keep original column",
+                            id: "keepOriginalColumn",
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: xe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: $e.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: xe.Name,
-                        ConfigForm: xe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: $e.Name,
+                        ConfigForm: $e.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: xe.Icon,
+                        Icon: $e.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t
+                    inputName: t,
+                    outputName: n
                 }) {
-                    return e.limit && (t += `.head(${e.limit})`), `\nprint(${t})\n`
+                    const o = `${n}_split`,
+                        a = `${n}_combined`;
+                    let s = "\n# Create a new DataFrame from the split operation\n";
+                    return s += `${o} = ${t}['${e.column}'].str.split('${e.delimiter}', expand=True)\n`, e.columnNames && e.columnNames.length > 0 && (s += "\n# Rename columns\n", s += `${o}.columns = ['${e.columnNames.map((e=>e.trim())).join("', '")}']\n`), s += "\n# Combine original DataFrame with the new temporary split DataFrame\n", s += `${a} = ${t}.join(${o})\n`, e.keepOriginalColumn ? s += `${n} = ${a}\n` : (s += "\n# Remove the original column used for split if required\n", s += `${n} = ${a}.drop(columns=['${e.column}'])\n`), s
                 }
             }
-            R = xe, xe.ConfigForm = ({
+            J = $e, $e.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = R.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = J.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: R.Type,
-                    name: R.Name,
-                    form: R.Form,
+                    type: J.Type,
+                    name: J.Name,
+                    form: J.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ye extends((0, a.PipelineComponent)()) {
+            class Ee extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Filter", this._id = "filter", this._type = "pandas_df_processor", this._category = "transform", this._icon = h, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Extract", this._id = "extract", this._type = "pandas_df_processor", this._category = "transform", this._icon = y, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
+                            type: "column",
                             label: "Column name",
                             id: "columnName",
                             placeholder: "Column name"
                         }, {
-                            type: "singleInputSelect",
-                            label: "Condition",
-                            id: "condition",
-                            placeholder: "Select condition",
+                            type: "selectCustomizable",
+                            label: "Regular Expression",
+                            id: "regex",
+                            tooltip: "Select of a type of data or add a custom regex",
+                            placeholder: "Select type or type regex",
                             options: [{
-                                value: "==",
-                                label: "Equals"
+                                value: "(\\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\\.[A-Z|a-z]{2,}\\b)",
+                                label: "Email"
                             }, {
-                                value: "!=",
-                                label: "Not Equals"
+                                value: "(https?://(?:www\\.)?[-a-zA-Z0-9@:%._\\+~#=]{2,256}\\.[a-z]{2,6}\\b(?:[-a-zA-Z0-9@:%_\\+.~#?&//=]*))",
+                                label: "URL"
                             }, {
-                                value: ">",
-                                label: "Greater Than (for numbers)"
+                                value: "(\\b\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\b)",
+                                label: "IPv4 Address"
                             }, {
-                                value: "<",
-                                label: "Less Than (for numbers)"
+                                value: "(([0-9a-fA-F]{1,4}:){7,7}[0-9a-fA-F]{1,4}|([0-9a-fA-F]{1,4}:){1,7}:|([0-9a-fA-F]{1,4}:){1,6}:[0-9a-fA-F]{1,4})",
+                                label: "IPv6 Address"
                             }, {
-                                value: ">=",
-                                label: "Greater Than or Equal To (numbers)"
+                                value: "(\\b\\d{4}[- ]?\\d{4}[- ]?\\d{4}[- ]?\\d{4}\\b)",
+                                label: "Credit Card"
                             }, {
-                                value: "<=",
-                                label: "Less Than or Equal To (numbers)"
+                                value: "(\\b\\d{3}-\\d{2}-\\d{4}\\b)",
+                                label: "SSN"
                             }, {
-                                value: "notnull",
-                                label: "Not Null"
+                                value: "(\\b\\d{1,3}(\\.\\d{1,2})?%\\b)",
+                                label: "Percentage"
                             }, {
-                                value: "notempty",
-                                label: "Not Empty"
+                                value: '("([^"\\\\]*(\\\\.[^"\\\\]*)*))',
+                                label: "JSON String"
                             }, {
-                                value: "contains",
-                                label: "Contains (string)"
+                                value: "(\\b\\d{3}-\\d{10}\\b)",
+                                label: "ISBN"
+                            }]
+                        }, {
+                            type: "select",
+                            label: "Flags",
+                            id: "flags",
+                            placeholder: "Type or select",
+                            options: [{
+                                value: "IGNORECASE",
+                                label: "Makes the match case-insensitive. For example, it will match both 'abc' and 'ABC'."
                             }, {
-                                value: "not contains",
-                                label: "Not contains (string)"
+                                value: "MULTILINE",
+                                label: "Changes the behavior of ^ and $ to match the start and end of each line, not just the start and end of the whole string."
                             }, {
-                                value: "startswith",
-                                label: "Starts With (string)"
+                                value: "DOTALL",
+                                label: "Makes the . match any character at all, including a newline; without this flag, . will match anything except a newline."
                             }, {
-                                value: "endswith",
-                                label: "Ends With (string)"
+                                value: "UNICODE",
+                                label: "Makes \\w, \\W, \\b, \\B, \\d, \\D, \\s, and \\S sequences dependent on the Unicode character properties database. This is the default behavior in Python 3 for strings."
                             }, {
-                                value: "is NaN",
-                                label: "Is Not a Number (Leave value field empty)"
+                                value: "ASCII",
+                                label: "Makes \\w, \\W, \\b, \\B, \\d, \\D, \\s, and \\S perform ASCII-only matching instead of full Unicode matching."
                             }, {
-                                value: "is not N",
-                                label: "Is a Number (Leave value field empty)"
+                                value: "VERBOSE",
+                                label: "Allows you to write regular expressions that are more readable by permitting whitespace and comments within the pattern string."
+                            }],
+                            advanced: !0
+                        }]
+                    }
+                }
+                UIComponent({
+                    id: e,
+                    data: t,
+                    context: n,
+                    componentService: d,
+                    manager: l,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
                             }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ee.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: C
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: t,
+                        context: n,
+                        manager: l,
+                        commands: i,
+                        name: Ee.Name,
+                        ConfigForm: Ee.ConfigForm({
+                            nodeId: e,
+                            data: t,
+                            context: n,
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: Ee.Icon,
+                        showContent: h,
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import pandas as pd", "import re"]
+                }
+                generateComponentCode({
+                    config: e,
+                    inputName: t,
+                    outputName: n
+                }) {
+                    const o = e.columnName,
+                        a = e.regex;
+                    let s = "";
+                    e.falgs && "" !== e.flags.trim() && (s = `, flags=${e.flags.split(",").filter((e=>""!==e.trim())).map((e=>`re.${e}`)).join(" | ")}`);
+                    const r = new RegExp(a + "|").exec("").length - 1,
+                        d = Array.from({
+                            length: r
+                        }, ((e, t) => `'${n}_${t+1}'`)).join(", "),
+                        l = `${n}_extracted`;
+                    return `\n# Extract data using regex\n${l} = ${t}['${o}'].str.extract(r'${a}'${s})\n${l}.columns = [${d}]\n${n} = ${t}.join(${l}, rsuffix='_extracted')\n`
+                }
+            }
+            Q = Ee, Ee.ConfigForm = ({
+                nodeId: e,
+                data: t,
+                context: n,
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = Q.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
+                        evtTargetValue: t,
+                        field: n,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: Q.Type,
+                    name: Q.Name,
+                    form: Q.Form,
+                    data: t,
+                    context: n,
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
+                }))
+            };
+            class Pe extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Sort", this._id = "sort", this._type = "pandas_df_processor", this._category = "transform", this._icon = I, this._default = {
+                        order: "True"
+                    }, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "columns",
+                            label: "Columns",
+                            id: "by",
+                            placeholder: "Column names"
                         }, {
-                            type: "input",
-                            label: "Value the condition satisfies",
-                            id: "conditionValue",
-                            placeholder: "Any string of characters (enforce numbers if needed)"
+                            type: "radio",
+                            label: "Order",
+                            id: "order",
+                            options: [{
+                                value: "True",
+                                label: "Asc."
+                            }, {
+                                value: "False",
+                                label: "Desc."
+                            }]
                         }, {
                             type: "boolean",
-                            label: "Enforce value as number",
-                            id: "enforceNumber",
+                            label: "Ignore Index",
+                            id: "ignoreIndex",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
+                    componentService: d,
+                    manager: l,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Pe.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: C
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: t,
+                        context: n,
+                        manager: l,
+                        commands: i,
+                        name: Pe.Name,
+                        ConfigForm: Pe.ConfigForm({
+                            nodeId: e,
+                            data: t,
+                            context: n,
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: Pe.Icon,
+                        showContent: h,
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import pandas as pd"]
+                }
+                generateComponentCode({
+                    config: e,
+                    inputName: t,
+                    outputName: n
+                }) {
+                    return `${n} = ${t}.sort_values(${e.by?`by=[${e.by.map((e=>`'${e.trim()}'`)).join(", ")}]`:""}${void 0!==e.order?`, ascending=${e.order}`:""}${e.ignoreIndex?`, ignore_index=${e.ignoreIndex}`:""})`
+                }
+            }
+            W = Pe, Pe.ConfigForm = ({
+                nodeId: e,
+                data: t,
+                context: n,
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = W.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
+                        evtTargetValue: t,
+                        field: n,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: W.Type,
+                    name: W.Name,
+                    form: W.Form,
+                    data: t,
+                    context: n,
+                    componentService: r,
                     manager: d,
-                    commands: l
+                    commands: l,
+                    handleChange: u
+                }))
+            };
+            class Te extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Deduplicate", this._id = "deduplicateData", this._type = "pandas_df_processor", this._category = "transform", this._icon = C, this._default = {
+                        keep: "first"
+                    }, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "select",
+                            label: "Keep (survivorship)",
+                            id: "keep",
+                            options: [{
+                                value: "first",
+                                label: "Drop duplicates except for the first occurrence"
+                            }, {
+                                value: "last",
+                                label: "Drop duplicates except for the last occurrence"
+                            }, {
+                                value: !1,
+                                label: "Drop all duplicates"
+                            }]
+                        }, {
+                            type: "columns",
+                            label: "Columns",
+                            id: "subset",
+                            placeholder: "All columns",
+                            tooltip: "Columns considered for identifying duplicates"
+                        }]
+                    }
+                }
+                UIComponent({
+                    id: e,
+                    data: t,
+                    context: n,
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ye.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Te.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ye.Name,
-                        ConfigForm: ye.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Te.Name,
+                        ConfigForm: Te.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ye.Icon,
+                        Icon: Te.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
                     inputName: t,
                     outputName: n
                 }) {
-                    const a = e.columnName,
-                        o = e.condition,
-                        s = e.conditionValue,
-                        r = e.enforceNumber ? s : `'${s}'`;
-                    let d;
-                    switch (o) {
-                        case "==":
-                        case "!=":
-                        default:
-                            d = `\`${a}\` ${o} ${r}`;
-                            break;
-                        case "contains":
-                            d = `\`${a}\`.str.contains(${r})`;
-                            break;
-                        case "not contains":
-                            d = `~\`${a}\`.str.contains(${r})`;
-                            break;
-                        case "startswith":
-                        case "endswith":
-                            d = `\`${a}\`.str.${o}(${r})`;
-                            break;
-                        case "isna":
-                        case "notna":
-                            d = `\`${a}\`.${o}()`
+                    let o = "# Deduplicate\n";
+                    return o += `${n} = ${t}.drop_duplicates(${e.columns.length>0?`subset=[${e.columns.map((e=>`'${e.trim()}'`)).join(", ")}], `:""}keep=${e.keepFirst?"'first'":"'last'"})\n`, o
+                }
+            }
+            K = Te, Te.ConfigForm = ({
+                nodeId: e,
+                data: t,
+                context: n,
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
+            }) => {
+                const c = K.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
+                        evtTargetValue: t,
+                        field: n,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: K.Type,
+                    name: K.Name,
+                    form: K.Form,
+                    data: t,
+                    context: n,
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
+                }))
+            };
+            class ke extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Expand JSON List", this._id = "expandList", this._type = "pandas_df_processor", this._category = "transform", this._icon = v, this._default = {}, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "column",
+                            label: "Column",
+                            id: "column",
+                            placeholder: "Select column"
+                        }]
                     }
-                    return `\n# Filter rows\n${n} = ${t}.query("${d}")\n`
+                }
+                UIComponent({
+                    id: e,
+                    data: t,
+                    context: n,
+                    componentService: d,
+                    manager: l,
+                    commands: i
+                }) {
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ke.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: C
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
+                        data: t,
+                        context: n,
+                        manager: l,
+                        commands: i,
+                        name: ke.Name,
+                        ConfigForm: ke.ConfigForm({
+                            nodeId: e,
+                            data: t,
+                            context: n,
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: ke.Icon,
+                        showContent: h,
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import pandas as pd"]
+                }
+                generateComponentCode({
+                    config: e,
+                    inputName: t,
+                    outputName: n
+                }) {
+                    let o = "# Expand the list in the specified column\n";
+                    return o += "import pandas as pd\n", o += `${n} = ${t}['${e.column}'].apply(pd.Series)\n`, o
                 }
             }
-            q = ye, ye.ConfigForm = ({
+            Z = ke, ke.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = q.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = Z.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: q.Type,
-                    name: q.Name,
-                    form: q.Form,
+                    type: Z.Type,
+                    name: Z.Name,
+                    form: Z.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class _e extends((0, a.PipelineComponent)()) {
+            class He extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Aggregate", this._id = "aggregate", this._type = "pandas_df_processor", this._icon = g, this._category = "transform", this._default = {
-                        csvOptions: {
-                            header: "infer"
-                        }
+                    super(...arguments), this._name = "Sample", this._id = "sample", this._type = "pandas_df_processor", this._category = "transform", this._icon = E, this._default = {
+                        mode: "random"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Column(s) to group by",
-                            id: "groupColumn",
-                            placeholder: "column(s) name"
-                        }, {
-                            type: "input",
-                            label: "Column(s) to apply operation",
-                            id: "aggColumns",
-                            placeholder: "column(s) name"
+                            type: "inputNumber",
+                            label: "Rows number",
+                            id: "rows",
+                            placeholder: "0",
+                            min: 0
                         }, {
-                            type: "datalist",
-                            label: "Operation function(s)",
-                            id: "aggFunctions",
-                            placeholder: "Select function(s) (comma separated for multiple functions",
+                            type: "radio",
+                            label: "Mode",
+                            id: "mode",
                             options: [{
-                                key: "min",
-                                value: "min",
-                                text: "Minimum of each group"
-                            }, {
-                                key: "max",
-                                value: "max",
-                                text: "Maximum of each group"
-                            }, {
-                                key: "sum",
-                                value: "sum",
-                                text: "Sum of each group"
-                            }, {
-                                key: "count",
-                                value: "count",
-                                text: "Count of each group"
+                                value: "random",
+                                label: "Random"
                             }, {
-                                key: "mean",
-                                value: "mean",
-                                text: "Mean"
+                                value: "head",
+                                label: "First"
                             }, {
-                                key: "minmaxsummin",
-                                value: "min, max, sum, mean",
-                                text: "Multiple functions example"
-                            }]
+                                value: "tail",
+                                label: "Last"
+                            }],
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: _e.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: He.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: _e.Name,
-                        ConfigForm: _e.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: He.Name,
+                        ConfigForm: He.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: _e.Icon,
+                        Icon: He.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
                     inputName: t,
                     outputName: n
                 }) {
-                    const a = e.groupColumn.split(",").map((e => e.trim())),
-                        o = e.aggColumns.split(",").map((e => e.trim())),
-                        s = e.aggFunctions.split(",").map((e => e.trim()));
-                    let r = {};
-                    o.forEach(((e, t) => {
-                        r[e] = s[t]
-                    }));
-                    let d = `\n${n} = ${t}.groupby([`;
-                    return a.forEach((e => {
-                        d += `\n'${e}',`
-                    })), d += `\n]).agg(${JSON.stringify(r)}).reset_index()\n`, d
+                    let o = "";
+                    return "random" === e.mode ? o = `${n} = ${t}.sample(n=${e.rows})` : "tail" === e.mode ? o = `${n} = ${t}.tail(${e.rows})` : "head" === e.mode && (o = `${n} = ${t}.head(${e.rows})`), `\n${o}\n  `
                 }
             }
-            B = _e, _e.ConfigForm = ({
+            X = He, He.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = B.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = X.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: B.Type,
-                    name: B.Name,
-                    form: B.Form,
+                    type: X.Type,
+                    name: X.Name,
+                    form: X.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class be extends((0, a.PipelineComponent)()) {
+            class Ae extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "SQL Query", this._id = "sqlQuery", this._type = "pandas_df_processor", this._category = "transform", this._icon = w, this._default = {
+                    super(...arguments), this._name = "SQL Query", this._id = "sqlQuery", this._type = "pandas_df_processor", this._category = "transform", this._icon = F, this._default = {
                         query: "SELECT * FROM input_df1"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "textarea",
                             label: "SQL",
                             id: "query",
@@ -2987,53 +3805,66 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: be.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ae.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: be.Name,
-                        ConfigForm: be.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ae.Name,
+                        ConfigForm: Ae.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: be.Icon,
+                        Icon: Ae.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd", "import duckdb"]
                 }
@@ -3041,57 +3872,59 @@
                     config: e,
                     inputName: t,
                     outputName: n
                 }) {
                     return `\n# Execute SQL Query using DuckDB\n${n} = duckdb.query("${e.query.replace("input_df1",t)}").to_df()\n`
                 }
             }
-            G = be, be.ConfigForm = ({
+            Y = Ae, Ae.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = G.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = Y.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: G.Type,
-                    name: G.Name,
-                    form: G.Form,
+                    type: Y.Type,
+                    name: Y.Name,
+                    form: Y.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Ne extends((0, a.PipelineComponent)()) {
+            class Ve extends((0, o.PipelineComponent)()) {
                 constructor() {
                     super(...arguments), this._name = "Custom Code", this._id = "customTransformations", this._type = "pandas_df_processor", this._category = "transform", this._icon = u, this._default = {
                         code: "output = input"
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "textarea",
@@ -3107,130 +3940,143 @@
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Ne.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ve.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Ne.Name,
-                        ConfigForm: Ne.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ve.Name,
+                        ConfigForm: Ve.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Ne.Icon,
+                        Icon: Ve.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports(e) {
                     return e.imports ? e.imports.split("\n").filter((e => e.startsWith("import "))) : []
                 }
                 generateComponentCode({
                     config: e,
                     inputName: t,
                     outputName: n
                 }) {
-                    let a = `\n${e.code}`.replace(/input/g, t);
-                    return a = a.replace(/output/g, n), a
+                    let o = `\n${e.code}`.replace(/input/g, t);
+                    return o = o.replace(/output/g, n), o
                 }
             }
-            Q = Ne, Ne.ConfigForm = ({
+            ee = Ve, Ve.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = Q.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = ee.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Q.Type,
-                    name: Q.Name,
-                    form: Q.Form,
+                    type: ee.Type,
+                    name: ee.Name,
+                    form: ee.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class we extends((0, a.PipelineComponent)()) {
+            class De extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Split Column", this._id = "splitColumn", this._type = "pandas_df_processor", this._category = "transform", this._icon = v, this._default = {
-                        keepOriginalColumn: !1
+                    super(...arguments), this._name = "CSV File Output", this._id = "csvFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
+                        csvOptions: {}
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Column",
-                            id: "column",
-                            placeholder: "Type column name"
+                            type: "file",
+                            label: "File path",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: "\\.(csv|tsv|txt)$",
+                            validationMessage: "This field expects a file with a csv, tsv or txt extension such as output.csv."
                         }, {
-                            type: "singleInputCreatableSelect",
-                            label: "Delimiter",
-                            id: "delimiter",
-                            placeholder: "Select or type delimiter",
+                            type: "selectCustomizable",
+                            label: "Separator",
+                            id: "csvOptions.sep",
+                            placeholder: "auto",
                             options: [{
-                                value: "null",
-                                label: "Select or type delimiter",
-                                isDisabled: !0
-                            }, {
                                 value: ",",
                                 label: "comma (,)"
                             }, {
                                 value: ";",
                                 label: "semicolon (;)"
                             }, {
                                 value: " ",
@@ -3239,1248 +4085,1586 @@
                                 value: "  ",
                                 label: "tab"
                             }, {
                                 value: "|",
                                 label: "pipe (|)"
                             }]
                         }, {
-                            type: "input",
-                            label: "Column names",
-                            id: "columnNames",
-                            placeholder: "Optional: comma separated",
+                            type: "radio",
+                            label: "Mode",
+                            id: "csvOptions.mode",
+                            options: [{
+                                value: "w",
+                                label: "Write"
+                            }, {
+                                value: "x",
+                                label: "Exclusive Creation"
+                            }, {
+                                value: "a",
+                                label: "Append"
+                            }],
                             advanced: !0
                         }, {
                             type: "boolean",
-                            label: "Keep original column",
-                            id: "keepOriginalColumn",
+                            label: "Header",
+                            id: "csvOptions.header",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: we.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: De.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: we.Name,
-                        ConfigForm: we.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: De.Name,
+                        ConfigForm: De.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: we.Icon,
+                        Icon: De.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    const a = `${n}_split`,
-                        o = `${n}_combined`;
-                    let s = "\n# Create a new DataFrame from the split operation\n";
-                    return s += `${a} = ${t}['${e.column}'].str.split('${e.delimiter}', expand=True)\n`, e.columnNames && (s += "\n# Rename columns\n", s += `${a}.columns = ['${e.columnNames.split(",").map((e=>e.trim())).join("', '")}']\n`), s += "\n# Combine original DataFrame with the new temporary split DataFrame\n", s += `${o} = ${t}.join(${a})\n`, e.keepOriginalColumn ? s += `${n} = ${o}\n` : (s += "\n# Remove the original column used for split if required\n", s += `${n} = ${o}.drop(columns=['${e.column}'])\n`), s
+                    let n = Object.entries(e.csvOptions).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
+                    return n = n ? `, ${n}` : "", `\n${t}.to_csv('${e.filePath}', index=False${n})\n`
                 }
             }
-            J = we, we.ConfigForm = ({
+            te = De, De.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = J.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = te.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: J.Type,
-                    name: J.Name,
-                    form: J.Form,
+                    type: te.Type,
+                    name: te.Name,
+                    form: te.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Fe extends((0, a.PipelineComponent)()) {
+            class Me extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Deduplicate", this._id = "deduplicateData", this._type = "pandas_df_processor", this._category = "transform", this._icon = C, this._default = {}, this._form = {
+                    super(...arguments), this._name = "JSON File Output", this._id = "jsonFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
+                        jsonOptions: {
+                            orient: "records"
+                        }
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Columns",
-                            id: "subset",
-                            placeholder: "Optional: comma separated column names"
+                            type: "file",
+                            label: "File path",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: ".(json|jsonl)$",
+                            validationMessage: "This field expects a file with a json or jsonl extension such as output.json."
                         }, {
-                            type: "datalist",
-                            label: "Keep (survivorship)",
-                            id: "keep",
-                            placeholder: "first",
+                            type: "select",
+                            label: "Orientation",
+                            id: "jsonOptions.orient",
+                            placeholder: "Select orientation",
                             options: [{
-                                key: "first",
-                                value: "first",
-                                text: "Drop duplicates except for the first occurrence."
+                                value: "columns",
+                                label: "columns (JSON object with column labels as keys)"
                             }, {
-                                key: "last",
-                                value: "last",
-                                text: "Drop duplicates except for the last occurrence."
+                                value: "records",
+                                label: "records (List of rows as JSON objects)"
                             }, {
-                                key: "false",
-                                value: !1,
-                                text: "Drop all duplicates."
+                                value: "index",
+                                label: "index (Dict with index labels as keys)"
+                            }, {
+                                value: "split",
+                                label: "split (Dict with 'index', 'columns', and 'data' keys)"
+                            }, {
+                                value: "table",
+                                label: "table (Dict with 'schema' and 'data' keys, following the Table Schema)"
                             }]
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Fe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Me.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Fe.Name,
-                        ConfigForm: Fe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Me.Name,
+                        ConfigForm: Me.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Fe.Icon,
+                        Icon: Me.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    let a = "# Deduplicate\n";
-                    return a += `${n} = ${t}.drop_duplicates(${e.columns?`subset=['${e.columns.split(",").map((e=>e.trim())).join("', '")}'], `:""}keep=${e.keepFirst?"'first'":"'last'"})\n`, a
+                    let n = Object.entries(e.jsonOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
+                    const o = n ? `, ${n}` : "";
+                    return `\n${t}.to_json('${e.filePath}'${o})\n`
                 }
             }
-            W = Fe, Fe.ConfigForm = ({
+            ne = Me, Me.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = W.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = ne.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: W.Type,
-                    name: W.Name,
-                    form: W.Form,
+                    type: ne.Type,
+                    name: ne.Name,
+                    form: ne.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class $e extends((0, a.PipelineComponent)()) {
+            class Oe extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Expand JSON List", this._id = "expandList", this._type = "pandas_df_processor", this._category = "transform", this._icon = f, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Excel File Output", this._id = "excelFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
+                        excelOptions: {}
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
+                            type: "file",
+                            label: "File path",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: "\\.(xlsx)$",
+                            validationMessage: "This field expects a file with a xlsx extension such as output.xlsx."
+                        }, {
                             type: "input",
-                            label: "Column",
-                            id: "column",
-                            placeholder: "Type column name"
+                            label: "Sheet",
+                            id: "excelOptions.sheet",
+                            placeholder: "default: Sheet1"
+                        }, {
+                            type: "radio",
+                            label: "Mode",
+                            id: "mode",
+                            options: [{
+                                value: "write",
+                                label: "Write"
+                            }, {
+                                value: "append",
+                                label: "Append"
+                            }],
+                            advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: $e.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Oe.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: $e.Name,
-                        ConfigForm: $e.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Oe.Name,
+                        ConfigForm: Oe.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: $e.Icon,
+                        Icon: Oe.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
+                provideDependencies({
+                    config: e
+                }) {
+                    let t = [];
+                    return t.push("openpyxl"), t
+                }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    let a = "# Expand the list in the specified column\n";
-                    return a += "import pandas as pd\n", a += `${n} = ${t}['${e.column}'].apply(pd.Series)\n`, a
+                    let n = "a" === e.excelOptions.mode,
+                        o = {
+                            ...e.excelOptions
+                        };
+                    delete o.mode;
+                    let a = Object.entries(o).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
+                    a = a ? `, ${a}` : "";
+                    let s = "";
+                    return s = n ? `with pd.ExcelWriter('${e.filePath}', mode='a') as writer:\n    ${t}.to_excel(writer, index=False${a})\n  ` : `${t}.to_excel('${e.filePath}', index=False${a})\n  `, s
                 }
             }
-            Z = $e, $e.ConfigForm = ({
+            oe = Oe, Oe.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = Z.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = oe.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Z.Type,
-                    name: Z.Name,
-                    form: Z.Form,
+                    type: oe.Type,
+                    name: oe.Name,
+                    form: oe.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Ee extends((0, a.PipelineComponent)()) {
+            class ze extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Sample", this._id = "sample", this._type = "pandas_df_processor", this._category = "transform", this._icon = h, this._default = {
-                        mode: "random"
+                    super(...arguments), this._name = "Parquet File Output", this._id = "parquetFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {
+                        parquetOptions: {
+                            compression: "snappy"
+                        }
                     }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "quantity",
-                            label: "Rows number",
-                            id: "rows",
-                            placeholder: "Rows number"
+                            type: "file",
+                            label: "File path",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: "\\.(parquet)$",
+                            validationMessage: "This field expects a file with a .parquet extension such as output.parquet."
                         }, {
                             type: "radio",
-                            label: "Mode",
-                            id: "mode",
+                            label: "Compression",
+                            id: "parquetOptions.compression",
                             options: [{
-                                key: "random",
-                                value: "random",
-                                text: "Random"
+                                value: "snappy",
+                                label: "Snappy"
                             }, {
-                                key: "head",
-                                value: "head",
-                                text: "First"
+                                value: "gzip",
+                                label: "GZip"
                             }, {
-                                key: "tail",
-                                value: "tail",
-                                text: "Last"
+                                value: "brotli",
+                                label: "Brotli"
+                            }, {
+                                value: "None",
+                                label: "None"
                             }],
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Ee.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: ze.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Ee.Name,
-                        ConfigForm: Ee.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: ze.Name,
+                        ConfigForm: ze.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Ee.Icon,
+                        Icon: ze.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    let a = "";
-                    return "random" === e.mode ? a = `${n} = ${t}.sample(n=${e.rows})` : "tail" === e.mode ? a = `${n} = ${t}.tail(${e.rows})` : "head" === e.mode && (a = `${n} = ${t}.head(${e.rows})`), `\n${a}\n  `
+                    let n = Object.entries(e.parquetOptions || {}).filter((([e, t]) => null !== t && "" !== t)).map((([e, t]) => `${e}='${t}'`)).join(", ");
+                    return n = n ? `, ${n}` : "", `\n${t}.to_parquet('${e.filePath}'${n})\n`
                 }
             }
-            K = Ee, Ee.ConfigForm = ({
+            ae = ze, ze.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = K.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = ae.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: K.Type,
-                    name: K.Name,
-                    form: K.Form,
+                    type: ae.Type,
+                    name: ae.Name,
+                    form: ae.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class ke extends((0, a.PipelineComponent)()) {
+            class Ue extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Sort", this._id = "sort", this._type = "pandas_df_processor", this._category = "transform", this._icon = I, this._default = {
-                        order: "true"
-                    }, this._form = {
+                    super(...arguments), this._name = "XML File Output", this._id = "xmlFileOutput", this._type = "pandas_df_output", this._category = "output", this._icon = i, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Columns",
-                            id: "by",
-                            placeholder: "Column name(s)"
-                        }, {
-                            type: "radio",
-                            label: "Order",
-                            id: "order",
-                            options: [{
-                                key: "true",
-                                value: "True",
-                                text: "Asc."
-                            }, {
-                                key: "false",
-                                value: "False",
-                                text: "Desc."
-                            }]
-                        }, {
-                            type: "boolean",
-                            label: "Ignore Index",
-                            id: "ignoreIndex",
-                            advanced: !0
+                            type: "file",
+                            label: "File path",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: "\\.xml$",
+                            validationMessage: "This field expects a file with an xml extension such as output.xml."
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: ke.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ue.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: ke.Name,
-                        ConfigForm: ke.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Ue.Name,
+                        ConfigForm: Ue.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: ke.Icon,
+                        Icon: Ue.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd"]
+                    return ["import xml.etree.ElementTree as ET", "import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    return `${n} = ${t}.sort_values(${e.by?`by=[${e.by.split(",").map((e=>`'${e.trim()}'`)).join(", ")}]`:""}${void 0!==e.order?`, ascending=${e.order}`:""}${e.ignoreIndex?`, ignore_index=${e.ignoreIndex}`:""})`
+                    const n = `${t}_xml_output`,
+                        o = `${t}_file`;
+                    return `\n# Output the XML content to a file\n${n} = ${t}.to_xml()\nwith open('${e.filePath}', 'w') as ${o}:\n    ${o}.write(${n})\n`
                 }
             }
-            X = ke, ke.ConfigForm = ({
+            se = Ue, Ue.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = X.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = se.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: X.Type,
-                    name: X.Name,
-                    form: X.Form,
+                    type: se.Type,
+                    name: se.Name,
+                    form: se.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Pe extends((0, a.PipelineComponent)()) {
+            class Le extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Rename Columns", this._id = "rename", this._type = "pandas_df_processor", this._category = "transform", this._icon = x, this._default = {}, this._form = {
+                    super(...arguments), this._name = "G. Sheets Output", this._id = "googleSheetsOutput", this._type = "pandas_df_output", this._category = "output", this._icon = w, this._default = {
+                        sheetOptions: {
+                            spreadsheetId: "",
+                            range: "Sheet1"
+                        }
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "keyvalue",
-                            label: "Columns",
-                            id: "columns",
-                            placeholders: {
-                                key: "column name",
-                                value: "new column name"
-                            },
-                            advanced: !0
+                            type: "file",
+                            label: "Service Account Key",
+                            id: "filePath",
+                            placeholder: "Type file name",
+                            validation: "\\.(json)$",
+                            validationMessage: "This field expects a file with a .json extension such as your-service-account-file.json."
                         }, {
-                            type: "boolean",
-                            label: "Numeric indexes",
-                            id: "indexes",
-                            placeholder: "false",
-                            advanced: !0
+                            type: "input",
+                            label: "Spreadsheet ID",
+                            id: "sheetOptions.spreadsheetId",
+                            placeholder: "Enter Google Sheets' name or ID",
+                            validation: "^[a-zA-Z0-9-_]+$",
+                            validationMessage: "Invalid Spreadsheet ID."
+                        }, {
+                            type: "input",
+                            label: "Range",
+                            id: "sheetOptions.range",
+                            placeholder: "e.g., Sheet1 or Sheet1!A1:D5",
+                            validation: "^[a-zA-Z0-9-_!]+$",
+                            validationMessage: "Invalid Range."
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Pe.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Le.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Pe.Name,
-                        ConfigForm: Pe.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Le.Name,
+                        ConfigForm: Le.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Pe.Icon,
+                        Icon: Le.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd"]
+                    return ["import pandas as pd", "import gspread", "from oauth2client.service_account import ServiceAccountCredentials"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    const a = e.indexes;
-                    let o = "";
-                    return e.columns && e.columns.length > 0 && (o = a ? "columns={" + e.columns.map((e => `${e.key}: '${e.value}'`)).join(", ") + "}" : "columns={" + e.columns.map((e => `'${e.key}': '${e.value}'`)).join(", ") + "}"), `\n# Rename columns\n${n} = ${t}.rename(${o})\n`
+                    let n = {
+                        ...e.sheetOptions
+                    };
+                    const o = `${t}Client`,
+                        a = `${t}Sheet`;
+                    return `\n# Outputting data to Google Sheets\nscope = ['https://spreadsheets.google.com/feeds','https://www.googleapis.com/auth/drive']\ncreds = ServiceAccountCredentials.from_json_keyfile_name(${e.filePath?`'${e.filePath}'`:"None"}, scope)\n${o} = gspread.authorize(creds)\n\n# Open the spreadsheet and select the right worksheet\n${a} = ${o}.open_by_key(${n.spreadsheetId?`'${n.spreadsheetId}'`:"None"}).worksheet(${n.range?`'${n.range.split("!")[0]}'`:"None"})\n\n# Update the sheet with dataframe's data\n${a}.update([${t}.columns.values.tolist()] + ${t}.values.tolist())\n`
                 }
             }
-            Y = Pe, Pe.ConfigForm = ({
+            re = Le, Le.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = Y.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = re.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: Y.Type,
-                    name: Y.Name,
-                    form: Y.Form,
+                    type: re.Type,
+                    name: re.Name,
+                    form: re.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Se extends((0, a.PipelineComponent)()) {
+            class je extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Filter Columns", this._id = "filterColumns", this._type = "pandas_df_processor", this._category = "transform", this._icon = h, this._default = {}, this._form = {
+                    super(...arguments), this._name = "MySQL Output", this._id = "mySQLOutput", this._type = "pandas_df_output", this._category = "output", this._icon = N, this._default = {
+                        dbOptions: {
+                            host: "localhost",
+                            port: "3306",
+                            databaseName: "",
+                            tableName: "",
+                            username: "",
+                            password: ""
+                        }
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "valuesList",
-                            label: "Columns to keep",
-                            id: "columns",
-                            placeholders: "columns list comma-separated",
+                            type: "input",
+                            label: "Host",
+                            id: "dbOptions.host",
+                            placeholder: "Enter database host",
                             advanced: !0
                         }, {
-                            type: "boolean",
-                            label: "Numeric indexes",
-                            id: "indexes",
-                            placeholder: "false",
+                            type: "input",
+                            label: "Port",
+                            id: "dbOptions.port",
+                            placeholder: "Enter database port",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Database Name",
+                            id: "dbOptions.databaseName",
+                            placeholder: "Enter database name"
+                        }, {
+                            type: "input",
+                            label: "Table Name",
+                            id: "dbOptions.tableName",
+                            placeholder: "Enter table name"
+                        }, {
+                            type: "input",
+                            label: "Username",
+                            id: "dbOptions.username",
+                            placeholder: "Enter username",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Password",
+                            id: "dbOptions.password",
+                            placeholder: "Enter password",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Se.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: je.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Se.Name,
-                        ConfigForm: Se.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: je.Name,
+                        ConfigForm: je.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Se.Icon,
+                        Icon: je.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd"]
+                    return ["import pandas as pd", "import sqlalchemy"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    const a = e.columns;
-                    let o = "";
-                    if (e.indexes) {
-                        const e = a.map((e => parseInt(e)));
-                        o = `.iloc[:, ${JSON.stringify(e)}]`
-                    } else o = `.filter(${JSON.stringify(a)})`;
-                    return `\n# Filter columns\n${n} = ${t}${o}\n    `
+                    const n = `${t}Engine`;
+                    return `\n# Connect to MySQL and output into table\n${n} = sqlalchemy.create_engine('mysql+pymysql://${e.dbOptions.username}:${e.dbOptions.password}@${e.dbOptions.host}:${e.dbOptions.port}/${e.dbOptions.databaseName}')\n${t}.to_sql(name='${e.dbOptions.tableName}', con=${n}, if_exists='replace', index=False)\n`
                 }
             }
-            ee = Se, Se.ConfigForm = ({
+            de = je, je.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = ee.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = de.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ee.Type,
-                    name: ee.Name,
-                    form: ee.Form,
+                    type: de.Type,
+                    name: de.Name,
+                    form: de.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Te extends((0, a.PipelineComponent)()) {
+            class Re extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Type Converter", this._id = "typeConverter", this._type = "pandas_df_processor", this._category = "transform", this._icon = y, this._default = {
-                        dataType: "string"
-                    }, this._form = {
+                    super(...arguments), this._name = "Console", this._id = "console", this._type = "pandas_df_output", this._category = "output", this._icon = m, this._default = {}, this._form = {
                         idPrefix: "component__form",
                         fields: [{
-                            type: "input",
-                            label: "Column name",
-                            id: "columnName",
-                            placeholder: "Column name"
-                        }, {
-                            type: "singleInputCreatableSelect",
-                            label: "Data Type to convert to",
-                            id: "dataType",
-                            placeholder: "Select column type to convert to",
-                            options: [{
-                                value: "null",
-                                label: "Select or specify type",
-                                isDisabled: !0
-                            }, {
-                                value: "string",
-                                label: "string: For string data."
-                            }, {
-                                value: "int",
-                                label: "int: For integer types (use int64, int32, int16, etc. for optimized memory usage)."
-                            }, {
-                                value: "float",
-                                label: "float: For floating-point numbers (use float64, float32, etc. for optimized memory usage)."
-                            }, {
-                                value: "object",
-                                label: "object: For generic objects (strings, timestamps, mixed types)."
-                            }, {
-                                value: "bool",
-                                label: "bool: For boolean values (True or False)."
-                            }, {
-                                value: "datetime64",
-                                label: "datetime64: For datetime values (use datetime64[ns], datetime64[ns, tz] for more options)."
-                            }, {
-                                value: "timedelta[ns]",
-                                label: "timedelta[ns]: For differences between two datetimes."
-                            }, {
-                                value: "category",
-                                label: "category: For categorical variables."
-                            }]
+                            type: "inputNumber",
+                            label: "Records limit",
+                            id: "limit",
+                            placeholder: "Number of records to print in console",
+                            min: 0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: Te.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Re.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: Te.Name,
-                        ConfigForm: Te.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Re.Name,
+                        ConfigForm: Re.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: Te.Icon,
+                        Icon: Re.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
                     return ["import pandas as pd"]
                 }
                 generateComponentCode({
                     config: e,
-                    inputName: t,
-                    outputName: n
+                    inputName: t
                 }) {
-                    const {
-                        columnName: a,
-                        dataType: o
-                    } = e;
-                    return `\n# Convert ${a} to ${o}\n${n} = ${t}.assign(${a}=${t}['${a}'].astype('${o}'))\n`
+                    return e.limit && (t += `.head(${e.limit})`), `\nprint(${t})\n`
                 }
             }
-            te = Te, Te.ConfigForm = ({
+            le = Re, Re.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = te.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = le.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: te.Type,
-                    name: te.Name,
-                    form: te.Form,
+                    type: le.Type,
+                    name: le.Name,
+                    form: le.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class He extends((0, a.PipelineComponent)()) {
+            class qe extends((0, o.PipelineComponent)()) {
+                constructor() {
+                    super(...arguments), this._name = "Annotation", this._id = "annotation", this._type = "annotation", this._icon = c, this._category = "other"
+                }
+                UIComponent({
+                    id: e,
+                    data: t,
+                    context: n,
+                    manager: o
+                }) {
+                    (0, r.useStore)((e => e.transform[2] >= 1));
+                    const {
+                        nodeInternals: a,
+                        edges: d
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    })));
+                    return s().createElement(s().Fragment, null, s().createElement("div", {
+                        className: "mt-[5px] border-0 bg-white mx-auto box-border w-full"
+                    }, s().createElement(qe.ConfigForm, {
+                        nodeId: e,
+                        data: t,
+                        context: n,
+                        manager: o
+                    })))
+                }
+            }
+            qe.ConfigForm = ({
+                nodeId: e,
+                data: t,
+                context: n,
+                manager: o
+            }) => {
+                const {
+                    setNodes: d
+                } = (0, r.useReactFlow)(), l = (0, r.useStoreApi)(), i = (0, a.useCallback)(((t, n) => {
+                    const o = t.target.value,
+                        {
+                            nodeInternals: a
+                        } = l.getState();
+                    d(Array.from(a.values()).map((t => (t.id === e && (t.data = {
+                        ...t.data,
+                        [n]: o
+                    }), t))))
+                }), []);
+                return s().createElement("textarea", {
+                    id: "text",
+                    name: "text",
+                    onChange: e => i(e, "text"),
+                    value: t.text,
+                    className: "nodrag mt-[5px] border-0 bg-white block w-full box-border"
+                })
+            };
+            class Be extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Extract (Regex)", this._id = "extract", this._type = "pandas_df_processor", this._category = "transform", this._icon = _, this._default = {}, this._form = {
+                    super(...arguments), this._name = "Email Logger", this._id = "emailLogger", this._type = "logger", this._category = "other", this._icon = g, this._default = {
+                        smtpServer: "smtp.example.com",
+                        smtpPort: 587
+                    }, this._form = {
                         idPrefix: "component__form",
                         fields: [{
                             type: "input",
-                            label: "Column name",
-                            id: "columnName",
-                            placeholder: "Column name"
+                            label: "Receiver Email",
+                            id: "receiverEmail",
+                            placeholder: "Receiver Email"
                         }, {
                             type: "input",
-                            label: "Regular Expression",
-                            id: "regex",
-                            placeholder: "Regular Expression"
+                            label: "Sender Email",
+                            id: "senderEmail",
+                            placeholder: "Sender Email",
+                            advanced: !0
                         }, {
-                            type: "datalist",
-                            label: "Flags",
-                            id: "flags",
-                            placeholder: "Type or select",
-                            options: [{
-                                key: "IGNORE CASE",
-                                value: "IGNORECASE",
-                                text: "Makes the match case-insensitive. For example, it will match both 'abc' and 'ABC'."
-                            }, {
-                                key: "MULTILINE",
-                                value: "MULTILINE",
-                                text: "Changes the behavior of ^ and $ to match the start and end of each line, not just the start and end of the whole string."
-                            }, {
-                                key: "DOTALL",
-                                value: "DOTALL",
-                                text: "Makes the . match any character at all, including a newline; without this flag, . will match anything except a newline."
-                            }, {
-                                key: "UNICODE",
-                                value: "UNICODE",
-                                text: "Makes \\w, \\W, \\b, \\B, \\d, \\D, \\s, and \\S sequences dependent on the Unicode character properties database. This is the default behavior in Python 3 for strings."
-                            }, {
-                                key: "ASCII",
-                                value: "ASCII",
-                                text: "Makes \\w, \\W, \\b, \\B, \\d, \\D, \\s, and \\S perform ASCII-only matching instead of full Unicode matching."
-                            }, {
-                                key: "VERBOSE",
-                                value: "VERBOSE",
-                                text: "Allows you to write regular expressions that are more readable by permitting whitespace and comments within the pattern string."
-                            }],
+                            type: "input",
+                            label: "Sender Password",
+                            id: "senderPassword",
+                            placeholder: "Receiver Email",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "SMTP server",
+                            id: "smtpServer",
+                            placeholder: "smtp.example.com",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "SMTP port",
+                            id: "smtpPort",
+                            placeholder: "587",
+                            advanced: !0
+                        }, {
+                            type: "input",
+                            label: "Subject",
+                            id: "emailSubject",
+                            placeholder: "Pipeline Failure",
+                            advanced: !0
+                        }, {
+                            type: "textarea",
+                            label: "Email Content",
+                            id: "emailContent",
+                            placeholder: "An error occurred in the script:\n\n{error_message}",
                             advanced: !0
                         }]
                     }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: d,
-                    commands: l
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
                     const {
-                        setNodes: i,
-                        deleteElements: m,
-                        setViewport: c
-                    } = (0, r.useReactFlow)(), p = (0, r.useStoreApi)(), u = (0, o.useCallback)((() => {
-                        m({
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
                             nodes: [{
                                 id: e
                             }]
                         })
-                    }), [e, m]), h = (0, r.useStore)((e => e.transform[2] >= 1)), g = s().createElement(a.renderHandle, {
-                        type: He.Type,
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Be.Type,
                         Handle: r.Handle,
-                        Position: r.Position
+                        Position: r.Position,
+                        internals: C
                     });
-                    return s().createElement(s().Fragment, null, (0, a.renderComponentUI)({
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
                         id: e,
                         data: t,
                         context: n,
-                        manager: d,
-                        commands: l,
-                        name: He.Name,
-                        ConfigForm: He.ConfigForm({
+                        manager: l,
+                        commands: i,
+                        name: Be.Name,
+                        ConfigForm: Be.ConfigForm({
                             nodeId: e,
                             data: t,
                             context: n,
-                            manager: d,
-                            commands: l,
-                            store: p,
-                            setNodes: i
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
                         }),
-                        Icon: He.Icon,
+                        Icon: Be.Icon,
                         showContent: h,
-                        handle: g,
-                        deleteNode: u,
-                        setViewport: c
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
                     }))
                 }
                 provideImports({
                     config: e
                 }) {
-                    return ["import pandas as pd", "import re"]
+                    return ["import smtplib", "from email.mime.text import MIMEText", "from email.mime.multipart import MIMEMultipart"]
+                }
+                provideFunctions({
+                    config: e
+                }) {
+                    let t = [];
+                    const n = `\ndef send_email(error_message):\n    sender_email = "${e.senderEmail}"\n    receiver_email = "${e.receiverEmail}"\n    password =\n\n    message = MIMEMultipart("alternative")\n    message["Subject"] = "Script Failure Notification"\n    message["From"] = sender_email\n    message["To"] = receiver_email\n\n    text =  "${e.emailContent}"\n    part1 = MIMEText(text, "plain")\n    message.attach(part1)\n\n    server = smtplib.SMTP('${e.smtpServer}', ${e.smtpPort})\n    server.starttls()\n    server.login(sender_email, password)\n    server.sendmail(sender_email, receiver_email, message.as_string())\n    server.quit()\n    `;
+                    return t.push(n), t
                 }
                 generateComponentCode({
-                    config: e,
-                    inputName: t,
-                    outputName: n
+                    config: e
                 }) {
-                    const a = e.columnName,
-                        o = e.regex;
-                    let s = "";
-                    "" !== e.flags.trim() && (s = `, flags=${e.flags.split(",").filter((e=>""!==e.trim())).map((e=>`re.${e}`)).join(" | ")}`);
-                    const r = new RegExp(o + "|").exec("").length - 1,
-                        d = Array.from({
-                            length: r
-                        }, ((e, t) => `'${n}_${t+1}'`)).join(", "),
-                        l = `${n}_extracted`;
-                    return `\n# Extract data using regex\n${l} = ${t}['${a}'].str.extract(r'${o}'${s})\n${l}.columns = [${d}]\n${n} = ${t}.join(${l}, rsuffix='_extracted')\n`
+                    return "\n# Send email\nsend_email(str(e))\n"
                 }
             }
-            ne = He, He.ConfigForm = ({
+            ie = Be, Be.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: r,
-                commands: d,
-                store: l,
-                setNodes: i
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const m = ne.Default,
-                    c = (0, o.useCallback)((() => {
-                        (0, a.setDefaultConfig)({
-                            nodeId: e,
-                            store: l,
-                            setNodes: i,
-                            defaultConfig: m
-                        })
-                    }), [e, l, i, m]);
-                (0, o.useEffect)((() => {
-                    c()
-                }), [c]);
-                const p = (0, o.useCallback)(((t, n) => {
-                    (0, a.onChange)({
+                const c = ie.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
                         evtTargetValue: t,
                         field: n,
                         nodeId: e,
-                        store: l,
-                        setNodes: i
+                        store: i,
+                        setNodes: m
                     })
-                }), [e, l, i]);
-                return s().createElement(s().Fragment, null, (0, a.generateUIFormComponent)({
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
                     nodeId: e,
-                    type: ne.Type,
-                    name: ne.Name,
-                    form: ne.Form,
+                    type: ie.Type,
+                    name: ie.Name,
+                    form: ie.Form,
                     data: t,
                     context: n,
-                    manager: r,
-                    commands: d,
-                    handleChange: p
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
                 }))
             };
-            class Ve extends((0, a.PipelineComponent)()) {
+            class Ge extends((0, o.PipelineComponent)()) {
                 constructor() {
-                    super(...arguments), this._name = "Annotation", this._id = "annotation", this._type = "annotation", this._icon = c, this._category = "other"
+                    super(...arguments), this._name = "File Logger", this._id = "fileLogger", this._type = "logger", this._category = "other", this._icon = g, this._default = {
+                        filePath: "pipeline.log",
+                        logLevel: "INFO",
+                        logMessage: "An error occurred in the script:\n\n{error_message}"
+                    }, this._form = {
+                        idPrefix: "component__form",
+                        fields: [{
+                            type: "file",
+                            label: "Log File Path",
+                            id: "filePath",
+                            placeholder: "pipeline.log"
+                        }, {
+                            type: "select",
+                            label: "Log Level",
+                            id: "logLevel",
+                            placeholder: "default: ,",
+                            options: [{
+                                value: "DEBUG",
+                                label: "DEBUG"
+                            }, {
+                                value: "INFO",
+                                label: "INFO"
+                            }, {
+                                value: "WARNING",
+                                label: "WARNING"
+                            }, {
+                                value: "ERROR",
+                                label: "ERROR"
+                            }, {
+                                value: "CRITICAL",
+                                label: "CRITICAL"
+                            }],
+                            advanced: !0
+                        }, {
+                            type: "textarea",
+                            label: "Log Message",
+                            id: "logMessage",
+                            placeholder: "An error occurred in the script:\n\n{error_message}",
+                            advanced: !0
+                        }]
+                    }
                 }
                 UIComponent({
                     id: e,
                     data: t,
                     context: n,
-                    manager: a
+                    componentService: d,
+                    manager: l,
+                    commands: i
                 }) {
-                    return (0, r.useStore)((e => e.transform[2] >= 1)), s().createElement(s().Fragment, null, s().createElement("div", {
-                        className: "mt-[5px] border-0 bg-white mx-auto box-border w-full"
-                    }, s().createElement(Ve.ConfigForm, {
-                        nodeId: e,
+                    const {
+                        setNodes: m,
+                        deleteElements: c,
+                        setViewport: p
+                    } = (0, r.useReactFlow)(), u = (0, r.useStoreApi)(), g = (0, a.useCallback)((() => {
+                        c({
+                            nodes: [{
+                                id: e
+                            }]
+                        })
+                    }), [e, c]), h = (0, r.useStore)((e => e.transform[2] >= 1)), {
+                        nodeInternals: f,
+                        edges: v
+                    } = (0, r.useStore)((e => ({
+                        nodeInternals: e.nodeInternals,
+                        edges: e.edges
+                    }))), C = {
+                        nodeInternals: f,
+                        edges: v,
+                        nodeId: e
+                    }, I = s().createElement(o.renderHandle, {
+                        type: Ge.Type,
+                        Handle: r.Handle,
+                        Position: r.Position,
+                        internals: C
+                    });
+                    return s().createElement(s().Fragment, null, (0, o.renderComponentUI)({
+                        id: e,
                         data: t,
                         context: n,
-                        manager: a
-                    })))
+                        manager: l,
+                        commands: i,
+                        name: Ge.Name,
+                        ConfigForm: Ge.ConfigForm({
+                            nodeId: e,
+                            data: t,
+                            context: n,
+                            componentService: d,
+                            manager: l,
+                            commands: i,
+                            store: u,
+                            setNodes: m
+                        }),
+                        Icon: Ge.Icon,
+                        showContent: h,
+                        handle: I,
+                        deleteNode: g,
+                        setViewport: p
+                    }))
+                }
+                provideImports({
+                    config: e
+                }) {
+                    return ["import logging"]
+                }
+                provideFunctions({
+                    config: e
+                }) {
+                    let t = [];
+                    const n = `\nlogger = logging.getLogger('PipelineLogger')\nlogging.basicConfig(filename='${e.filePath}', level=logging.${e.logLevel}, format='%(asctime)s - %(name)s - %(levelname)s - %(message)s')\n`;
+                    return t.push(n), t
+                }
+                generateComponentCode({
+                    config: e
+                }) {
+                    return "\nlogger.info(str(e))\n"
                 }
             }
-            Ve.ConfigForm = ({
+            me = Ge, Ge.ConfigForm = ({
                 nodeId: e,
                 data: t,
                 context: n,
-                manager: a
+                componentService: r,
+                manager: d,
+                commands: l,
+                store: i,
+                setNodes: m
             }) => {
-                const {
-                    setNodes: d
-                } = (0, r.useReactFlow)(), l = (0, r.useStoreApi)(), i = (0, o.useCallback)(((t, n) => {
-                    const a = t.target.value,
-                        {
-                            nodeInternals: o
-                        } = l.getState();
-                    d(Array.from(o.values()).map((t => (t.id === e && (t.data = {
-                        ...t.data,
-                        [n]: a
-                    }), t))))
-                }), []);
-                return s().createElement("textarea", {
-                    id: "text",
-                    name: "text",
-                    onChange: e => i(e, "text"),
-                    value: t.text,
-                    className: "nodrag mt-[5px] border-0 bg-white block w-full box-border"
-                })
+                const c = me.Default,
+                    p = (0, a.useCallback)((() => {
+                        (0, o.setDefaultConfig)({
+                            nodeId: e,
+                            store: i,
+                            setNodes: m,
+                            defaultConfig: c
+                        })
+                    }), [e, i, m, c]);
+                (0, a.useEffect)((() => {
+                    p()
+                }), [p]);
+                const u = (0, a.useCallback)(((t, n) => {
+                    (0, o.onChange)({
+                        evtTargetValue: t,
+                        field: n,
+                        nodeId: e,
+                        store: i,
+                        setNodes: m
+                    })
+                }), [e, i, m]);
+                return s().createElement(s().Fragment, null, (0, o.generateUIFormComponent)({
+                    nodeId: e,
+                    type: me.Type,
+                    name: me.Name,
+                    form: me.Form,
+                    data: t,
+                    context: n,
+                    componentService: r,
+                    manager: d,
+                    commands: l,
+                    handleChange: u
+                }))
             };
-            const Oe = {
+            const Je = {
                 id: "@amphi/pipeline-components-core",
                 description: "Adds a step counter/button (1 of 3 related examples). This extension holds the UI/interface",
                 autoStart: !0,
-                requires: [a.ComponentManager],
+                requires: [o.ComponentManager],
                 activate: (e, t) => {
-                    console.log("JupyterLab extension pipeline-components-core is activated!"), t.addComponent(ae.getInstance()), t.addComponent(oe.getInstance()), t.addComponent(se.getInstance()), t.addComponent(re.getInstance()), t.addComponent(de.getInstance()), t.addComponent(le.getInstance()), t.addComponent(ie.getInstance()), t.addComponent(me.getInstance()), t.addComponent(ce.getInstance()), t.addComponent(pe.getInstance()), t.addComponent(ue.getInstance()), t.addComponent(he.getInstance()), t.addComponent(ge.getInstance()), t.addComponent(fe.getInstance()), t.addComponent(Ce.getInstance()), t.addComponent(ve.getInstance()), t.addComponent(Ie.getInstance()), t.addComponent(xe.getInstance()), t.addComponent(ye.getInstance()), t.addComponent(_e.getInstance()), t.addComponent(be.getInstance()), t.addComponent(Ne.getInstance()), t.addComponent(we.getInstance()), t.addComponent(Fe.getInstance()), t.addComponent($e.getInstance()), t.addComponent(Ee.getInstance()), t.addComponent(ke.getInstance()), t.addComponent(Pe.getInstance()), t.addComponent(Se.getInstance()), t.addComponent(Te.getInstance()), t.addComponent(He.getInstance()), t.addComponent(Ve.getInstance())
+                    console.log("JupyterLab extension pipeline-components-core is activated!"), t.addComponent(ce.getInstance()), t.addComponent(pe.getInstance()), t.addComponent(ue.getInstance()), t.addComponent(ge.getInstance()), t.addComponent(he.getInstance()), t.addComponent(fe.getInstance()), t.addComponent(ve.getInstance()), t.addComponent(Ce.getInstance()), t.addComponent(Ie.getInstance()), t.addComponent(be.getInstance()), t.addComponent(_e.getInstance()), t.addComponent(ye.getInstance()), t.addComponent(xe.getInstance()), t.addComponent(we.getInstance()), t.addComponent(Ne.getInstance()), t.addComponent(Fe.getInstance()), t.addComponent(Se.getInstance()), t.addComponent($e.getInstance()), t.addComponent(Ee.getInstance()), t.addComponent(Pe.getInstance()), t.addComponent(Te.getInstance()), t.addComponent(ke.getInstance()), t.addComponent(He.getInstance()), t.addComponent(Ae.getInstance()), t.addComponent(Ve.getInstance()), t.addComponent(De.getInstance()), t.addComponent(Me.getInstance()), t.addComponent(Oe.getInstance()), t.addComponent(ze.getInstance()), t.addComponent(Ue.getInstance()), t.addComponent(Le.getInstance()), t.addComponent(je.getInstance()), t.addComponent(Re.getInstance()), t.addComponent(qe.getInstance()), t.addComponent(Be.getInstance()), t.addComponent(Ge.getInstance())
                 }
             }
         }
     }
 ]);
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/713.672682fff3504f6c1da4.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-/*! For license information please see 713.672682fff3504f6c1da4.js.LICENSE.txt */
+/*! For license information please see 713.a7e0851307239af436d3.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amphi_pipeline_components_core = self.webpackChunk_amphi_pipeline_components_core || []).push([
     [713], {
         335: (e, t, n) => {
             var o = n(345),
                 r = Symbol.for("react.element"),
                 a = Symbol.for("react.fragment"),
@@ -50,21 +50,21 @@
                 EdgeText: () => xo,
                 Handle: () => Hr,
                 MarkerType: () => Wo,
                 MiniMap: () => Gc,
                 NodeResizeControl: () => BN,
                 NodeResizer: () => TN,
                 NodeToolbar: () => Uv,
-                PanOnScrollMode: () => Fo,
+                PanOnScrollMode: () => Ko,
                 Panel: () => yo,
                 Position: () => Go,
                 ReactFlow: () => Qs,
                 ReactFlowProvider: () => Xs,
                 ResizeControlVariant: () => _N,
-                SelectionMode: () => Ko,
+                SelectionMode: () => Fo,
                 SimpleBezierEdge: () => Jo,
                 SmoothStepEdge: () => rr,
                 StepEdge: () => ar,
                 StraightEdge: () => ir,
                 addEdge: () => vr,
                 applyEdgeChanges: () => us,
                 applyNodeChanges: () => cs,
@@ -380,22 +380,22 @@
 
             function Z(e, t) {
                 return function() {
                     this.setAttributeNS(e.space, e.local, t)
                 }
             }
 
-            function F(e, t) {
+            function K(e, t) {
                 return function() {
                     var n = t.apply(this, arguments);
                     null == n ? this.removeAttribute(e) : this.setAttribute(e, n)
                 }
             }
 
-            function K(e, t) {
+            function F(e, t) {
                 return function() {
                     var n = t.apply(this, arguments);
                     null == n ? this.removeAttributeNS(e.space, e.local) : this.setAttributeNS(e.space, e.local, n)
                 }
             }
 
             function U(e) {
@@ -766,15 +766,15 @@
                 },
                 attr: function(e, t) {
                     var n = H(e);
                     if (arguments.length < 2) {
                         var o = this.node();
                         return n.local ? o.getAttributeNS(n.space, n.local) : o.getAttribute(n)
                     }
-                    return this.each((null == t ? n.local ? X : Y : "function" == typeof t ? n.local ? K : F : n.local ? Z : V)(n, t))
+                    return this.each((null == t ? n.local ? X : Y : "function" == typeof t ? n.local ? F : K : n.local ? Z : V)(n, t))
                 },
                 style: function(e, t, n) {
                     return arguments.length > 1 ? this.each((null == t ? W : "function" == typeof t ? q : G)(e, t, null == n ? "" : n)) : Q(this.node(), e)
                 },
                 property: function(e, t) {
                     return arguments.length > 1 ? this.each((null == t ? J : "function" == typeof t ? te : ee)(e, t)) : this.node()[e]
                 },
@@ -983,30 +983,30 @@
                 return !e.ctrlKey && !e.button
             }
 
             function Ze() {
                 return this.parentNode
             }
 
-            function Fe(e, t) {
+            function Ke(e, t) {
                 return null == t ? {
                     x: e.x,
                     y: e.y
                 } : t
             }
 
-            function Ke() {
+            function Fe() {
                 return navigator.maxTouchPoints || "ontouchstart" in this
             }
 
             function Ue() {
                 var e, t, n, o, r = Ve,
                     a = Ze,
-                    s = Fe,
-                    i = Ke,
+                    s = Ke,
+                    i = Fe,
                     l = {},
                     d = v("start", "drag", "end"),
                     c = 0,
                     u = 0;
 
                 function g(e) {
                     e.on("mousedown.drag", h).filter(i).on("touchstart.drag", m).on("touchmove.drag", y, ze).on("touchend.drag touchcancel.drag", S).style("touch-action", "none").style("-webkit-tap-highlight-color", "rgba(0,0,0,0)")
@@ -1454,22 +1454,22 @@
             }
 
             function Ht() {}
             var Yt = .7,
                 Xt = 1 / Yt,
                 Vt = "\\s*([+-]?\\d+)\\s*",
                 Zt = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)\\s*",
-                Ft = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
-                Kt = /^#([0-9a-f]{3,8})$/,
+                Kt = "\\s*([+-]?(?:\\d*\\.)?\\d+(?:[eE][+-]?\\d+)?)%\\s*",
+                Ft = /^#([0-9a-f]{3,8})$/,
                 Ut = new RegExp(`^rgb\\(${Vt},${Vt},${Vt}\\)$`),
-                Wt = new RegExp(`^rgb\\(${Ft},${Ft},${Ft}\\)$`),
+                Wt = new RegExp(`^rgb\\(${Kt},${Kt},${Kt}\\)$`),
                 Gt = new RegExp(`^rgba\\(${Vt},${Vt},${Vt},${Zt}\\)$`),
-                qt = new RegExp(`^rgba\\(${Ft},${Ft},${Ft},${Zt}\\)$`),
-                Qt = new RegExp(`^hsl\\(${Zt},${Ft},${Ft}\\)$`),
-                Jt = new RegExp(`^hsla\\(${Zt},${Ft},${Ft},${Zt}\\)$`),
+                qt = new RegExp(`^rgba\\(${Kt},${Kt},${Kt},${Zt}\\)$`),
+                Qt = new RegExp(`^hsl\\(${Zt},${Kt},${Kt}\\)$`),
+                Jt = new RegExp(`^hsla\\(${Zt},${Kt},${Kt},${Zt}\\)$`),
                 en = {
                     aliceblue: 15792383,
                     antiquewhite: 16444375,
                     aqua: 65535,
                     aquamarine: 8388564,
                     azure: 15794175,
                     beige: 16119260,
@@ -1623,15 +1623,15 @@
 
             function nn() {
                 return this.rgb().formatRgb()
             }
 
             function on(e) {
                 var t, n;
-                return e = (e + "").trim().toLowerCase(), (t = Kt.exec(e)) ? (n = t[1].length, t = parseInt(t[1], 16), 6 === n ? rn(t) : 3 === n ? new ln(t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | 240 & t, (15 & t) << 4 | 15 & t, 1) : 8 === n ? an(t >> 24 & 255, t >> 16 & 255, t >> 8 & 255, (255 & t) / 255) : 4 === n ? an(t >> 12 & 15 | t >> 8 & 240, t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | 240 & t, ((15 & t) << 4 | 15 & t) / 255) : null) : (t = Ut.exec(e)) ? new ln(t[1], t[2], t[3], 1) : (t = Wt.exec(e)) ? new ln(255 * t[1] / 100, 255 * t[2] / 100, 255 * t[3] / 100, 1) : (t = Gt.exec(e)) ? an(t[1], t[2], t[3], t[4]) : (t = qt.exec(e)) ? an(255 * t[1] / 100, 255 * t[2] / 100, 255 * t[3] / 100, t[4]) : (t = Qt.exec(e)) ? pn(t[1], t[2] / 100, t[3] / 100, 1) : (t = Jt.exec(e)) ? pn(t[1], t[2] / 100, t[3] / 100, t[4]) : en.hasOwnProperty(e) ? rn(en[e]) : "transparent" === e ? new ln(NaN, NaN, NaN, 0) : null
+                return e = (e + "").trim().toLowerCase(), (t = Ft.exec(e)) ? (n = t[1].length, t = parseInt(t[1], 16), 6 === n ? rn(t) : 3 === n ? new ln(t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | 240 & t, (15 & t) << 4 | 15 & t, 1) : 8 === n ? an(t >> 24 & 255, t >> 16 & 255, t >> 8 & 255, (255 & t) / 255) : 4 === n ? an(t >> 12 & 15 | t >> 8 & 240, t >> 8 & 15 | t >> 4 & 240, t >> 4 & 15 | 240 & t, ((15 & t) << 4 | 15 & t) / 255) : null) : (t = Ut.exec(e)) ? new ln(t[1], t[2], t[3], 1) : (t = Wt.exec(e)) ? new ln(255 * t[1] / 100, 255 * t[2] / 100, 255 * t[3] / 100, 1) : (t = Gt.exec(e)) ? an(t[1], t[2], t[3], t[4]) : (t = qt.exec(e)) ? an(255 * t[1] / 100, 255 * t[2] / 100, 255 * t[3] / 100, t[4]) : (t = Qt.exec(e)) ? pn(t[1], t[2] / 100, t[3] / 100, 1) : (t = Jt.exec(e)) ? pn(t[1], t[2] / 100, t[3] / 100, t[4]) : en.hasOwnProperty(e) ? rn(en[e]) : "transparent" === e ? new ln(NaN, NaN, NaN, 0) : null
             }
 
             function rn(e) {
                 return new ln(e >> 16 & 255, e >> 8 & 255, 255 & e, 1)
             }
 
             function an(e, t, n, o) {
@@ -1987,15 +1987,15 @@
             function Vn(e, t, n, o) {
                 this._groups = e, this._parents = t, this._name = n, this._id = o
             }
 
             function Zn() {
                 return ++Xn
             }
-            var Fn = De.prototype;
+            var Kn = De.prototype;
             Vn.prototype = function(e) {
                 return De().transition(e)
             }.prototype = {
                 constructor: Vn,
                 select: function(e) {
                     var t = this._name,
                         n = this._id;
@@ -2011,16 +2011,16 @@
                     for (var o = this._groups, r = o.length, a = [], s = [], i = 0; i < r; ++i)
                         for (var l, d = o[i], c = d.length, u = 0; u < c; ++u)
                             if (l = d[u]) {
                                 for (var g, h = e.call(l, l.__data__, u, d), p = Mt(l, n), f = 0, m = h.length; f < m; ++f)(g = h[f]) && wt(g, t, n, f, h, p);
                                 a.push(h), s.push(l)
                             } return new Vn(a, s, t, n)
                 },
-                selectChild: Fn.selectChild,
-                selectChildren: Fn.selectChildren,
+                selectChild: Kn.selectChild,
+                selectChildren: Kn.selectChildren,
                 filter: function(e) {
                     "function" != typeof e && (e = M(e));
                     for (var t = this._groups, n = t.length, o = new Array(n), r = 0; r < n; ++r)
                         for (var a, s = t[r], i = s.length, l = o[r] = [], d = 0; d < i; ++d)(a = s[d]) && e.call(a, a.__data__, d, s) && l.push(a);
                     return new Vn(o, this._parents, this._name, this._id)
                 },
                 merge: function(e) {
@@ -2042,20 +2042,20 @@
                                     time: c.time + c.delay + c.duration,
                                     delay: 0,
                                     duration: c.duration,
                                     ease: c.ease
                                 })
                             } return new Vn(o, this._parents, e, n)
                 },
-                call: Fn.call,
-                nodes: Fn.nodes,
-                node: Fn.node,
-                size: Fn.size,
-                empty: Fn.empty,
-                each: Fn.each,
+                call: Kn.call,
+                nodes: Kn.nodes,
+                node: Kn.node,
+                size: Kn.size,
+                empty: Kn.empty,
+                each: Kn.each,
                 on: function(e, t) {
                     var n = this._id;
                     return arguments.length < 2 ? Mt(this.node(), n).on.on(e) : this.each(function(e, t, n) {
                         var o, r, a = function(e) {
                             return (e + "").trim().split(/^|\s+/).every((function(e) {
                                 var t = e.indexOf(".");
                                 return t >= 0 && (e = e.slice(0, t)), !e || "start" === e
@@ -2227,17 +2227,17 @@
                         n.each((function() {
                             var n = Nt(this, o),
                                 r = n.on;
                             r !== e && ((t = (e = r).copy())._.cancel.push(i), t._.interrupt.push(i), t._.end.push(l)), n.on = t
                         })), 0 === r && a()
                     }))
                 },
-                [Symbol.iterator]: Fn[Symbol.iterator]
+                [Symbol.iterator]: Kn[Symbol.iterator]
             };
-            var Kn = {
+            var Fn = {
                 time: null,
                 delay: 0,
                 duration: 250,
                 ease: function(e) {
                     return ((e *= 2) <= 1 ? e * e * e : (e -= 2) * e * e + 2) / 2
                 }
             };
@@ -2249,15 +2249,15 @@
             }
             De.prototype.interrupt = function(e) {
                 return this.each((function() {
                     kt(this, e)
                 }))
             }, De.prototype.transition = function(e) {
                 var t, n;
-                e instanceof Vn ? (t = e._id, e = e._name) : (t = Zn(), (n = Kn).time = lt(), e = null == e ? null : e + "");
+                e instanceof Vn ? (t = e._id, e = e._name) : (t = Zn(), (n = Fn).time = lt(), e = null == e ? null : e + "");
                 for (var o = this._groups, r = o.length, a = 0; a < r; ++a)
                     for (var s, i = o[a], l = i.length, d = 0; d < l; ++d)(s = i[d]) && wt(s, e, t, d, i, n || Un(s, t));
                 return new Vn(o, this._parents, e, t)
             };
             const Wn = e => () => e;
 
             function Gn(e, {
@@ -2918,15 +2918,15 @@
                 targetControlX: s,
                 targetControlY: i
             }) {
                 const l = .125 * e + .375 * r + .375 * s + .125 * n,
                     d = .125 * t + .375 * a + .375 * i + .125 * o;
                 return [l, d, Math.abs(l - e), Math.abs(d - t)]
             }
-            var Zo, Fo, Ko, Uo, Wo, Go;
+            var Zo, Ko, Fo, Uo, Wo, Go;
 
             function qo({
                 pos: e,
                 x1: t,
                 y1: n,
                 x2: o,
                 y2: r
@@ -2966,18 +2966,18 @@
                 });
                 return [`M${e},${t} C${s},${i} ${l},${d} ${o},${r}`, c, u, g, h]
             }! function(e) {
                 e.Strict = "strict", e.Loose = "loose"
             }(Zo || (Zo = {})),
             function(e) {
                 e.Free = "free", e.Vertical = "vertical", e.Horizontal = "horizontal"
-            }(Fo || (Fo = {})),
+            }(Ko || (Ko = {})),
             function(e) {
                 e.Partial = "partial", e.Full = "full"
-            }(Ko || (Ko = {})),
+            }(Fo || (Fo = {})),
             function(e) {
                 e.Bezier = "default", e.Straight = "straight", e.Step = "step", e.SmoothStep = "smoothstep", e.SimpleBezier = "simplebezier"
             }(Uo || (Uo = {})),
             function(e) {
                 e.Arrow = "arrow", e.ArrowClosed = "arrowclosed"
             }(Wo || (Wo = {})),
             function(e) {
@@ -3887,27 +3887,27 @@
                     type: "source",
                     position: n,
                     isConnectable: t
                 })]
             });
             Vr.displayName = "InputNode";
             var Zr = (0, r.memo)(Vr);
-            const Fr = ({
+            const Kr = ({
                 data: e,
                 isConnectable: t,
                 targetPosition: n = Go.Top
             }) => (0, o.jsxs)(o.Fragment, {
                 children: [(0, o.jsx)(Hr, {
                     type: "target",
                     position: n,
                     isConnectable: t
                 }), e?.label]
             });
-            Fr.displayName = "OutputNode";
-            var Kr = (0, r.memo)(Fr);
+            Kr.displayName = "OutputNode";
+            var Fr = (0, r.memo)(Kr);
             const Ur = () => null;
             Ur.displayName = "GroupNode";
             const Wr = e => ({
                     selectedNodes: e.getNodes().filter((e => e.selected)),
                     selectedEdges: e.edges.filter((e => e.selected))
                 }),
                 Gr = e => e.id;
@@ -4007,18 +4007,18 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F
+                    isValidConnection: K
                 }) => {
                     const {
-                        setNodes: K,
+                        setNodes: F,
                         setEdges: U,
                         setDefaultNodesAndEdges: W,
                         setMinZoom: G,
                         setMaxZoom: q,
                         setTranslateExtent: Q,
                         setNodeExtent: J,
                         reset: ee
@@ -4027,15 +4027,15 @@
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return W(n, e), () => {
                             ee()
                         }
-                    }), []), oa("defaultEdgeOptions", P, te.setState), oa("connectionMode", w, te.setState), oa("onConnect", a, te.setState), oa("onConnectStart", s, te.setState), oa("onConnectEnd", i, te.setState), oa("onClickConnectStart", l, te.setState), oa("onClickConnectEnd", d, te.setState), oa("nodesDraggable", c, te.setState), oa("nodesConnectable", u, te.setState), oa("nodesFocusable", g, te.setState), oa("edgesFocusable", h, te.setState), oa("edgesUpdatable", p, te.setState), oa("elementsSelectable", E, te.setState), oa("elevateNodesOnSelect", m, te.setState), oa("snapToGrid", N, te.setState), oa("snapGrid", C, te.setState), oa("onNodesChange", b, te.setState), oa("onEdgesChange", v, te.setState), oa("connectOnClick", k, te.setState), oa("fitViewOnInit", O, te.setState), oa("fitViewOnInitOptions", I, te.setState), oa("onNodesDelete", A, te.setState), oa("onEdgesDelete", _, te.setState), oa("onNodeDrag", D, te.setState), oa("onNodeDragStart", R, te.setState), oa("onNodeDragStop", B, te.setState), oa("onSelectionDrag", z, te.setState), oa("onSelectionDragStart", $, te.setState), oa("onSelectionDragStop", T, te.setState), oa("noPanClassName", L, te.setState), oa("nodeOrigin", j, te.setState), oa("rfId", H, te.setState), oa("autoPanOnConnect", Y, te.setState), oa("autoPanOnNodeDrag", X, te.setState), oa("onError", V, te.setState), oa("connectionRadius", Z, te.setState), oa("isValidConnection", F, te.setState), na(e, K), na(t, U), na(y, G), na(S, q), na(M, Q), na(x, J), null
+                    }), []), oa("defaultEdgeOptions", P, te.setState), oa("connectionMode", w, te.setState), oa("onConnect", a, te.setState), oa("onConnectStart", s, te.setState), oa("onConnectEnd", i, te.setState), oa("onClickConnectStart", l, te.setState), oa("onClickConnectEnd", d, te.setState), oa("nodesDraggable", c, te.setState), oa("nodesConnectable", u, te.setState), oa("nodesFocusable", g, te.setState), oa("edgesFocusable", h, te.setState), oa("edgesUpdatable", p, te.setState), oa("elementsSelectable", E, te.setState), oa("elevateNodesOnSelect", m, te.setState), oa("snapToGrid", N, te.setState), oa("snapGrid", C, te.setState), oa("onNodesChange", b, te.setState), oa("onEdgesChange", v, te.setState), oa("connectOnClick", k, te.setState), oa("fitViewOnInit", O, te.setState), oa("fitViewOnInitOptions", I, te.setState), oa("onNodesDelete", A, te.setState), oa("onEdgesDelete", _, te.setState), oa("onNodeDrag", D, te.setState), oa("onNodeDragStart", R, te.setState), oa("onNodeDragStop", B, te.setState), oa("onSelectionDrag", z, te.setState), oa("onSelectionDragStart", $, te.setState), oa("onSelectionDragStop", T, te.setState), oa("noPanClassName", L, te.setState), oa("nodeOrigin", j, te.setState), oa("rfId", H, te.setState), oa("autoPanOnConnect", Y, te.setState), oa("autoPanOnNodeDrag", X, te.setState), oa("onError", V, te.setState), oa("connectionRadius", Z, te.setState), oa("isValidConnection", K, te.setState), na(e, F), na(t, U), na(y, G), na(S, q), na(M, Q), na(x, J), null
                 },
                 aa = {
                     display: "none"
                 },
                 sa = {
                     position: "absolute",
                     width: 1,
@@ -4147,17 +4147,17 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K
                 }) => {
-                    const K = (0, r.useRef)(null),
+                    const F = (0, r.useRef)(null),
                         [U, W] = (0, r.useState)(!1),
                         [G, q] = (0, r.useState)(!1),
                         Q = fo(),
                         J = (0, r.useMemo)((() => `url(#${br(j,H)})`), [j, H]),
                         ee = (0, r.useMemo)((() => `url(#${br(L,H)})`), [L, H]);
                     if (P) return null;
                     const te = Yo(t, Q.getState, d),
@@ -4216,25 +4216,25 @@
                         onKeyDown: X ? e => {
                             if (Bo.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
                                 } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                "Escape" === e.key ? (F.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : void 0,
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${la}-${H}` : void 0,
-                        ref: K,
+                        ref: F,
                         children: [!G && (0, o.jsx)(e, {
                             id: t,
                             source: x,
                             target: b,
                             selected: c,
                             animated: u,
                             label: g,
@@ -4252,15 +4252,15 @@
                             sourcePosition: N,
                             targetPosition: M,
                             sourceHandleId: O,
                             targetHandleId: I,
                             markerStart: J,
                             markerEnd: ee,
                             pathOptions: Z,
-                            interactionWidth: F
+                            interactionWidth: K
                         }), V && (0, o.jsxs)(o.Fragment, {
                             children: [("source" === V || !0 === V) && (0, o.jsx)(ma, {
                                 position: N,
                                 centerX: v,
                                 centerY: E,
                                 radius: B,
                                 onMouseDown: e => se(e, !0),
@@ -4737,16 +4737,16 @@
                         L = (0, r.useRef)(null),
                         j = (0, r.useRef)(N),
                         H = (0, r.useRef)(M),
                         Y = (0, r.useRef)(n),
                         X = v || b || g || h || p || f,
                         V = Ra(),
                         Z = Oa(t, T.getState, h),
-                        F = Oa(t, T.getState, p),
-                        K = Oa(t, T.getState, f),
+                        K = Oa(t, T.getState, p),
+                        F = Oa(t, T.getState, f),
                         U = Oa(t, T.getState, m),
                         W = Oa(t, T.getState, y);
                     (0, r.useEffect)((() => {
                         if (L.current && !k) {
                             const e = L.current;
                             return P?.observe(e), () => P?.unobserve(e)
                         }
@@ -4785,16 +4785,16 @@
                             pointerEvents: X ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: Z,
-                        onMouseMove: F,
-                        onMouseLeave: K,
+                        onMouseMove: K,
+                        onMouseLeave: F,
                         onContextMenu: U,
                         onClick: e => {
                             if (!v || C && b || Ia({
                                     id: t,
                                     store: T,
                                     nodeRef: L
                                 }), g) {
@@ -4849,15 +4849,15 @@
                 return t.displayName = "NodeWrapper", (0, r.memo)(t)
             };
 
             function $a(e) {
                 return {
                     input: za(e.input || Zr),
                     default: za(e.default || Xr),
-                    output: za(e.output || Kr),
+                    output: za(e.output || Fr),
                     group: za(e.group || Ur),
                     ...Object.keys(e).filter((e => !["input", "default", "output", "group"].includes(e))).reduce(((t, n) => (t[n] = za(e[n] || Xr), t)), {})
                 }
             }
             const Ta = "undefined" != typeof document ? document : null;
             var La = (e = null, t = {
                 target: Ta
@@ -4985,26 +4985,26 @@
                             h = Qn.translate(d, c).scale(g);
                         return "number" == typeof t.duration && t.duration > 0 ? i.transform(Ir(l, t.duration), h) : i.transform(l, h), !0
                     }
                 }
                 return !1
             }
 
-            function Fa(e, t) {
+            function Ka(e, t) {
                 return e.forEach((e => {
                     const n = t.get(e.id);
                     n && t.set(n.id, {
                         ...n,
                         [Ro]: n[Ro],
                         selected: e.selected
                     })
                 })), new Map(t)
             }
 
-            function Ka(e, t) {
+            function Fa(e, t) {
                 return t.map((t => {
                     const n = e.find((e => e.id === t.id));
                     return n && (t.selected = n.selected), t
                 }))
             }
 
             function Ua({
@@ -5018,17 +5018,17 @@
                     edges: a,
                     onNodesChange: s,
                     onEdgesChange: i,
                     hasDefaultNodes: l,
                     hasDefaultEdges: d
                 } = n();
                 e?.length && (l && o({
-                    nodeInternals: Fa(e, r)
+                    nodeInternals: Ka(e, r)
                 }), s?.(e)), t?.length && (d && o({
-                    edges: Ka(t, a)
+                    edges: Fa(t, a)
                 }), i?.(t))
             }
             const Wa = () => {},
                 Ga = {
                     zoomIn: Wa,
                     zoomOut: Wa,
                     zoomTo: Wa,
@@ -5304,15 +5304,15 @@
                     onMoveStart: t,
                     onMoveEnd: n,
                     onPaneContextMenu: a,
                     zoomOnScroll: s = !0,
                     zoomOnPinch: i = !0,
                     panOnScroll: l = !1,
                     panOnScrollSpeed: d = .5,
-                    panOnScrollMode: c = Fo.Free,
+                    panOnScrollMode: c = Ko.Free,
                     zoomOnDoubleClick: u = !0,
                     elementsSelectable: g,
                     panOnDrag: h = !0,
                     defaultViewport: p,
                     translateExtent: m,
                     minZoom: y,
                     maxZoom: S,
@@ -5388,16 +5388,16 @@
                             if (e.ctrlKey && i) {
                                 const n = Be(e),
                                     o = -e.deltaY * (1 === e.deltaMode ? .05 : e.deltaMode ? 1 : .002) * 10,
                                     r = t * Math.pow(2, o);
                                 return void I.scaleTo(A, r, n)
                             }
                             const n = 1 === e.deltaMode ? 20 : 1,
-                                o = c === Fo.Vertical ? 0 : e.deltaX * n,
-                                r = c === Fo.Horizontal ? 0 : e.deltaY * n;
+                                o = c === Ko.Vertical ? 0 : e.deltaX * n,
+                                r = c === Ko.Horizontal ? 0 : e.deltaY * n;
                             I.translateBy(A, -o / t * d, -r / t * d)
                         }), {
                             passive: !1
                         }))
                     }), [D, l, c, A, I, _, R, i, b, E]), (0, r.useEffect)((() => {
                         I && I.on("start", (e => {
                             if (!e.sourceEvent) return null;
@@ -5560,15 +5560,15 @@
                 fs = e => ({
                     userSelectionActive: e.userSelectionActive,
                     elementsSelectable: e.elementsSelectable,
                     dragging: e.paneDragging
                 }),
                 ms = (0, r.memo)((({
                     isSelecting: e,
-                    selectionMode: t = Ko.Full,
+                    selectionMode: t = Fo.Full,
                     panOnDrag: n,
                     onSelectionStart: a,
                     onSelectionEnd: i,
                     onPaneClick: l,
                     onPaneContextMenu: d,
                     onPaneScroll: c,
                     onPaneMouseEnter: u,
@@ -5654,15 +5654,15 @@
                                     ...o,
                                     x: u.x < g ? u.x : g,
                                     y: u.y < h ? u.y : h,
                                     width: Math.abs(u.x - g),
                                     height: Math.abs(u.y - h)
                                 },
                                 f = c(),
-                                m = kr(r, p, s, t === Ko.Partial, !0, d),
+                                m = kr(r, p, s, t === Fo.Partial, !0, d),
                                 v = Pr(m, a).map((e => e.id)),
                                 E = m.map((e => e.id));
                             if (S.current !== E.length) {
                                 S.current = E.length;
                                 const e = hs(f, E);
                                 e.length && i?.(e)
                             }
@@ -6453,16 +6453,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -6482,16 +6482,16 @@
             }) => (function(e) {
                 const t = Ja(),
                     n = (0, r.useRef)(!1);
                 (0, r.useEffect)((() => {
                     !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                 }), [e, t.viewportInitialized])
             }(i), (0, o.jsx)(vs, {
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneContextMenu: q,
                 onPaneScroll: G,
                 deleteKeyCode: O,
                 selectionKeyCode: w,
                 selectionOnDrag: C,
@@ -6882,21 +6882,21 @@
                 children: e
             });
 
             function Zs(e, t) {
                 return (0, r.useRef)(null), (0, r.useMemo)((() => t(e)), [e])
             }
             Vs.displayName = "ReactFlowWrapper";
-            const Fs = {
+            const Ks = {
                     input: Zr,
                     default: Xr,
-                    output: Kr,
+                    output: Fr,
                     group: Ur
                 },
-                Ks = {
+                Fs = {
                     default: ur,
                     straight: ir,
                     step: ar,
                     smoothstep: rr,
                     simplebezier: Jo
                 },
                 Us = [0, 0],
@@ -6915,16 +6915,16 @@
                 },
                 Qs = (0, r.forwardRef)((({
                     nodes: e,
                     edges: t,
                     defaultNodes: n,
                     defaultEdges: r,
                     className: a,
-                    nodeTypes: i = Fs,
-                    edgeTypes: l = Ks,
+                    nodeTypes: i = Ks,
+                    edgeTypes: l = Fs,
                     onNodeClick: d,
                     onEdgeClick: c,
                     onInit: u,
                     onMove: g,
                     onMoveStart: h,
                     onMoveEnd: p,
                     onConnect: f,
@@ -6953,17 +6953,17 @@
                     connectionLineType: T = Uo.Bezier,
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
-                    selectionMode: Z = Ko.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = "Meta",
+                    selectionMode: Z = Fo.Full,
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = "Meta",
                     zoomActivationKeyCode: U = "Meta",
                     snapToGrid: W = !1,
                     snapGrid: G = Ws,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -6979,15 +6979,15 @@
                     preventScrolling: ce = !0,
                     nodeExtent: ue,
                     defaultMarkerColor: ge = "#b1b1b7",
                     zoomOnScroll: he = !0,
                     zoomOnPinch: pe = !0,
                     panOnScroll: fe = !1,
                     panOnScrollSpeed: me = .5,
-                    panOnScrollMode: ye = Fo.Free,
+                    panOnScrollMode: ye = Ko.Free,
                     zoomOnDoubleClick: Se = !0,
                     panOnDrag: xe = !0,
                     onPaneClick: be,
                     onPaneMouseEnter: ve,
                     onPaneMouseMove: Ee,
                     onPaneMouseLeave: we,
                     onPaneScroll: Ce,
@@ -7008,16 +7008,16 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
@@ -7057,16 +7057,16 @@
                                 connectionLineStyle: L,
                                 connectionLineComponent: j,
                                 connectionLineContainerStyle: H,
                                 selectionKeyCode: X,
                                 selectionOnDrag: V,
                                 selectionMode: Z,
                                 deleteKeyCode: Y,
-                                multiSelectionKeyCode: K,
-                                panActivationKeyCode: F,
+                                multiSelectionKeyCode: F,
+                                panActivationKeyCode: K,
                                 zoomActivationKeyCode: U,
                                 onlyRenderVisibleElements: q,
                                 selectNodesOnDrag: Q,
                                 defaultViewport: se,
                                 translateExtent: de,
                                 minZoom: ie,
                                 maxZoom: le,
@@ -7117,26 +7117,26 @@
                                 onClickConnectEnd: x,
                                 nodesDraggable: J,
                                 nodesConnectable: ee,
                                 nodesFocusable: te,
                                 edgesFocusable: oe,
                                 edgesUpdatable: re,
                                 elementsSelectable: ae,
-                                elevateNodesOnSelect: Ke,
+                                elevateNodesOnSelect: Fe,
                                 minZoom: ie,
                                 maxZoom: le,
                                 nodeExtent: ue,
                                 onNodesChange: ze,
                                 onEdgesChange: $e,
                                 snapToGrid: W,
                                 snapGrid: G,
                                 connectionMode: $,
                                 translateExtent: de,
                                 connectOnClick: Xe,
-                                defaultEdgeOptions: Fe,
+                                defaultEdgeOptions: Ke,
                                 fitView: He,
                                 fitViewOptions: Ye,
                                 onNodesDelete: P,
                                 onEdgesDelete: O,
                                 onNodeDragStart: N,
                                 onNodeDrag: M,
                                 onNodeDragStop: k,
@@ -7507,27 +7507,27 @@
                     const r = t().edges.find((t => t.id === e));
                     r && n(o, {
                         ...r
                     })
                 }
             }
 
-            function Fi({
+            function Ki({
                 sourceX: e,
                 sourceY: t,
                 targetX: n,
                 targetY: o
             }) {
                 const r = Math.abs(n - e) / 2,
                     a = n < e ? n + r : n - r,
                     s = Math.abs(o - t) / 2;
                 return [a, o < t ? o + s : o - s, r, s]
             }
 
-            function Ki({
+            function Fi({
                 sourceX: e,
                 sourceY: t,
                 targetX: n,
                 targetY: o,
                 sourceControlX: r,
                 sourceControlY: a,
                 targetControlX: s,
@@ -7565,15 +7565,15 @@
                     y2: r
                 }), [l, d] = el({
                     pos: a,
                     x1: o,
                     y1: r,
                     x2: e,
                     y2: t
-                }), [c, u, g, h] = Ki({
+                }), [c, u, g, h] = Fi({
                     sourceX: e,
                     sourceY: t,
                     targetX: o,
                     targetY: r,
                     sourceControlX: s,
                     sourceControlY: i,
                     targetControlX: l,
@@ -7713,15 +7713,15 @@
                             source: l,
                             sourcePosition: t,
                             target: d
                         }),
                         u = 0 !== c.x ? "x" : "y",
                         g = c[u];
                     let h, p, f = [];
-                    const [m, y, S, x] = Fi({
+                    const [m, y, S, x] = Ki({
                         sourceX: e.x,
                         sourceY: e.y,
                         targetX: n.x,
                         targetY: n.y
                     });
                     if (s[u] * i[u] == -1) {
                         h = r.x || m, p = r.y || y;
@@ -7865,15 +7865,15 @@
             }) => {
                 const [f, m, y] = function({
                     sourceX: e,
                     sourceY: t,
                     targetX: n,
                     targetY: o
                 }) {
-                    const [r, a, s, i] = Fi({
+                    const [r, a, s, i] = Ki({
                         sourceX: e,
                         sourceY: t,
                         targetX: n,
                         targetY: o
                     });
                     return [`M ${e},${t}L ${n},${o}`, r, a, s, i]
                 }({
@@ -7942,15 +7942,15 @@
                 }), [d, c] = cl({
                     pos: a,
                     x1: o,
                     y1: r,
                     x2: e,
                     y2: t,
                     c: s
-                }), [u, g, h, p] = Ki({
+                }), [u, g, h, p] = Fi({
                     sourceX: e,
                     sourceY: t,
                     targetX: o,
                     targetY: r,
                     sourceControlX: i,
                     sourceControlY: l,
                     targetControlX: d,
@@ -8493,15 +8493,15 @@
                     selectedEdges: e.edges.filter((e => e.selected))
                 }),
                 Vl = e => e.id;
 
             function Zl(e, t) {
                 return f(e.selectedNodes.map(Vl), t.selectedNodes.map(Vl)) && f(e.selectedEdges.map(Vl), t.selectedEdges.map(Vl))
             }
-            const Fl = (0, r.memo)((({
+            const Kl = (0, r.memo)((({
                 onSelectionChange: e
             }) => {
                 const t = vi(),
                     {
                         selectedNodes: n,
                         selectedEdges: o
                     } = bi(Xl, Zl);
@@ -8509,22 +8509,22 @@
                     const r = {
                         nodes: n,
                         edges: o
                     };
                     e?.(r), t.getState().onSelectionChange?.(r)
                 }), [n, o, e]), null
             }));
-            Fl.displayName = "SelectionListener";
-            const Kl = e => !!e.onSelectionChange;
+            Kl.displayName = "SelectionListener";
+            const Fl = e => !!e.onSelectionChange;
 
             function Ul({
                 onSelectionChange: e
             }) {
-                const t = bi(Kl);
-                return e || t ? (0, o.jsx)(Fl, {
+                const t = bi(Fl);
+                return e || t ? (0, o.jsx)(Kl, {
                     onSelectionChange: e
                 }) : null
             }
             const Wl = e => ({
                 setNodes: e.setNodes,
                 setEdges: e.setEdges,
                 setDefaultNodesAndEdges: e.setDefaultNodesAndEdges,
@@ -8589,18 +8589,18 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F
+                    isValidConnection: K
                 }) => {
                     const {
-                        setNodes: K,
+                        setNodes: F,
                         setEdges: U,
                         setDefaultNodesAndEdges: W,
                         setMinZoom: G,
                         setMaxZoom: q,
                         setTranslateExtent: Q,
                         setNodeExtent: J,
                         reset: ee
@@ -8609,15 +8609,15 @@
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return W(n, e), () => {
                             ee()
                         }
-                    }), []), ql("defaultEdgeOptions", P, te.setState), ql("connectionMode", w, te.setState), ql("onConnect", a, te.setState), ql("onConnectStart", s, te.setState), ql("onConnectEnd", i, te.setState), ql("onClickConnectStart", l, te.setState), ql("onClickConnectEnd", d, te.setState), ql("nodesDraggable", c, te.setState), ql("nodesConnectable", u, te.setState), ql("nodesFocusable", g, te.setState), ql("edgesFocusable", h, te.setState), ql("edgesUpdatable", p, te.setState), ql("elementsSelectable", E, te.setState), ql("elevateNodesOnSelect", m, te.setState), ql("snapToGrid", N, te.setState), ql("snapGrid", C, te.setState), ql("onNodesChange", b, te.setState), ql("onEdgesChange", v, te.setState), ql("connectOnClick", k, te.setState), ql("fitViewOnInit", O, te.setState), ql("fitViewOnInitOptions", I, te.setState), ql("onNodesDelete", A, te.setState), ql("onEdgesDelete", _, te.setState), ql("onNodeDrag", D, te.setState), ql("onNodeDragStart", R, te.setState), ql("onNodeDragStop", B, te.setState), ql("onSelectionDrag", z, te.setState), ql("onSelectionDragStart", $, te.setState), ql("onSelectionDragStop", T, te.setState), ql("noPanClassName", L, te.setState), ql("nodeOrigin", j, te.setState), ql("rfId", H, te.setState), ql("autoPanOnConnect", Y, te.setState), ql("autoPanOnNodeDrag", X, te.setState), ql("onError", V, te.setState), ql("connectionRadius", Z, te.setState), ql("isValidConnection", F, te.setState), Gl(e, K), Gl(t, U), Gl(y, G), Gl(S, q), Gl(M, Q), Gl(x, J), null
+                    }), []), ql("defaultEdgeOptions", P, te.setState), ql("connectionMode", w, te.setState), ql("onConnect", a, te.setState), ql("onConnectStart", s, te.setState), ql("onConnectEnd", i, te.setState), ql("onClickConnectStart", l, te.setState), ql("onClickConnectEnd", d, te.setState), ql("nodesDraggable", c, te.setState), ql("nodesConnectable", u, te.setState), ql("nodesFocusable", g, te.setState), ql("edgesFocusable", h, te.setState), ql("edgesUpdatable", p, te.setState), ql("elementsSelectable", E, te.setState), ql("elevateNodesOnSelect", m, te.setState), ql("snapToGrid", N, te.setState), ql("snapGrid", C, te.setState), ql("onNodesChange", b, te.setState), ql("onEdgesChange", v, te.setState), ql("connectOnClick", k, te.setState), ql("fitViewOnInit", O, te.setState), ql("fitViewOnInitOptions", I, te.setState), ql("onNodesDelete", A, te.setState), ql("onEdgesDelete", _, te.setState), ql("onNodeDrag", D, te.setState), ql("onNodeDragStart", R, te.setState), ql("onNodeDragStop", B, te.setState), ql("onSelectionDrag", z, te.setState), ql("onSelectionDragStart", $, te.setState), ql("onSelectionDragStop", T, te.setState), ql("noPanClassName", L, te.setState), ql("nodeOrigin", j, te.setState), ql("rfId", H, te.setState), ql("autoPanOnConnect", Y, te.setState), ql("autoPanOnNodeDrag", X, te.setState), ql("onError", V, te.setState), ql("connectionRadius", Z, te.setState), ql("isValidConnection", K, te.setState), Gl(e, F), Gl(t, U), Gl(y, G), Gl(S, q), Gl(M, Q), Gl(x, J), null
                 },
                 Jl = {
                     display: "none"
                 },
                 ed = {
                     position: "absolute",
                     width: 1,
@@ -8729,17 +8729,17 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K
                 }) => {
-                    const K = (0, r.useRef)(null),
+                    const F = (0, r.useRef)(null),
                         [U, W] = (0, r.useState)(!1),
                         [G, q] = (0, r.useState)(!1),
                         Q = vi(),
                         J = (0, r.useMemo)((() => `url(#${ml(j,H)})`), [j, H]),
                         ee = (0, r.useMemo)((() => `url(#${ml(L,H)})`), [L, H]);
                     if (P) return null;
                     const te = Zi(t, Q.getState, d),
@@ -8798,25 +8798,25 @@
                         onKeyDown: X ? e => {
                             if (Li.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
                                 } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                "Escape" === e.key ? (F.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : void 0,
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${nd}-${H}` : void 0,
-                        ref: K,
+                        ref: F,
                         children: [!G && (0, o.jsx)(e, {
                             id: t,
                             source: x,
                             target: b,
                             selected: c,
                             animated: u,
                             label: g,
@@ -8834,15 +8834,15 @@
                             sourcePosition: N,
                             targetPosition: M,
                             sourceHandleId: O,
                             targetHandleId: I,
                             markerStart: J,
                             markerEnd: ee,
                             pathOptions: Z,
-                            interactionWidth: F
+                            interactionWidth: K
                         }), V && (0, o.jsxs)(o.Fragment, {
                             children: [("source" === V || !0 === V) && (0, o.jsx)(cd, {
                                 position: N,
                                 centerX: v,
                                 centerY: E,
                                 radius: B,
                                 onMouseDown: e => se(e, !0),
@@ -9317,16 +9317,16 @@
                         L = (0, r.useRef)(null),
                         j = (0, r.useRef)(N),
                         H = (0, r.useRef)(M),
                         Y = (0, r.useRef)(n),
                         X = v || b || g || h || p || f,
                         V = kd(),
                         Z = wd(t, T.getState, h),
-                        F = wd(t, T.getState, p),
-                        K = wd(t, T.getState, f),
+                        K = wd(t, T.getState, p),
+                        F = wd(t, T.getState, f),
                         U = wd(t, T.getState, m),
                         W = wd(t, T.getState, y);
                     (0, r.useEffect)((() => {
                         if (L.current && !k) {
                             const e = L.current;
                             return P?.observe(e), () => P?.unobserve(e)
                         }
@@ -9365,16 +9365,16 @@
                             pointerEvents: X ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: Z,
-                        onMouseMove: F,
-                        onMouseLeave: K,
+                        onMouseMove: K,
+                        onMouseLeave: F,
                         onContextMenu: U,
                         onClick: e => {
                             if (!v || C && b || Cd({
                                     id: t,
                                     store: T,
                                     nodeRef: L
                                 }), g) {
@@ -9855,22 +9855,22 @@
                     addEdges: c,
                     toObject: u,
                     deleteElements: g,
                     getIntersectingNodes: p,
                     isNodeIntersecting: m
                 })), [e, n, o, a, s, i, l, d, c, u, g, p, m])
             }
-            const Fd = {
+            const Kd = {
                     position: "absolute",
                     width: "100%",
                     height: "100%",
                     top: 0,
                     left: 0
                 },
-                Kd = e => ({
+                Fd = e => ({
                     x: e.x,
                     y: e.y,
                     zoom: e.k
                 }),
                 Ud = (e, t) => e.target.closest(`.${t}`),
                 Wd = (e, t) => 2 === t && Array.isArray(e) && e.includes(2),
                 Gd = e => ({
@@ -9984,40 +9984,40 @@
                             B.current = e.sourceEvent.button;
                             const {
                                 onViewportChangeStart: n
                             } = N.getState();
                             if (M.current = !0, "mousedown" === e.sourceEvent?.type && N.setState({
                                     paneDragging: !0
                                 }), t || n) {
-                                const o = Kd(e.transform);
+                                const o = Fd(e.transform);
                                 O.current = o, n?.(o), t?.(e.sourceEvent, o)
                             }
                         }))
                     }), [I, t]), (0, r.useEffect)((() => {
                         I && (D && !M.current ? I.on("zoom", null) : D || I.on("zoom", (t => {
                             const {
                                 onViewportChange: n
                             } = N.getState();
                             if (N.setState({
                                     transform: [t.transform.x, t.transform.y, t.transform.k]
                                 }), k.current = !(!a || !Wd(h, B.current ?? 0)), e || n) {
-                                const o = Kd(t.transform);
+                                const o = Fd(t.transform);
                                 n?.(o), e?.(t.sourceEvent, o)
                             }
                         })))
                     }), [D, I, e, h, a]), (0, r.useEffect)((() => {
                         I && I.on("end", (e => {
                             if (!e.sourceEvent) return null;
                             const {
                                 onViewportChangeEnd: t
                             } = N.getState();
                             if (M.current = !1, N.setState({
                                     paneDragging: !1
                                 }), a && Wd(h, B.current ?? 0) && !k.current && a(e.sourceEvent), k.current = !1, (n || t) && (o = O.current, r = e.transform, o.x !== r.x || o.y !== r.y || o.zoom !== r.k)) {
-                                const o = Kd(e.transform);
+                                const o = Fd(e.transform);
                                 O.current = o, clearTimeout(C.current), C.current = setTimeout((() => {
                                     t?.(o), n?.(e.sourceEvent, o)
                                 }), l ? 150 : 0)
                             }
                             var o, r
                         }))
                     }), [I, l, h, n, a]), (0, r.useEffect)((() => {
@@ -10036,15 +10036,15 @@
                             if (Array.isArray(h) && !h.includes(e.button) && ("mousedown" === e.type || "touchstart" === e.type)) return !1;
                             const o = Array.isArray(h) && h.includes(e.button) || !e.button || e.button <= 1;
                             return (!e.ctrlKey || "wheel" === e.type) && o
                         }))
                     }), [D, I, s, i, l, u, h, g, R]), (0, o.jsx)("div", {
                         className: "react-flow__renderer",
                         ref: P,
-                        style: Fd,
+                        style: Kd,
                         children: v
                     })
                 },
                 Qd = e => ({
                     userSelectionActive: e.userSelectionActive,
                     userSelectionRect: e.userSelectionRect
                 });
@@ -10262,15 +10262,15 @@
                         } : void 0,
                         onMouseLeave: k ? e => {
                             v && (y.setState({
                                 nodesSelectionActive: S.current > 0
                             }), i?.(e)), C()
                         } : h,
                         ref: m,
-                        style: Fd,
+                        style: Kd,
                         children: [p, (0, o.jsx)(Jd, {})]
                     })
                 }));
             ic.displayName = "Pane";
             const lc = e => {
                 const t = e.getNodes().filter((e => e.selected));
                 return {
@@ -10485,15 +10485,15 @@
                             }));
                             return u.current = e, e
                         }), []);
                     return (0, r.useEffect)((() => () => {
                         u?.current?.disconnect()
                     }), []), (0, o.jsx)("div", {
                         className: "react-flow__nodes",
-                        style: Fd,
+                        style: Kd,
                         children: d.map((r => {
                             let i = r.type || "default";
                             e.nodeTypes[i] || (l?.("003", Si.error003(i)), i = "default");
                             const d = e.nodeTypes[i] || e.nodeTypes.default,
                                 c = !!(r.draggable || t && void 0 === r.draggable),
                                 u = !!(r.selectable || s && void 0 === r.selectable),
                                 h = !!(r.connectable || n && void 0 === r.connectable),
@@ -11029,16 +11029,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -11058,16 +11058,16 @@
             }) => (function(e) {
                 const t = Zd(),
                     n = (0, r.useRef)(!1);
                 (0, r.useEffect)((() => {
                     !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                 }), [e, t.viewportInitialized])
             }(i), (0, o.jsx)(gc, {
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneContextMenu: q,
                 onPaneScroll: G,
                 deleteKeyCode: O,
                 selectionKeyCode: w,
                 selectionOnDrag: C,
@@ -11530,16 +11530,16 @@
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
                     selectionMode: Z = Gi.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = "Meta",
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = "Meta",
                     zoomActivationKeyCode: U = "Meta",
                     snapToGrid: W = !1,
                     snapGrid: G = jc,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -11584,16 +11584,16 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
@@ -11633,16 +11633,16 @@
                                 connectionLineStyle: L,
                                 connectionLineComponent: j,
                                 connectionLineContainerStyle: H,
                                 selectionKeyCode: X,
                                 selectionOnDrag: V,
                                 selectionMode: Z,
                                 deleteKeyCode: Y,
-                                multiSelectionKeyCode: K,
-                                panActivationKeyCode: F,
+                                multiSelectionKeyCode: F,
+                                panActivationKeyCode: K,
                                 zoomActivationKeyCode: U,
                                 onlyRenderVisibleElements: q,
                                 selectNodesOnDrag: Q,
                                 defaultViewport: se,
                                 translateExtent: de,
                                 minZoom: ie,
                                 maxZoom: le,
@@ -11693,26 +11693,26 @@
                                 onClickConnectEnd: x,
                                 nodesDraggable: J,
                                 nodesConnectable: ee,
                                 nodesFocusable: te,
                                 edgesFocusable: oe,
                                 edgesUpdatable: re,
                                 elementsSelectable: ae,
-                                elevateNodesOnSelect: Ke,
+                                elevateNodesOnSelect: Fe,
                                 minZoom: ie,
                                 maxZoom: le,
                                 nodeExtent: ue,
                                 onNodesChange: ze,
                                 onEdgesChange: $e,
                                 snapToGrid: W,
                                 snapGrid: G,
                                 connectionMode: $,
                                 translateExtent: de,
                                 connectOnClick: Xe,
-                                defaultEdgeOptions: Fe,
+                                defaultEdgeOptions: Ke,
                                 fitView: He,
                                 fitViewOptions: Ye,
                                 onNodesDelete: P,
                                 onEdgesDelete: O,
                                 onNodeDragStart: N,
                                 onNodeDrag: M,
                                 onNodeDragStop: k,
@@ -11780,16 +11780,16 @@
                     stroke: d,
                     strokeWidth: c,
                     shapeRendering: h,
                     onClick: p ? t => p(t, e) : void 0
                 })
             };
             Zc.displayName = "MiniMapNode";
-            var Fc = (0, r.memo)(Zc);
-            const Kc = e => {
+            var Kc = (0, r.memo)(Zc);
+            const Fc = e => {
                     const t = e.getNodes(),
                         n = {
                             x: -e.transform[0] / e.transform[2],
                             y: -e.transform[1] / e.transform[2],
                             width: e.width / e.transform[2],
                             height: e.height / e.transform[2]
                         };
@@ -11808,15 +11808,15 @@
                 style: e,
                 className: t,
                 nodeStrokeColor: n = "transparent",
                 nodeColor: a = "#e2e2e2",
                 nodeClassName: i = "",
                 nodeBorderRadius: l = 5,
                 nodeStrokeWidth: d = 2,
-                nodeComponent: c = Fc,
+                nodeComponent: c = Kc,
                 maskColor: u = "rgb(240, 240, 240, 0.6)",
                 maskStrokeColor: g = "none",
                 maskStrokeWidth: h = 1,
                 position: p = "bottom-right",
                 onClick: m,
                 onNodeClick: y,
                 pannable: S = !1,
@@ -11829,15 +11829,15 @@
                     C = (0, r.useRef)(null),
                     {
                         boundingRect: N,
                         viewBB: M,
                         nodes: k,
                         rfId: P,
                         nodeOrigin: O
-                    } = bi(Kc, f),
+                    } = bi(Fc, f),
                     I = e?.width ?? 200,
                     A = e?.height ?? 150,
                     _ = Uc(a),
                     D = Uc(n),
                     R = Uc(i),
                     B = N.width / I,
                     z = N.height / A,
@@ -11846,17 +11846,17 @@
                     L = $ * A,
                     j = 5 * $,
                     H = N.x - (T - N.width) / 2 - j,
                     Y = N.y - (L - N.height) / 2 - j,
                     X = T + 2 * j,
                     V = L + 2 * j,
                     Z = "undefined" == typeof window || window.chrome ? "crispEdges" : "geometricPrecision",
-                    F = `react-flow__minimap-desc-${P}`,
-                    K = (0, r.useRef)(0);
-                K.current = $, (0, r.useEffect)((() => {
+                    K = `react-flow__minimap-desc-${P}`,
+                    F = (0, r.useRef)(0);
+                F.current = $, (0, r.useEffect)((() => {
                     if (C.current) {
                         const e = Re(C.current),
                             t = e => {
                                 const {
                                     transform: t,
                                     d3Selection: n,
                                     d3Zoom: o
@@ -11872,15 +11872,15 @@
                                     d3Selection: n,
                                     d3Zoom: o,
                                     translateExtent: r,
                                     width: a,
                                     height: s
                                 } = w.getState();
                                 if ("mousemove" !== e.sourceEvent.type || !n || !o) return;
-                                const i = K.current * Math.max(1, t[2]) * (v ? -1 : 1),
+                                const i = F.current * Math.max(1, t[2]) * (v ? -1 : 1),
                                     l = {
                                         x: t[0] - e.sourceEvent.movementX * i,
                                         y: t[1] - e.sourceEvent.movementY * i
                                     },
                                     d = [
                                         [0, 0],
                                         [a, s]
@@ -11912,19 +11912,19 @@
                     className: s(["react-flow__minimap", t]),
                     "data-testid": "rf__minimap",
                     children: (0, o.jsxs)("svg", {
                         width: I,
                         height: A,
                         viewBox: `${H} ${Y} ${X} ${V}`,
                         role: "img",
-                        "aria-labelledby": F,
+                        "aria-labelledby": K,
                         ref: C,
                         onClick: U,
                         children: [b && (0, o.jsx)("title", {
-                            id: F,
+                            id: K,
                             children: b
                         }), k.map((e => {
                             const {
                                 x: t,
                                 y: n
                             } = xl(e, O).positionAbsolute;
                             return (0, o.jsx)(c, {
@@ -12681,17 +12681,17 @@
                     style: h,
                     markerEnd: p,
                     markerStart: f,
                     interactionWidth: y
                 })
             }));
             Zu.displayName = "BezierEdge";
-            const Fu = (0, r.createContext)(null),
-                Ku = Fu.Provider;
-            Fu.Consumer;
+            const Ku = (0, r.createContext)(null),
+                Fu = Ku.Provider;
+            Ku.Consumer;
             const Uu = ({
                     source: e,
                     sourceHandle: t,
                     target: n,
                     targetHandle: o
                 }) => `reactflow__edge-${e}${t||""}-${n}${o||""}`,
                 Wu = (e, t) => void 0 === e ? "" : "string" == typeof e ? e : `${t?`${t}__`:""}${Object.keys(e).sort().map((t=>`${t}=${e[t]}`)).join("&")}`,
@@ -13015,15 +13015,15 @@
                     onMouseDown: h,
                     onTouchStart: p,
                     ...m
                 }, y) => {
                     const S = d || null,
                         x = "target" === e,
                         b = nu(),
-                        v = (0, r.useContext)(Fu),
+                        v = (0, r.useContext)(Ku),
                         {
                             connectOnClick: E,
                             noPanClassName: w
                         } = tu(gg, f),
                         {
                             connecting: C,
                             clickConnecting: N
@@ -13285,18 +13285,18 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F
+                    isValidConnection: K
                 }) => {
                     const {
-                        setNodes: K,
+                        setNodes: F,
                         setEdges: U,
                         setDefaultNodesAndEdges: W,
                         setMinZoom: G,
                         setMaxZoom: q,
                         setTranslateExtent: Q,
                         setNodeExtent: J,
                         reset: ee
@@ -13305,15 +13305,15 @@
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return W(n, e), () => {
                             ee()
                         }
-                    }), []), Ig("defaultEdgeOptions", P, te.setState), Ig("connectionMode", w, te.setState), Ig("onConnect", a, te.setState), Ig("onConnectStart", s, te.setState), Ig("onConnectEnd", i, te.setState), Ig("onClickConnectStart", l, te.setState), Ig("onClickConnectEnd", d, te.setState), Ig("nodesDraggable", c, te.setState), Ig("nodesConnectable", u, te.setState), Ig("nodesFocusable", g, te.setState), Ig("edgesFocusable", h, te.setState), Ig("edgesUpdatable", p, te.setState), Ig("elementsSelectable", E, te.setState), Ig("elevateNodesOnSelect", m, te.setState), Ig("snapToGrid", N, te.setState), Ig("snapGrid", C, te.setState), Ig("onNodesChange", b, te.setState), Ig("onEdgesChange", v, te.setState), Ig("connectOnClick", k, te.setState), Ig("fitViewOnInit", O, te.setState), Ig("fitViewOnInitOptions", I, te.setState), Ig("onNodesDelete", A, te.setState), Ig("onEdgesDelete", _, te.setState), Ig("onNodeDrag", D, te.setState), Ig("onNodeDragStart", R, te.setState), Ig("onNodeDragStop", B, te.setState), Ig("onSelectionDrag", z, te.setState), Ig("onSelectionDragStart", $, te.setState), Ig("onSelectionDragStop", T, te.setState), Ig("noPanClassName", L, te.setState), Ig("nodeOrigin", j, te.setState), Ig("rfId", H, te.setState), Ig("autoPanOnConnect", Y, te.setState), Ig("autoPanOnNodeDrag", X, te.setState), Ig("onError", V, te.setState), Ig("connectionRadius", Z, te.setState), Ig("isValidConnection", F, te.setState), Og(e, K), Og(t, U), Og(y, G), Og(S, q), Og(M, Q), Og(x, J), null
+                    }), []), Ig("defaultEdgeOptions", P, te.setState), Ig("connectionMode", w, te.setState), Ig("onConnect", a, te.setState), Ig("onConnectStart", s, te.setState), Ig("onConnectEnd", i, te.setState), Ig("onClickConnectStart", l, te.setState), Ig("onClickConnectEnd", d, te.setState), Ig("nodesDraggable", c, te.setState), Ig("nodesConnectable", u, te.setState), Ig("nodesFocusable", g, te.setState), Ig("edgesFocusable", h, te.setState), Ig("edgesUpdatable", p, te.setState), Ig("elementsSelectable", E, te.setState), Ig("elevateNodesOnSelect", m, te.setState), Ig("snapToGrid", N, te.setState), Ig("snapGrid", C, te.setState), Ig("onNodesChange", b, te.setState), Ig("onEdgesChange", v, te.setState), Ig("connectOnClick", k, te.setState), Ig("fitViewOnInit", O, te.setState), Ig("fitViewOnInitOptions", I, te.setState), Ig("onNodesDelete", A, te.setState), Ig("onEdgesDelete", _, te.setState), Ig("onNodeDrag", D, te.setState), Ig("onNodeDragStart", R, te.setState), Ig("onNodeDragStop", B, te.setState), Ig("onSelectionDrag", z, te.setState), Ig("onSelectionDragStart", $, te.setState), Ig("onSelectionDragStop", T, te.setState), Ig("noPanClassName", L, te.setState), Ig("nodeOrigin", j, te.setState), Ig("rfId", H, te.setState), Ig("autoPanOnConnect", Y, te.setState), Ig("autoPanOnNodeDrag", X, te.setState), Ig("onError", V, te.setState), Ig("connectionRadius", Z, te.setState), Ig("isValidConnection", K, te.setState), Og(e, F), Og(t, U), Og(y, G), Og(S, q), Og(M, Q), Og(x, J), null
                 },
                 _g = {
                     display: "none"
                 },
                 Dg = {
                     position: "absolute",
                     width: 1,
@@ -13425,17 +13425,17 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K
                 }) => {
-                    const K = (0, r.useRef)(null),
+                    const F = (0, r.useRef)(null),
                         [U, W] = (0, r.useState)(!1),
                         [G, q] = (0, r.useState)(!1),
                         Q = nu(),
                         J = (0, r.useMemo)((() => `url(#${Wu(j,H)})`), [j, H]),
                         ee = (0, r.useMemo)((() => `url(#${Wu(L,H)})`), [L, H]);
                     if (P) return null;
                     const te = Cu(t, Q.getState, d),
@@ -13494,25 +13494,25 @@
                         onKeyDown: X ? e => {
                             if (Su.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
                                 } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                "Escape" === e.key ? (F.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : void 0,
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${Bg}-${H}` : void 0,
-                        ref: K,
+                        ref: F,
                         children: [!G && (0, o.jsx)(e, {
                             id: t,
                             source: x,
                             target: b,
                             selected: c,
                             animated: u,
                             label: g,
@@ -13530,15 +13530,15 @@
                             sourcePosition: N,
                             targetPosition: M,
                             sourceHandleId: O,
                             targetHandleId: I,
                             markerStart: J,
                             markerEnd: ee,
                             pathOptions: Z,
-                            interactionWidth: F
+                            interactionWidth: K
                         }), V && (0, o.jsxs)(o.Fragment, {
                             children: [("source" === V || !0 === V) && (0, o.jsx)(Xg, {
                                 position: N,
                                 centerX: v,
                                 centerY: E,
                                 radius: B,
                                 onMouseDown: e => se(e, !0),
@@ -13557,26 +13557,26 @@
                             })]
                         })]
                     })
                 };
                 return t.displayName = "EdgeWrapper", (0, r.memo)(t)
             };
 
-            function Fg(e) {
+            function Kg(e) {
                 return {
                     default: Zg(e.default || Zu),
                     straight: Zg(e.bezier || Hu),
                     step: Zg(e.step || ju),
                     smoothstep: Zg(e.step || Lu),
                     simplebezier: Zg(e.simplebezier || Bu),
                     ...Object.keys(e).filter((e => !["default", "bezier"].includes(e))).reduce(((t, n) => (t[n] = Zg(e[n] || Zu), t)), {})
                 }
             }
 
-            function Kg(e, t, n = null) {
+            function Fg(e, t, n = null) {
                 const o = (n?.x || 0) + t.x,
                     r = (n?.y || 0) + t.y,
                     a = n?.width || t.width,
                     s = n?.height || t.height;
                 switch (e) {
                     case _u.Top:
                         return {
@@ -14013,16 +14013,16 @@
                         L = (0, r.useRef)(null),
                         j = (0, r.useRef)(N),
                         H = (0, r.useRef)(M),
                         Y = (0, r.useRef)(n),
                         X = v || b || g || h || p || f,
                         V = sh(),
                         Z = nh(t, T.getState, h),
-                        F = nh(t, T.getState, p),
-                        K = nh(t, T.getState, f),
+                        K = nh(t, T.getState, p),
+                        F = nh(t, T.getState, f),
                         U = nh(t, T.getState, m),
                         W = nh(t, T.getState, y);
                     (0, r.useEffect)((() => {
                         if (L.current && !k) {
                             const e = L.current;
                             return P?.observe(e), () => P?.unobserve(e)
                         }
@@ -14061,16 +14061,16 @@
                             pointerEvents: X ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: Z,
-                        onMouseMove: F,
-                        onMouseLeave: K,
+                        onMouseMove: K,
+                        onMouseLeave: F,
                         onContextMenu: U,
                         onClick: e => {
                             if (!v || C && b || oh({
                                     id: t,
                                     store: T,
                                     nodeRef: L
                                 }), g) {
@@ -14099,15 +14099,15 @@
                                     isShiftPressed: e.shiftKey
                                 }))
                         } : void 0,
                         tabIndex: w ? 0 : void 0,
                         role: w ? "button" : void 0,
                         "aria-describedby": B ? void 0 : `${Rg}-${$}`,
                         "aria-label": z,
-                        children: (0, o.jsx)(Ku, {
+                        children: (0, o.jsx)(Fu, {
                             value: t,
                             children: (0, o.jsx)(e, {
                                 id: t,
                                 data: a,
                                 type: n,
                                 xPos: i,
                                 yPos: l,
@@ -15141,31 +15141,31 @@
                                 disableKeyboardA11y: $
                             })]
                         })
                     })
                 };
             Vh.displayName = "FlowRenderer";
             var Zh = (0, r.memo)(Vh);
-            const Fh = e => ({
+            const Kh = e => ({
                     nodesDraggable: e.nodesDraggable,
                     nodesConnectable: e.nodesConnectable,
                     nodesFocusable: e.nodesFocusable,
                     elementsSelectable: e.elementsSelectable,
                     updateNodeDimensions: e.updateNodeDimensions,
                     onError: e.onError
                 }),
-                Kh = e => {
+                Fh = e => {
                     const {
                         nodesDraggable: t,
                         nodesConnectable: n,
                         nodesFocusable: a,
                         elementsSelectable: s,
                         updateNodeDimensions: i,
                         onError: l
-                    } = tu(Fh, f), d = (c = e.onlyRenderVisibleElements, tu((0, r.useCallback)((e => c ? eg(e.nodeInternals, {
+                    } = tu(Kh, f), d = (c = e.onlyRenderVisibleElements, tu((0, r.useCallback)((e => c ? eg(e.nodeInternals, {
                         x: 0,
                         y: 0,
                         width: e.width,
                         height: e.height
                     }, e.transform, !0) : e.getNodes()), [c])));
                     var c;
                     const u = (0, r.useRef)(),
@@ -15254,16 +15254,16 @@
                                 rfId: e.rfId,
                                 disableKeyboardA11y: e.disableKeyboardA11y,
                                 ariaLabel: r.ariaLabel
                             }, r.id)
                         }))
                     })
                 };
-            Kh.displayName = "NodeRenderer";
-            var Uh = (0, r.memo)(Kh);
+            Fh.displayName = "NodeRenderer";
+            var Uh = (0, r.memo)(Fh);
             const Wh = [{
                 level: 0,
                 isMaxLevel: !0,
                 edges: []
             }];
             const Gh = {
                     [Au.Arrow]: ({
@@ -15494,16 +15494,16 @@
                                     if (!A || !_) return P?.("008", Jc.error008(A, e)), null;
                                     const {
                                         sourceX: $,
                                         sourceY: T,
                                         targetX: L,
                                         targetY: j
                                     } = ((e, t, n, o, r, a) => {
-                                        const s = Kg(n, e, t),
-                                            i = Kg(a, o, r);
+                                        const s = Fg(n, e, t),
+                                            i = Fg(a, o, r);
                                         return {
                                             sourceX: s.x,
                                             sourceY: s.y,
                                             targetX: i.x,
                                             targetY: i.y
                                         }
                                     })(t, A, D, f, _, R);
@@ -15725,16 +15725,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -15754,16 +15754,16 @@
             }) => (function(e) {
                 const t = Ch(),
                     n = (0, r.useRef)(!1);
                 (0, r.useEffect)((() => {
                     !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                 }), [e, t.viewportInitialized])
             }(i), (0, o.jsx)(Zh, {
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneContextMenu: q,
                 onPaneScroll: G,
                 deleteKeyCode: O,
                 selectionKeyCode: w,
                 selectionOnDrag: C,
@@ -16226,16 +16226,16 @@
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
                     selectionMode: Z = Ou.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = "Meta",
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = "Meta",
                     zoomActivationKeyCode: U = "Meta",
                     snapToGrid: W = !1,
                     snapGrid: G = xp,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -16280,29 +16280,29 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
                     style: tt,
                     id: nt,
                     ...ot
                 }, rt) => {
                     const at = fp(i, dh),
-                        st = fp(l, Fg),
+                        st = fp(l, Kg),
                         it = nt || "1";
                     return (0, o.jsx)("div", {
                         ...ot,
                         style: {
                             ...tt,
                             ...vp
                         },
@@ -16329,16 +16329,16 @@
                                 connectionLineStyle: L,
                                 connectionLineComponent: j,
                                 connectionLineContainerStyle: H,
                                 selectionKeyCode: X,
                                 selectionOnDrag: V,
                                 selectionMode: Z,
                                 deleteKeyCode: Y,
-                                multiSelectionKeyCode: K,
-                                panActivationKeyCode: F,
+                                multiSelectionKeyCode: F,
+                                panActivationKeyCode: K,
                                 zoomActivationKeyCode: U,
                                 onlyRenderVisibleElements: q,
                                 selectNodesOnDrag: Q,
                                 defaultViewport: se,
                                 translateExtent: de,
                                 minZoom: ie,
                                 maxZoom: le,
@@ -16389,26 +16389,26 @@
                                 onClickConnectEnd: x,
                                 nodesDraggable: J,
                                 nodesConnectable: ee,
                                 nodesFocusable: te,
                                 edgesFocusable: oe,
                                 edgesUpdatable: re,
                                 elementsSelectable: ae,
-                                elevateNodesOnSelect: Ke,
+                                elevateNodesOnSelect: Fe,
                                 minZoom: ie,
                                 maxZoom: le,
                                 nodeExtent: ue,
                                 onNodesChange: ze,
                                 onEdgesChange: $e,
                                 snapToGrid: W,
                                 snapGrid: G,
                                 connectionMode: $,
                                 translateExtent: de,
                                 connectOnClick: Xe,
-                                defaultEdgeOptions: Fe,
+                                defaultEdgeOptions: Ke,
                                 fitView: He,
                                 fitViewOptions: Ye,
                                 onNodesDelete: P,
                                 onEdgesDelete: O,
                                 onNodeDragStart: N,
                                 onNodeDrag: M,
                                 onNodeDragStop: k,
@@ -16723,16 +16723,16 @@
                 Zp = (e = {
                     x: 0,
                     y: 0
                 }, t) => ({
                     x: Vp(e.x, t[0][0], t[1][0]),
                     y: Vp(e.y, t[0][1], t[1][1])
                 }),
-                Fp = (e, t, n) => e < t ? Vp(Math.abs(e - t), 1, 50) / 50 : e > n ? -Vp(Math.abs(e - n), 1, 50) / 50 : 0,
-                Kp = (e, t) => [20 * Fp(e.x, 35, t.width - 35), 20 * Fp(e.y, 35, t.height - 35)],
+                Kp = (e, t, n) => e < t ? Vp(Math.abs(e - t), 1, 50) / 50 : e > n ? -Vp(Math.abs(e - n), 1, 50) / 50 : 0,
+                Fp = (e, t) => [20 * Kp(e.x, 35, t.width - 35), 20 * Kp(e.y, 35, t.height - 35)],
                 Up = e => e.getRootNode?.() || window?.document,
                 Wp = ({
                     x: e,
                     y: t,
                     width: n,
                     height: o
                 }) => ({
@@ -17506,20 +17506,20 @@
                 return e || (t?.classList.contains("target") ? "target" : t?.classList.contains("source") ? "source" : null)
             }
 
             function Zf(e) {
                 e?.classList.remove("valid", "connecting", "react-flow__handle-valid", "react-flow__handle-connecting")
             }
 
-            function Ff(e, t) {
+            function Kf(e, t) {
                 let n = null;
                 return t ? n = "valid" : e && !t && (n = "invalid"), n
             }
 
-            function Kf({
+            function Ff({
                 event: e,
                 handleId: t,
                 nodeId: n,
                 onConnect: o,
                 isTarget: r,
                 getState: a,
                 setState: s,
@@ -17570,15 +17570,15 @@
                         nodes: y(),
                         nodeId: n,
                         handleId: t,
                         handleType: C
                     }),
                     D = () => {
                         if (!h) return;
-                        const [e, t] = Kp(k, N);
+                        const [e, t] = Fp(k, N);
                         m({
                             x: e,
                             y: t
                         }), b = requestAnimationFrame(D)
                     };
 
                 function R(e) {
@@ -17595,15 +17595,15 @@
                     }(Df(k, o, !1, [1, 1]), p, _), P || (D(), P = !0);
                     const l = Xf(e, x, u, n, t, r ? "target" : "source", i, c);
                     if (A = l.handleDomNode, O = l.connection, I = l.isValid, s({
                             connectionPosition: x && I ? Rf({
                                 x: x.x,
                                 y: x.y
                             }, o) : k,
-                            connectionStatus: Ff(!!x, I),
+                            connectionStatus: Kf(!!x, I),
                             connectionEndHandle: l.endHandle
                         }), !x && !I && !A) return Zf(M);
                     O.source !== O.target && A && (Zf(M), M = A, A.classList.add("connecting", "react-flow__handle-connecting"), A.classList.toggle("valid", I), A.classList.toggle("react-flow__handle-valid", I))
                 }
 
                 function B(e) {
                     (x || A) && O && I && o?.(O), a().onConnectEnd?.(e), l && d?.(e), Zf(M), S(), cancelAnimationFrame(b), P = !1, I = !1, O = null, A = null, c.removeEventListener("mousemove", R), c.removeEventListener("mouseup", B), c.removeEventListener("touchmove", R), c.removeEventListener("touchend", B)
@@ -17697,15 +17697,15 @@
                                 })(r, e))
                             }
                             n?.(r), c?.(r)
                         },
                         k = e => {
                             if (!v) return;
                             const t = of(e);
-                            i && (t && 0 === e.button || !t) && Kf({
+                            i && (t && 0 === e.button || !t) && Ff({
                                 event: e,
                                 handleId: S,
                                 nodeId: v,
                                 onConnect: M,
                                 isTarget: x,
                                 getState: b.getState,
                                 setState: b.setState,
@@ -17916,18 +17916,18 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F
+                    isValidConnection: K
                 }) => {
                     const {
-                        setNodes: K,
+                        setNodes: F,
                         setEdges: U,
                         setDefaultNodesAndEdges: W,
                         setMinZoom: G,
                         setMaxZoom: q,
                         setTranslateExtent: Q,
                         setNodeExtent: J,
                         reset: ee
@@ -17936,15 +17936,15 @@
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return W(n, e), () => {
                             ee()
                         }
-                    }), []), hm("defaultEdgeOptions", P, te.setState), hm("connectionMode", w, te.setState), hm("onConnect", a, te.setState), hm("onConnectStart", s, te.setState), hm("onConnectEnd", i, te.setState), hm("onClickConnectStart", l, te.setState), hm("onClickConnectEnd", d, te.setState), hm("nodesDraggable", c, te.setState), hm("nodesConnectable", u, te.setState), hm("nodesFocusable", g, te.setState), hm("edgesFocusable", h, te.setState), hm("edgesUpdatable", p, te.setState), hm("elementsSelectable", E, te.setState), hm("elevateNodesOnSelect", m, te.setState), hm("snapToGrid", N, te.setState), hm("snapGrid", C, te.setState), hm("onNodesChange", b, te.setState), hm("onEdgesChange", v, te.setState), hm("connectOnClick", k, te.setState), hm("fitViewOnInit", O, te.setState), hm("fitViewOnInitOptions", I, te.setState), hm("onNodesDelete", A, te.setState), hm("onEdgesDelete", _, te.setState), hm("onNodeDrag", D, te.setState), hm("onNodeDragStart", R, te.setState), hm("onNodeDragStop", B, te.setState), hm("onSelectionDrag", z, te.setState), hm("onSelectionDragStart", $, te.setState), hm("onSelectionDragStop", T, te.setState), hm("noPanClassName", L, te.setState), hm("nodeOrigin", j, te.setState), hm("rfId", H, te.setState), hm("autoPanOnConnect", Y, te.setState), hm("autoPanOnNodeDrag", X, te.setState), hm("onError", V, te.setState), hm("connectionRadius", Z, te.setState), hm("isValidConnection", F, te.setState), gm(e, K), gm(t, U), gm(y, G), gm(S, q), gm(M, Q), gm(x, J), null
+                    }), []), hm("defaultEdgeOptions", P, te.setState), hm("connectionMode", w, te.setState), hm("onConnect", a, te.setState), hm("onConnectStart", s, te.setState), hm("onConnectEnd", i, te.setState), hm("onClickConnectStart", l, te.setState), hm("onClickConnectEnd", d, te.setState), hm("nodesDraggable", c, te.setState), hm("nodesConnectable", u, te.setState), hm("nodesFocusable", g, te.setState), hm("edgesFocusable", h, te.setState), hm("edgesUpdatable", p, te.setState), hm("elementsSelectable", E, te.setState), hm("elevateNodesOnSelect", m, te.setState), hm("snapToGrid", N, te.setState), hm("snapGrid", C, te.setState), hm("onNodesChange", b, te.setState), hm("onEdgesChange", v, te.setState), hm("connectOnClick", k, te.setState), hm("fitViewOnInit", O, te.setState), hm("fitViewOnInitOptions", I, te.setState), hm("onNodesDelete", A, te.setState), hm("onEdgesDelete", _, te.setState), hm("onNodeDrag", D, te.setState), hm("onNodeDragStart", R, te.setState), hm("onNodeDragStop", B, te.setState), hm("onSelectionDrag", z, te.setState), hm("onSelectionDragStart", $, te.setState), hm("onSelectionDragStop", T, te.setState), hm("noPanClassName", L, te.setState), hm("nodeOrigin", j, te.setState), hm("rfId", H, te.setState), hm("autoPanOnConnect", Y, te.setState), hm("autoPanOnNodeDrag", X, te.setState), hm("onError", V, te.setState), hm("connectionRadius", Z, te.setState), hm("isValidConnection", K, te.setState), gm(e, F), gm(t, U), gm(y, G), gm(S, q), gm(M, Q), gm(x, J), null
                 },
                 fm = {
                     display: "none"
                 },
                 mm = {
                     position: "absolute",
                     width: 1,
@@ -18056,17 +18056,17 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K
                 }) => {
-                    const K = (0, r.useRef)(null),
+                    const F = (0, r.useRef)(null),
                         [U, W] = (0, r.useState)(!1),
                         [G, q] = (0, r.useState)(!1),
                         Q = Tp(),
                         J = (0, r.useMemo)((() => `url(#${_f(j,H)})`), [j, H]),
                         ee = (0, r.useMemo)((() => `url(#${_f(L,H)})`), [L, H]);
                     if (P) return null;
                     const te = sf(t, Q.getState, d),
@@ -18076,15 +18076,15 @@
                         ae = sf(t, Q.getState, R),
                         se = (e, n) => {
                             if (0 !== e.button) return;
                             const {
                                 edges: o,
                                 isValidConnection: r
                             } = Q.getState(), a = n ? b : x, s = (n ? I : O) || null, i = n ? "target" : "source", l = r || km, d = n, c = o.find((e => e.id === t));
-                            q(!0), $?.(e, c, i), Kf({
+                            q(!0), $?.(e, c, i), Ff({
                                 event: e,
                                 handleId: s,
                                 nodeId: a,
                                 onConnect: e => z?.(c, e),
                                 isTarget: d,
                                 getState: Q.getState,
                                 setState: Q.setState,
@@ -18125,25 +18125,25 @@
                         onKeyDown: X ? e => {
                             if (ef.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
                                 } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                "Escape" === e.key ? (F.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : void 0,
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${Sm}-${H}` : void 0,
-                        ref: K,
+                        ref: F,
                         children: [!G && (0, o.jsx)(e, {
                             id: t,
                             source: x,
                             target: b,
                             selected: c,
                             animated: u,
                             label: g,
@@ -18161,15 +18161,15 @@
                             sourcePosition: N,
                             targetPosition: M,
                             sourceHandleId: O,
                             targetHandleId: I,
                             markerStart: J,
                             markerEnd: ee,
                             pathOptions: Z,
-                            interactionWidth: F
+                            interactionWidth: K
                         }), V && (0, o.jsxs)(o.Fragment, {
                             children: [("source" === V || !0 === V) && (0, o.jsx)(Mm, {
                                 position: N,
                                 centerX: v,
                                 centerY: E,
                                 radius: B,
                                 onMouseDown: e => se(e, !0),
@@ -18476,15 +18476,15 @@
                                         nodeInternals: n
                                     });
                                     S(m.current, e, t)
                                 }
                             },
                             x = () => {
                                 if (!p.current) return;
-                                const [e, t] = Kp(f.current, p.current);
+                                const [e, t] = Fp(f.current, p.current);
                                 if (0 !== e || 0 !== t) {
                                     const {
                                         transform: n,
                                         panBy: o
                                     } = l.getState();
                                     g.current.x = (g.current.x ?? 0) - e / n[2], g.current.y = (g.current.y ?? 0) - t / n[2], o({
                                         x: e,
@@ -18644,16 +18644,16 @@
                         L = (0, r.useRef)(null),
                         j = (0, r.useRef)(N),
                         H = (0, r.useRef)(M),
                         Y = (0, r.useRef)(n),
                         X = v || b || g || h || p || f,
                         V = Xm(),
                         Z = Lm(t, T.getState, h),
-                        F = Lm(t, T.getState, p),
-                        K = Lm(t, T.getState, f),
+                        K = Lm(t, T.getState, p),
+                        F = Lm(t, T.getState, f),
                         U = Lm(t, T.getState, m),
                         W = Lm(t, T.getState, y);
                     (0, r.useEffect)((() => {
                         if (L.current && !k) {
                             const e = L.current;
                             return P?.observe(e), () => P?.unobserve(e)
                         }
@@ -18692,16 +18692,16 @@
                             pointerEvents: X ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: Z,
-                        onMouseMove: F,
-                        onMouseLeave: K,
+                        onMouseMove: K,
+                        onMouseLeave: F,
                         onContextMenu: U,
                         onClick: e => {
                             if (!v || C && b || jm({
                                     id: t,
                                     store: T,
                                     nodeRef: L
                                 }), g) {
@@ -18752,26 +18752,26 @@
                             })
                         })
                     })
                 };
                 return t.displayName = "NodeWrapper", (0, r.memo)(t)
             };
 
-            function Fm(e) {
+            function Km(e) {
                 return {
                     input: Zm(e.input || tm),
                     default: Zm(e.default || Jf),
                     output: Zm(e.output || om),
                     group: Zm(e.group || rm),
                     ...Object.keys(e).filter((e => !["input", "default", "output", "group"].includes(e))).reduce(((t, n) => (t[n] = Zm(e[n] || Jf), t)), {})
                 }
             }
-            const Km = "undefined" != typeof document ? document : null;
+            const Fm = "undefined" != typeof document ? document : null;
             var Um = (e = null, t = {
-                target: Km
+                target: Fm
             }) => {
                 const [n, o] = (0, r.useState)(!1), a = (0, r.useRef)(!1), s = (0, r.useRef)(new Set([])), [i, l] = (0, r.useMemo)((() => {
                     if (null !== e) {
                         const t = (Array.isArray(e) ? e : [e]).filter((e => "string" == typeof e)).map((e => e.split("+"))),
                             n = t.reduce(((e, t) => e.concat(...t)), []);
                         return [t, n]
                     }
@@ -20311,15 +20311,15 @@
                             type: n,
                             CustomComponent: r,
                             connectionStatus: u
                         })
                     })
                 }) : null
             }
-            const Fy = ({
+            const Ky = ({
                 nodeTypes: e,
                 edgeTypes: t,
                 onMove: n,
                 onMoveStart: a,
                 onMoveEnd: s,
                 onInit: i,
                 onNodeClick: l,
@@ -20356,16 +20356,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -20385,16 +20385,16 @@
             }) => (function(e) {
                 const t = iy(),
                     n = (0, r.useRef)(!1);
                 (0, r.useEffect)((() => {
                     !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                 }), [e, t.viewportInitialized])
             }(i), (0, o.jsx)(Py, {
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneContextMenu: q,
                 onPaneScroll: G,
                 deleteKeyCode: O,
                 selectionKeyCode: w,
                 selectionOnDrag: C,
@@ -20467,16 +20467,16 @@
                         disableKeyboardA11y: ce,
                         nodeOrigin: ue,
                         nodeExtent: ge,
                         rfId: he
                     })]
                 })
             }));
-            Fy.displayName = "GraphView";
-            var Ky = (0, r.memo)(Fy);
+            Ky.displayName = "GraphView";
+            var Fy = (0, r.memo)(Ky);
             const Uy = [
                     [Number.NEGATIVE_INFINITY, Number.NEGATIVE_INFINITY],
                     [Number.POSITIVE_INFINITY, Number.POSITIVE_INFINITY]
                 ],
                 Wy = {
                     rfId: "1",
                     width: 0,
@@ -20857,16 +20857,16 @@
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
                     selectionMode: Z = gf.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = "Meta",
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = "Meta",
                     zoomActivationKeyCode: U = "Meta",
                     snapToGrid: W = !1,
                     snapGrid: G = nS,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -20911,42 +20911,42 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
                     style: tt,
                     id: nt,
                     ...ot
                 }, rt) => {
-                    const at = Qy(i, Fm),
+                    const at = Qy(i, Km),
                         st = Qy(l, Om),
                         it = nt || "1";
                     return (0, o.jsx)("div", {
                         ...ot,
                         style: {
                             ...tt,
                             ...rS
                         },
                         ref: rt,
                         className: s(["react-flow", a]),
                         "data-testid": "rf__wrapper",
                         id: nt,
                         children: (0, o.jsxs)(qy, {
-                            children: [(0, o.jsx)(Ky, {
+                            children: [(0, o.jsx)(Fy, {
                                 onInit: u,
                                 onMove: g,
                                 onMoveStart: h,
                                 onMoveEnd: p,
                                 onNodeClick: d,
                                 onEdgeClick: c,
                                 onNodeMouseEnter: b,
@@ -20960,16 +20960,16 @@
                                 connectionLineStyle: L,
                                 connectionLineComponent: j,
                                 connectionLineContainerStyle: H,
                                 selectionKeyCode: X,
                                 selectionOnDrag: V,
                                 selectionMode: Z,
                                 deleteKeyCode: Y,
-                                multiSelectionKeyCode: K,
-                                panActivationKeyCode: F,
+                                multiSelectionKeyCode: F,
+                                panActivationKeyCode: K,
                                 zoomActivationKeyCode: U,
                                 onlyRenderVisibleElements: q,
                                 selectNodesOnDrag: Q,
                                 defaultViewport: se,
                                 translateExtent: de,
                                 minZoom: ie,
                                 maxZoom: le,
@@ -21020,26 +21020,26 @@
                                 onClickConnectEnd: x,
                                 nodesDraggable: J,
                                 nodesConnectable: ee,
                                 nodesFocusable: te,
                                 edgesFocusable: oe,
                                 edgesUpdatable: re,
                                 elementsSelectable: ae,
-                                elevateNodesOnSelect: Ke,
+                                elevateNodesOnSelect: Fe,
                                 minZoom: ie,
                                 maxZoom: le,
                                 nodeExtent: ue,
                                 onNodesChange: ze,
                                 onEdgesChange: $e,
                                 snapToGrid: W,
                                 snapGrid: G,
                                 connectionMode: $,
                                 translateExtent: de,
                                 connectOnClick: Xe,
-                                defaultEdgeOptions: Fe,
+                                defaultEdgeOptions: Ke,
                                 fitView: He,
                                 fitViewOptions: Ye,
                                 onNodesDelete: P,
                                 onEdgesDelete: O,
                                 onNodeDragStart: N,
                                 onNodeDrag: M,
                                 onNodeDragStop: k,
@@ -21441,15 +21441,15 @@
                 targetControlX: s,
                 targetControlY: i
             }) {
                 const l = .125 * e + .375 * r + .375 * s + .125 * n,
                     d = .125 * t + .375 * a + .375 * i + .125 * o;
                 return [l, d, Math.abs(l - e), Math.abs(d - t)]
             }
-            var ZS, FS, KS, US, WS, GS;
+            var ZS, KS, FS, US, WS, GS;
 
             function qS({
                 pos: e,
                 x1: t,
                 y1: n,
                 x2: o,
                 y2: r
@@ -21491,18 +21491,18 @@
             }
             HS.displayName = "BaseEdge",
                 function(e) {
                     e.Strict = "strict", e.Loose = "loose"
                 }(ZS || (ZS = {})),
                 function(e) {
                     e.Free = "free", e.Vertical = "vertical", e.Horizontal = "horizontal"
-                }(FS || (FS = {})),
+                }(KS || (KS = {})),
                 function(e) {
                     e.Partial = "partial", e.Full = "full"
-                }(KS || (KS = {})),
+                }(FS || (FS = {})),
                 function(e) {
                     e.Bezier = "default", e.Straight = "straight", e.Step = "step", e.SmoothStep = "smoothstep", e.SimpleBezier = "simplebezier"
                 }(US || (US = {})),
                 function(e) {
                     e.Arrow = "arrow", e.ArrowClosed = "arrowclosed"
                 }(WS || (WS = {})),
                 function(e) {
@@ -22436,23 +22436,23 @@
                     };
                     e?.(r), t.getState().onSelectionChange?.(r)
                 }), [n, o, e]), null
             }));
             Vx.displayName = "SelectionListener";
             const Zx = e => !!e.onSelectionChange;
 
-            function Fx({
+            function Kx({
                 onSelectionChange: e
             }) {
                 const t = xS(Zx);
                 return e || t ? (0, o.jsx)(Vx, {
                     onSelectionChange: e
                 }) : null
             }
-            const Kx = e => ({
+            const Fx = e => ({
                 setNodes: e.setNodes,
                 setEdges: e.setEdges,
                 setDefaultNodesAndEdges: e.setDefaultNodesAndEdges,
                 setMinZoom: e.setMinZoom,
                 setMaxZoom: e.setMaxZoom,
                 setTranslateExtent: e.setTranslateExtent,
                 setNodeExtent: e.setNodeExtent,
@@ -22513,35 +22513,35 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F
+                    isValidConnection: K
                 }) => {
                     const {
-                        setNodes: K,
+                        setNodes: F,
                         setEdges: U,
                         setDefaultNodesAndEdges: W,
                         setMinZoom: G,
                         setMaxZoom: q,
                         setTranslateExtent: Q,
                         setNodeExtent: J,
                         reset: ee
-                    } = xS(Kx, f), te = bS();
+                    } = xS(Fx, f), te = bS();
                     return (0, r.useEffect)((() => {
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return W(n, e), () => {
                             ee()
                         }
-                    }), []), Wx("defaultEdgeOptions", P, te.setState), Wx("connectionMode", w, te.setState), Wx("onConnect", a, te.setState), Wx("onConnectStart", s, te.setState), Wx("onConnectEnd", i, te.setState), Wx("onClickConnectStart", l, te.setState), Wx("onClickConnectEnd", d, te.setState), Wx("nodesDraggable", c, te.setState), Wx("nodesConnectable", u, te.setState), Wx("nodesFocusable", g, te.setState), Wx("edgesFocusable", h, te.setState), Wx("edgesUpdatable", p, te.setState), Wx("elementsSelectable", E, te.setState), Wx("elevateNodesOnSelect", m, te.setState), Wx("snapToGrid", N, te.setState), Wx("snapGrid", C, te.setState), Wx("onNodesChange", b, te.setState), Wx("onEdgesChange", v, te.setState), Wx("connectOnClick", k, te.setState), Wx("fitViewOnInit", O, te.setState), Wx("fitViewOnInitOptions", I, te.setState), Wx("onNodesDelete", A, te.setState), Wx("onEdgesDelete", _, te.setState), Wx("onNodeDrag", D, te.setState), Wx("onNodeDragStart", R, te.setState), Wx("onNodeDragStop", B, te.setState), Wx("onSelectionDrag", z, te.setState), Wx("onSelectionDragStart", $, te.setState), Wx("onSelectionDragStop", T, te.setState), Wx("noPanClassName", L, te.setState), Wx("nodeOrigin", j, te.setState), Wx("rfId", H, te.setState), Wx("autoPanOnConnect", Y, te.setState), Wx("autoPanOnNodeDrag", X, te.setState), Wx("onError", V, te.setState), Wx("connectionRadius", Z, te.setState), Wx("isValidConnection", F, te.setState), Ux(e, K), Ux(t, U), Ux(y, G), Ux(S, q), Ux(M, Q), Ux(x, J), null
+                    }), []), Wx("defaultEdgeOptions", P, te.setState), Wx("connectionMode", w, te.setState), Wx("onConnect", a, te.setState), Wx("onConnectStart", s, te.setState), Wx("onConnectEnd", i, te.setState), Wx("onClickConnectStart", l, te.setState), Wx("onClickConnectEnd", d, te.setState), Wx("nodesDraggable", c, te.setState), Wx("nodesConnectable", u, te.setState), Wx("nodesFocusable", g, te.setState), Wx("edgesFocusable", h, te.setState), Wx("edgesUpdatable", p, te.setState), Wx("elementsSelectable", E, te.setState), Wx("elevateNodesOnSelect", m, te.setState), Wx("snapToGrid", N, te.setState), Wx("snapGrid", C, te.setState), Wx("onNodesChange", b, te.setState), Wx("onEdgesChange", v, te.setState), Wx("connectOnClick", k, te.setState), Wx("fitViewOnInit", O, te.setState), Wx("fitViewOnInitOptions", I, te.setState), Wx("onNodesDelete", A, te.setState), Wx("onEdgesDelete", _, te.setState), Wx("onNodeDrag", D, te.setState), Wx("onNodeDragStart", R, te.setState), Wx("onNodeDragStop", B, te.setState), Wx("onSelectionDrag", z, te.setState), Wx("onSelectionDragStart", $, te.setState), Wx("onSelectionDragStop", T, te.setState), Wx("noPanClassName", L, te.setState), Wx("nodeOrigin", j, te.setState), Wx("rfId", H, te.setState), Wx("autoPanOnConnect", Y, te.setState), Wx("autoPanOnNodeDrag", X, te.setState), Wx("onError", V, te.setState), Wx("connectionRadius", Z, te.setState), Wx("isValidConnection", K, te.setState), Ux(e, F), Ux(t, U), Ux(y, G), Ux(S, q), Ux(M, Q), Ux(x, J), null
                 },
                 qx = {
                     display: "none"
                 },
                 Qx = {
                     position: "absolute",
                     width: 1,
@@ -22653,17 +22653,17 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K
                 }) => {
-                    const K = (0, r.useRef)(null),
+                    const F = (0, r.useRef)(null),
                         [U, W] = (0, r.useState)(!1),
                         [G, q] = (0, r.useState)(!1),
                         Q = bS(),
                         J = (0, r.useMemo)((() => `url(#${px(j,H)})`), [j, H]),
                         ee = (0, r.useMemo)((() => `url(#${px(L,H)})`), [L, H]);
                     if (P) return null;
                     const te = YS(t, Q.getState, d),
@@ -22722,25 +22722,25 @@
                         onKeyDown: X ? e => {
                             if (zS.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
                                 } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                "Escape" === e.key ? (F.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : void 0,
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${eb}-${H}` : void 0,
-                        ref: K,
+                        ref: F,
                         children: [!G && (0, o.jsx)(e, {
                             id: t,
                             source: x,
                             target: b,
                             selected: c,
                             animated: u,
                             label: g,
@@ -22758,15 +22758,15 @@
                             sourcePosition: N,
                             targetPosition: M,
                             sourceHandleId: O,
                             targetHandleId: I,
                             markerStart: J,
                             markerEnd: ee,
                             pathOptions: Z,
-                            interactionWidth: F
+                            interactionWidth: K
                         }), V && (0, o.jsxs)(o.Fragment, {
                             children: [("source" === V || !0 === V) && (0, o.jsx)(lb, {
                                 position: N,
                                 centerX: v,
                                 centerY: E,
                                 radius: B,
                                 onMouseDown: e => se(e, !0),
@@ -23241,16 +23241,16 @@
                         L = (0, r.useRef)(null),
                         j = (0, r.useRef)(N),
                         H = (0, r.useRef)(M),
                         Y = (0, r.useRef)(n),
                         X = v || b || g || h || p || f,
                         V = Nb(),
                         Z = vb(t, T.getState, h),
-                        F = vb(t, T.getState, p),
-                        K = vb(t, T.getState, f),
+                        K = vb(t, T.getState, p),
+                        F = vb(t, T.getState, f),
                         U = vb(t, T.getState, m),
                         W = vb(t, T.getState, y);
                     (0, r.useEffect)((() => {
                         if (L.current && !k) {
                             const e = L.current;
                             return P?.observe(e), () => P?.unobserve(e)
                         }
@@ -23289,16 +23289,16 @@
                             pointerEvents: X ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: Z,
-                        onMouseMove: F,
-                        onMouseLeave: K,
+                        onMouseMove: K,
+                        onMouseLeave: F,
                         onContextMenu: U,
                         onClick: e => {
                             if (!v || C && b || Eb({
                                     id: t,
                                     store: T,
                                     nodeRef: L
                                 }), g) {
@@ -23791,16 +23791,16 @@
                     left: 0
                 },
                 Zb = e => ({
                     x: e.x,
                     y: e.y,
                     zoom: e.k
                 }),
-                Fb = (e, t) => e.target.closest(`.${t}`),
-                Kb = (e, t) => 2 === t && Array.isArray(e) && e.includes(2),
+                Kb = (e, t) => e.target.closest(`.${t}`),
+                Fb = (e, t) => 2 === t && Array.isArray(e) && e.includes(2),
                 Ub = e => ({
                     d3Zoom: e.d3Zoom,
                     d3Selection: e.d3Selection,
                     d3ZoomHandler: e.d3ZoomHandler,
                     userSelectionActive: e.userSelectionActive
                 }),
                 Wb = ({
@@ -23808,15 +23808,15 @@
                     onMoveStart: t,
                     onMoveEnd: n,
                     onPaneContextMenu: a,
                     zoomOnScroll: s = !0,
                     zoomOnPinch: i = !0,
                     panOnScroll: l = !1,
                     panOnScrollSpeed: d = .5,
-                    panOnScrollMode: c = FS.Free,
+                    panOnScrollMode: c = KS.Free,
                     zoomOnDoubleClick: u = !0,
                     elementsSelectable: g,
                     panOnDrag: h = !0,
                     defaultViewport: p,
                     translateExtent: m,
                     minZoom: y,
                     maxZoom: S,
@@ -23877,31 +23877,31 @@
                                 d3ZoomHandler: n.on("wheel.zoom"),
                                 transform: [a.x, a.y, a.k],
                                 domNode: P.current.closest(".react-flow")
                             })
                         }
                     }), []), (0, r.useEffect)((() => {
                         A && I && (!l || R || D ? void 0 !== _ && A.on("wheel.zoom", (function(e, t) {
-                            if (!b || Fb(e, E)) return null;
+                            if (!b || Kb(e, E)) return null;
                             e.preventDefault(), _.call(this, e, t)
                         }), {
                             passive: !1
                         }) : A.on("wheel.zoom", (e => {
-                            if (Fb(e, E)) return !1;
+                            if (Kb(e, E)) return !1;
                             e.preventDefault(), e.stopImmediatePropagation();
                             const t = A.property("__zoom").k || 1;
                             if (e.ctrlKey && i) {
                                 const n = Be(e),
                                     o = -e.deltaY * (1 === e.deltaMode ? .05 : e.deltaMode ? 1 : .002) * 10,
                                     r = t * Math.pow(2, o);
                                 return void I.scaleTo(A, r, n)
                             }
                             const n = 1 === e.deltaMode ? 20 : 1,
-                                o = c === FS.Vertical ? 0 : e.deltaX * n,
-                                r = c === FS.Horizontal ? 0 : e.deltaY * n;
+                                o = c === KS.Vertical ? 0 : e.deltaX * n,
+                                r = c === KS.Horizontal ? 0 : e.deltaY * n;
                             I.translateBy(A, -o / t * d, -r / t * d)
                         }), {
                             passive: !1
                         }))
                     }), [D, l, c, A, I, _, R, i, b, E]), (0, r.useEffect)((() => {
                         I && I.on("start", (e => {
                             if (!e.sourceEvent) return null;
@@ -23919,45 +23919,45 @@
                     }), [I, t]), (0, r.useEffect)((() => {
                         I && (D && !M.current ? I.on("zoom", null) : D || I.on("zoom", (t => {
                             const {
                                 onViewportChange: n
                             } = N.getState();
                             if (N.setState({
                                     transform: [t.transform.x, t.transform.y, t.transform.k]
-                                }), k.current = !(!a || !Kb(h, B.current ?? 0)), e || n) {
+                                }), k.current = !(!a || !Fb(h, B.current ?? 0)), e || n) {
                                 const o = Zb(t.transform);
                                 n?.(o), e?.(t.sourceEvent, o)
                             }
                         })))
                     }), [D, I, e, h, a]), (0, r.useEffect)((() => {
                         I && I.on("end", (e => {
                             if (!e.sourceEvent) return null;
                             const {
                                 onViewportChangeEnd: t
                             } = N.getState();
                             if (M.current = !1, N.setState({
                                     paneDragging: !1
-                                }), a && Kb(h, B.current ?? 0) && !k.current && a(e.sourceEvent), k.current = !1, (n || t) && (o = O.current, r = e.transform, o.x !== r.x || o.y !== r.y || o.zoom !== r.k)) {
+                                }), a && Fb(h, B.current ?? 0) && !k.current && a(e.sourceEvent), k.current = !1, (n || t) && (o = O.current, r = e.transform, o.x !== r.x || o.y !== r.y || o.zoom !== r.k)) {
                                 const o = Zb(e.transform);
                                 O.current = o, clearTimeout(C.current), C.current = setTimeout((() => {
                                     t?.(o), n?.(e.sourceEvent, o)
                                 }), l ? 150 : 0)
                             }
                             var o, r
                         }))
                     }), [I, l, h, n, a]), (0, r.useEffect)((() => {
                         I && I.filter((e => {
                             const t = R || s,
                                 n = i && e.ctrlKey;
-                            if (1 === e.button && "mousedown" === e.type && (Fb(e, "react-flow__node") || Fb(e, "react-flow__edge"))) return !0;
+                            if (1 === e.button && "mousedown" === e.type && (Kb(e, "react-flow__node") || Kb(e, "react-flow__edge"))) return !0;
                             if (!(h || t || l || u || i)) return !1;
                             if (D) return !1;
                             if (!u && "dblclick" === e.type) return !1;
-                            if (Fb(e, E) && "wheel" === e.type) return !1;
-                            if (Fb(e, w) && "wheel" !== e.type) return !1;
+                            if (Kb(e, E) && "wheel" === e.type) return !1;
+                            if (Kb(e, w) && "wheel" !== e.type) return !1;
                             if (!i && e.ctrlKey && "wheel" === e.type) return !1;
                             if (!t && !l && !n && "wheel" === e.type) return !1;
                             if (!h && ("mousedown" === e.type || "touchstart" === e.type)) return !1;
                             if (Array.isArray(h) && !h.includes(e.button) && ("mousedown" === e.type || "touchstart" === e.type)) return !1;
                             const o = Array.isArray(h) && h.includes(e.button) || !e.button || e.button <= 1;
                             return (!e.ctrlKey || "wheel" === e.type) && o
                         }))
@@ -24060,15 +24060,15 @@
                 rv = e => ({
                     userSelectionActive: e.userSelectionActive,
                     elementsSelectable: e.elementsSelectable,
                     dragging: e.paneDragging
                 }),
                 av = (0, r.memo)((({
                     isSelecting: e,
-                    selectionMode: t = KS.Full,
+                    selectionMode: t = FS.Full,
                     panOnDrag: n,
                     onSelectionStart: a,
                     onSelectionEnd: i,
                     onPaneClick: l,
                     onPaneContextMenu: d,
                     onPaneScroll: c,
                     onPaneMouseEnter: u,
@@ -24154,15 +24154,15 @@
                                     ...o,
                                     x: u.x < g ? u.x : g,
                                     y: u.y < h ? u.y : h,
                                     width: Math.abs(u.x - g),
                                     height: Math.abs(u.y - h)
                                 },
                                 f = c(),
-                                m = xx(r, p, s, t === KS.Partial, !0, d),
+                                m = xx(r, p, s, t === FS.Partial, !0, d),
                                 v = bx(m, a).map((e => e.id)),
                                 E = m.map((e => e.id));
                             if (S.current !== E.length) {
                                 S.current = E.length;
                                 const e = nv(f, E);
                                 e.length && i?.(e)
                             }
@@ -24953,16 +24953,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -24982,16 +24982,16 @@
             }) => (function(e) {
                 const t = Xb(),
                     n = (0, r.useRef)(!1);
                 (0, r.useEffect)((() => {
                     !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                 }), [e, t.viewportInitialized])
             }(i), (0, o.jsx)(cv, {
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneContextMenu: q,
                 onPaneScroll: G,
                 deleteKeyCode: O,
                 selectionKeyCode: w,
                 selectionOnDrag: C,
@@ -25453,17 +25453,17 @@
                     connectionLineType: T = US.Bezier,
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
-                    selectionMode: Z = KS.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = "Meta",
+                    selectionMode: Z = FS.Full,
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = "Meta",
                     zoomActivationKeyCode: U = "Meta",
                     snapToGrid: W = !1,
                     snapGrid: G = Tv,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -25479,15 +25479,15 @@
                     preventScrolling: ce = !0,
                     nodeExtent: ue,
                     defaultMarkerColor: ge = "#b1b1b7",
                     zoomOnScroll: he = !0,
                     zoomOnPinch: pe = !0,
                     panOnScroll: fe = !1,
                     panOnScrollSpeed: me = .5,
-                    panOnScrollMode: ye = FS.Free,
+                    panOnScrollMode: ye = KS.Free,
                     zoomOnDoubleClick: Se = !0,
                     panOnDrag: xe = !0,
                     onPaneClick: be,
                     onPaneMouseEnter: ve,
                     onPaneMouseMove: Ee,
                     onPaneMouseLeave: we,
                     onPaneScroll: Ce,
@@ -25508,16 +25508,16 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
@@ -25557,16 +25557,16 @@
                                 connectionLineStyle: L,
                                 connectionLineComponent: j,
                                 connectionLineContainerStyle: H,
                                 selectionKeyCode: X,
                                 selectionOnDrag: V,
                                 selectionMode: Z,
                                 deleteKeyCode: Y,
-                                multiSelectionKeyCode: K,
-                                panActivationKeyCode: F,
+                                multiSelectionKeyCode: F,
+                                panActivationKeyCode: K,
                                 zoomActivationKeyCode: U,
                                 onlyRenderVisibleElements: q,
                                 selectNodesOnDrag: Q,
                                 defaultViewport: se,
                                 translateExtent: de,
                                 minZoom: ie,
                                 maxZoom: le,
@@ -25617,26 +25617,26 @@
                                 onClickConnectEnd: x,
                                 nodesDraggable: J,
                                 nodesConnectable: ee,
                                 nodesFocusable: te,
                                 edgesFocusable: oe,
                                 edgesUpdatable: re,
                                 elementsSelectable: ae,
-                                elevateNodesOnSelect: Ke,
+                                elevateNodesOnSelect: Fe,
                                 minZoom: ie,
                                 maxZoom: le,
                                 nodeExtent: ue,
                                 onNodesChange: ze,
                                 onEdgesChange: $e,
                                 snapToGrid: W,
                                 snapGrid: G,
                                 connectionMode: $,
                                 translateExtent: de,
                                 connectOnClick: Xe,
-                                defaultEdgeOptions: Fe,
+                                defaultEdgeOptions: Ke,
                                 fitView: He,
                                 fitViewOptions: Ye,
                                 onNodesDelete: P,
                                 onEdgesDelete: O,
                                 onNodeDragStart: N,
                                 onNodeDrag: M,
                                 onNodeDragStop: k,
@@ -25647,15 +25647,15 @@
                                 nodeOrigin: ne,
                                 rfId: it,
                                 autoPanOnConnect: Ge,
                                 autoPanOnNodeDrag: qe,
                                 onError: et,
                                 connectionRadius: Qe,
                                 isValidConnection: Je
-                            }), (0, o.jsx)(Fx, {
+                            }), (0, o.jsx)(Kx, {
                                 onSelectionChange: I
                             }), Me, (0, o.jsx)(wS, {
                                 proOptions: Ze,
                                 position: Ve
                             }), (0, o.jsx)(rb, {
                                 rfId: it,
                                 disableKeyboardA11y: We
@@ -25678,21 +25678,21 @@
             function Vv({
                 children: e
             }) {
                 const t = xS(Xv);
                 return t ? (0, lo.createPortal)(e, t) : null
             }
             const Zv = (e, t) => e.length === t.length && e.every(((e, n) => ((e, t) => e?.positionAbsolute?.x === t?.positionAbsolute?.x && e?.positionAbsolute?.y === t?.positionAbsolute?.y && e?.width === t?.width && e?.height === t?.height && e?.selected === t?.selected && e?.[BS]?.z === t?.[BS]?.z)(e, t[n]))),
-                Fv = e => ({
+                Kv = e => ({
                     transform: e.transform,
                     nodeOrigin: e.nodeOrigin,
                     selectedNodesCount: e.getNodes().filter((e => e.selected)).length
                 });
 
-            function Kv(e, t, n, o, r) {
+            function Fv(e, t, n, o, r) {
                 let a = .5;
                 "start" === r ? a = 0 : "end" === r && (a = 1);
                 let s = [(e.x + e.width * a) * t[2] + t[0], e.y * t[2] + t[1] - o],
                     i = [-100 * a, -100];
                 switch (n) {
                     case GS.Right:
                         s = [(e.x + e.width) * t[2] + t[0] + o, (e.y + e.height * a) * t[2] + t[1]], i = [0, -100 * a];
@@ -25723,21 +25723,21 @@
                         return o && e.push(o), e
                     }), [])), [e, g]),
                     p = xS(h, Zv),
                     {
                         transform: m,
                         nodeOrigin: y,
                         selectedNodesCount: S
-                    } = xS(Fv, f);
+                    } = xS(Kv, f);
                 if (!("boolean" == typeof i ? i : 1 === p.length && p[0].selected && 1 === S) || !p.length) return null;
                 const x = Sx(p, y),
                     b = Math.max(...p.map((e => (e[BS]?.z || 1) + 1))),
                     v = {
                         position: "absolute",
-                        transform: Kv(x, m, l, d, c),
+                        transform: Fv(x, m, l, d, c),
                         zIndex: b,
                         ...a
                     };
                 return (0, o.jsx)(Vv, {
                     children: (0, o.jsx)("div", {
                         style: v,
                         className: s(["react-flow__node-toolbar", n]),
@@ -26209,15 +26209,15 @@
                         [S, x, b, v] = OE({
                             sourceX: e.x,
                             sourceY: e.y,
                             targetX: n.x,
                             targetY: n.y
                         });
                     if (s[u] * i[u] == -1) {
-                        h = r.x || S, p = r.y || x;
+                        h = r.x ?? S, p = r.y ?? x;
                         const e = [{
                                 x: h,
                                 y: l.y
                             }, {
                                 x: h,
                                 y: d.y
                             }],
@@ -26405,55 +26405,55 @@
                     style: u,
                     markerEnd: g,
                     markerStart: h,
                     interactionWidth: p
                 })
             }));
 
-            function FE(e, t) {
+            function KE(e, t) {
                 return e >= 0 ? .5 * e : 25 * t * Math.sqrt(-e)
             }
 
-            function KE({
+            function FE({
                 pos: e,
                 x1: t,
                 y1: n,
                 x2: o,
                 y2: r,
                 c: a
             }) {
                 switch (e) {
                     case zE.Left:
-                        return [t - FE(t - o, a), n];
+                        return [t - KE(t - o, a), n];
                     case zE.Right:
-                        return [t + FE(o - t, a), n];
+                        return [t + KE(o - t, a), n];
                     case zE.Top:
-                        return [t, n - FE(n - r, a)];
+                        return [t, n - KE(n - r, a)];
                     case zE.Bottom:
-                        return [t, n + FE(r - n, a)]
+                        return [t, n + KE(r - n, a)]
                 }
             }
 
             function UE({
                 sourceX: e,
                 sourceY: t,
                 sourcePosition: n = zE.Bottom,
                 targetX: o,
                 targetY: r,
                 targetPosition: a = zE.Top,
                 curvature: s = .25
             }) {
-                const [i, l] = KE({
+                const [i, l] = FE({
                     pos: n,
                     x1: e,
                     y1: t,
                     x2: o,
                     y2: r,
                     c: s
-                }), [d, c] = KE({
+                }), [d, c] = FE({
                     pos: a,
                     x1: o,
                     y1: r,
                     x2: e,
                     y2: t,
                     c: s
                 }), [u, g, h, p] = IE({
@@ -27165,16 +27165,16 @@
                     noPanClassName: L,
                     nodeOrigin: j,
                     rfId: H,
                     autoPanOnConnect: Y,
                     autoPanOnNodeDrag: X,
                     onError: V,
                     connectionRadius: Z,
-                    isValidConnection: F,
-                    nodeDragThreshold: K
+                    isValidConnection: K,
+                    nodeDragThreshold: F
                 }) => {
                     const {
                         setNodes: U,
                         setEdges: W,
                         setDefaultNodesAndEdges: G,
                         setMinZoom: q,
                         setMaxZoom: Q,
@@ -27186,15 +27186,15 @@
                         const e = o?.map((e => ({
                             ...e,
                             ...P
                         })));
                         return G(n, e), () => {
                             te()
                         }
-                    }), []), zw("defaultEdgeOptions", P, ne.setState), zw("connectionMode", w, ne.setState), zw("onConnect", a, ne.setState), zw("onConnectStart", s, ne.setState), zw("onConnectEnd", i, ne.setState), zw("onClickConnectStart", l, ne.setState), zw("onClickConnectEnd", d, ne.setState), zw("nodesDraggable", c, ne.setState), zw("nodesConnectable", u, ne.setState), zw("nodesFocusable", g, ne.setState), zw("edgesFocusable", h, ne.setState), zw("edgesUpdatable", p, ne.setState), zw("elementsSelectable", E, ne.setState), zw("elevateNodesOnSelect", m, ne.setState), zw("snapToGrid", N, ne.setState), zw("snapGrid", C, ne.setState), zw("onNodesChange", b, ne.setState), zw("onEdgesChange", v, ne.setState), zw("connectOnClick", k, ne.setState), zw("fitViewOnInit", O, ne.setState), zw("fitViewOnInitOptions", I, ne.setState), zw("onNodesDelete", A, ne.setState), zw("onEdgesDelete", _, ne.setState), zw("onNodeDrag", D, ne.setState), zw("onNodeDragStart", R, ne.setState), zw("onNodeDragStop", B, ne.setState), zw("onSelectionDrag", z, ne.setState), zw("onSelectionDragStart", $, ne.setState), zw("onSelectionDragStop", T, ne.setState), zw("noPanClassName", L, ne.setState), zw("nodeOrigin", j, ne.setState), zw("rfId", H, ne.setState), zw("autoPanOnConnect", Y, ne.setState), zw("autoPanOnNodeDrag", X, ne.setState), zw("onError", V, ne.setState), zw("connectionRadius", Z, ne.setState), zw("isValidConnection", F, ne.setState), zw("nodeDragThreshold", K, ne.setState), Bw(e, U), Bw(t, W), Bw(y, q), Bw(S, Q), Bw(M, J), Bw(x, ee), null
+                    }), []), zw("defaultEdgeOptions", P, ne.setState), zw("connectionMode", w, ne.setState), zw("onConnect", a, ne.setState), zw("onConnectStart", s, ne.setState), zw("onConnectEnd", i, ne.setState), zw("onClickConnectStart", l, ne.setState), zw("onClickConnectEnd", d, ne.setState), zw("nodesDraggable", c, ne.setState), zw("nodesConnectable", u, ne.setState), zw("nodesFocusable", g, ne.setState), zw("edgesFocusable", h, ne.setState), zw("edgesUpdatable", p, ne.setState), zw("elementsSelectable", E, ne.setState), zw("elevateNodesOnSelect", m, ne.setState), zw("snapToGrid", N, ne.setState), zw("snapGrid", C, ne.setState), zw("onNodesChange", b, ne.setState), zw("onEdgesChange", v, ne.setState), zw("connectOnClick", k, ne.setState), zw("fitViewOnInit", O, ne.setState), zw("fitViewOnInitOptions", I, ne.setState), zw("onNodesDelete", A, ne.setState), zw("onEdgesDelete", _, ne.setState), zw("onNodeDrag", D, ne.setState), zw("onNodeDragStart", R, ne.setState), zw("onNodeDragStop", B, ne.setState), zw("onSelectionDrag", z, ne.setState), zw("onSelectionDragStart", $, ne.setState), zw("onSelectionDragStop", T, ne.setState), zw("noPanClassName", L, ne.setState), zw("nodeOrigin", j, ne.setState), zw("rfId", H, ne.setState), zw("autoPanOnConnect", Y, ne.setState), zw("autoPanOnNodeDrag", X, ne.setState), zw("onError", V, ne.setState), zw("connectionRadius", Z, ne.setState), zw("isValidConnection", K, ne.setState), zw("nodeDragThreshold", F, ne.setState), Bw(e, U), Bw(t, W), Bw(y, q), Bw(S, Q), Bw(M, J), Bw(x, ee), null
                 },
                 Tw = {
                     display: "none"
                 },
                 Lw = {
                     position: "absolute",
                     width: 1,
@@ -27233,15 +27233,15 @@
                 }, "Press enter or space to select a node.", !t && "You can then use the arrow keys to move the node around.", " Press delete to remove it and escape to cancel.", " "), a().createElement("div", {
                     id: `${Hw}-${e}`,
                     style: Tw
                 }, "Press enter or space to select an edge. You can then press delete to remove it or escape to cancel."), !t && a().createElement(Vw, {
                     rfId: e
                 }))
             }
-            var Fw = (e = null, t = {
+            var Kw = (e = null, t = {
                 actInsideInputWithModifier: !0
             }) => {
                 const [n, o] = (0, r.useState)(!1), a = (0, r.useRef)(!1), s = (0, r.useRef)(new Set([])), [i, l] = (0, r.useMemo)((() => {
                     if (null !== e) {
                         const t = (Array.isArray(e) ? e : [e]).filter((e => "string" == typeof e)).map((e => e.split("+"))),
                             n = t.reduce(((e, t) => e.concat(...t)), []);
                         return [t, n]
@@ -27254,54 +27254,56 @@
                 return (0, r.useEffect)((() => {
                     const n = "undefined" != typeof document ? document : null,
                         r = t?.target || n;
                     if (null !== e) {
                         const e = e => {
                                 if (a.current = e.ctrlKey || e.metaKey || e.shiftKey, (!a.current || a.current && !t.actInsideInputWithModifier) && wE(e)) return !1;
                                 const n = Uw(e.code, l);
-                                s.current.add(e[n]), Kw(i, s.current, !1) && (e.preventDefault(), o(!0))
+                                s.current.add(e[n]), Fw(i, s.current, !1) && (e.preventDefault(), o(!0))
                             },
                             n = e => {
                                 if ((!a.current || a.current && !t.actInsideInputWithModifier) && wE(e)) return !1;
                                 const n = Uw(e.code, l);
-                                Kw(i, s.current, !0) ? (o(!1), s.current.clear()) : s.current.delete(e[n]), "Meta" === e.key && s.current.clear(), a.current = !1
+                                Fw(i, s.current, !0) ? (o(!1), s.current.clear()) : s.current.delete(e[n]), "Meta" === e.key && s.current.clear(), a.current = !1
                             },
                             d = () => {
                                 s.current.clear(), o(!1)
                             };
                         return r?.addEventListener("keydown", e), r?.addEventListener("keyup", n), window.addEventListener("blur", d), () => {
                             r?.removeEventListener("keydown", e), r?.removeEventListener("keyup", n), window.removeEventListener("blur", d)
                         }
                     }
                 }), [e, o]), n
             };
 
-            function Kw(e, t, n) {
+            function Fw(e, t, n) {
                 return e.filter((e => n || e.length === t.size)).some((e => e.every((e => t.has(e)))))
             }
 
             function Uw(e, t) {
                 return t.includes(e) ? "code" : "key"
             }
 
             function Ww(e, t, n, o) {
-                if (!e.parentNode) return n;
-                const r = t.get(e.parentNode),
-                    a = ow(r, o);
-                return Ww(r, t, {
-                    x: (n.x ?? 0) + a.x,
-                    y: (n.y ?? 0) + a.y,
-                    z: (r[bE]?.z ?? 0) > (n.z ?? 0) ? r[bE]?.z ?? 0 : n.z ?? 0
+                const r = e.parentNode || e.parentId;
+                if (!r) return n;
+                const a = t.get(r),
+                    s = ow(a, o);
+                return Ww(a, t, {
+                    x: (n.x ?? 0) + s.x,
+                    y: (n.y ?? 0) + s.y,
+                    z: (a[bE]?.z ?? 0) > (n.z ?? 0) ? a[bE]?.z ?? 0 : n.z ?? 0
                 }, o)
             }
 
             function Gw(e, t, n) {
                 e.forEach((o => {
-                    if (o.parentNode && !e.has(o.parentNode)) throw new Error(`Parent node ${o.parentNode} not found`);
-                    if (o.parentNode || n?.[o.id]) {
+                    const r = o.parentNode || o.parentId;
+                    if (r && !e.has(r)) throw new Error(`Parent node ${r} not found`);
+                    if (r || n?.[o.id]) {
                         const {
                             x: r,
                             y: a,
                             z: s
                         } = Ww(o, e, {
                             ...o.position,
                             z: o[bE]?.z ?? 0
@@ -27323,21 +27325,22 @@
                         o = t.get(e.id),
                         i = {
                             ...e,
                             positionAbsolute: {
                                 x: e.position.x,
                                 y: e.position.y
                             }
-                        };
-                    e.parentNode && (a[e.parentNode] = !0);
-                    const l = o?.type && o?.type !== e.type;
+                        },
+                        l = e.parentNode || e.parentId;
+                    l && (a[l] = !0);
+                    const d = o?.type && o?.type !== e.type;
                     Object.defineProperty(i, bE, {
                         enumerable: !1,
                         value: {
-                            handleBounds: l ? void 0 : o?.[bE]?.handleBounds,
+                            handleBounds: d ? void 0 : o?.[bE]?.handleBounds,
                             z: n
                         }
                     }), r.set(e.id, i)
                 })), Gw(r, n, a), r
             }
 
             function Qw(e, t = {}) {
@@ -27638,16 +27641,17 @@
                             hasDefaultNodes: s,
                             hasDefaultEdges: i,
                             onNodesDelete: l,
                             onEdgesDelete: d,
                             onNodesChange: c,
                             onEdgesChange: u
                         } = t.getState(), g = (e || []).map((e => e.id)), h = (n || []).map((e => e.id)), p = r().reduce(((e, t) => {
-                            const n = !g.includes(t.id) && t.parentNode && e.find((e => e.id === t.parentNode));
-                            return ("boolean" != typeof t.deletable || t.deletable) && (g.includes(t.id) || n) && e.push(t), e
+                            const n = t.parentNode || t.parentId,
+                                o = !g.includes(t.id) && n && e.find((e => e.id === n));
+                            return ("boolean" != typeof t.deletable || t.deletable) && (g.includes(t.id) || o) && e.push(t), e
                         }), []), f = a.filter((e => "boolean" != typeof e.deletable || e.deletable)), m = f.filter((e => h.includes(e.id)));
                         if (p || m) {
                             const e = sw(p, f),
                                 n = [...m, ...e],
                                 r = n.reduce(((e, t) => (e.includes(t.id) || e.push(t.id), e)), []);
                             (i || s) && (i && t.setState({
                                 edges: a.filter((e => !r.includes(e.id)))
@@ -27763,15 +27767,15 @@
                         }),
                         {
                             d3Zoom: I,
                             d3Selection: A,
                             d3ZoomHandler: _,
                             userSelectionActive: D
                         } = rE(gC, f),
-                        R = Fw(x),
+                        R = Kw(x),
                         B = (0, r.useRef)(0),
                         z = (0, r.useRef)(!1),
                         $ = (0, r.useRef)();
                     return function(e) {
                         const t = aE();
                         (0, r.useEffect)((() => {
                             let n;
@@ -27804,15 +27808,15 @@
                                 d3ZoomHandler: n.on("wheel.zoom"),
                                 transform: [a.x, a.y, a.k],
                                 domNode: P.current.closest(".react-flow")
                             })
                         }
                     }), []), (0, r.useEffect)((() => {
                         A && I && (!l || R || D ? void 0 !== _ && A.on("wheel.zoom", (function(e, t) {
-                            if (!b || dC(e, E)) return null;
+                            if (!b && "wheel" === e.type && !e.ctrlKey || dC(e, E)) return null;
                             e.preventDefault(), _.call(this, e, t)
                         }), {
                             passive: !1
                         }) : A.on("wheel.zoom", (o => {
                             if (dC(o, E)) return !1;
                             o.preventDefault(), o.stopImmediatePropagation();
                             const r = A.property("__zoom").k || 1,
@@ -27920,30 +27924,31 @@
                         height: t.height,
                         transform: `translate(${t.x}px, ${t.y}px)`
                     }
                 }) : null
             }
 
             function mC(e, t) {
-                const n = e.find((e => e.id === t.parentNode));
-                if (n) {
-                    const e = t.position.x + t.width - n.width,
-                        o = t.position.y + t.height - n.height;
-                    if (e > 0 || o > 0 || t.position.x < 0 || t.position.y < 0) {
-                        if (n.style = {
-                                ...n.style
-                            } || {}, n.style.width = n.style.width ?? n.width, n.style.height = n.style.height ?? n.height, e > 0 && (n.style.width += e), o > 0 && (n.style.height += o), t.position.x < 0) {
+                const n = t.parentNode || t.parentId,
+                    o = e.find((e => e.id === n));
+                if (o) {
+                    const e = t.position.x + t.width - o.width,
+                        n = t.position.y + t.height - o.height;
+                    if (e > 0 || n > 0 || t.position.x < 0 || t.position.y < 0) {
+                        if (o.style = {
+                                ...o.style
+                            } || {}, o.style.width = o.style.width ?? o.width, o.style.height = o.style.height ?? o.height, e > 0 && (o.style.width += e), n > 0 && (o.style.height += n), t.position.x < 0) {
                             const e = Math.abs(t.position.x);
-                            n.position.x = n.position.x - e, n.style.width += e, t.position.x = 0
+                            o.position.x = o.position.x - e, o.style.width += e, t.position.x = 0
                         }
                         if (t.position.y < 0) {
                             const e = Math.abs(t.position.y);
-                            n.position.y = n.position.y - e, n.style.height += e, t.position.y = 0
+                            o.position.y = o.position.y - e, o.style.height += e, t.position.y = 0
                         }
-                        n.width = n.style.width, n.height = n.style.height
+                        o.width = o.style.width, o.height = o.style.height
                     }
                 }
             }
 
             function yC(e, t) {
                 if (e.some((e => "reset" === e.type))) return e.filter((e => "reset" === e.type)).map((e => e.item));
                 const n = e.filter((e => "add" === e.type)).map((e => e.item));
@@ -28126,31 +28131,32 @@
                         } : h,
                         ref: m,
                         style: iC
                     }, p, a().createElement(fC, null))
                 }));
 
             function CC(e, t) {
-                if (!e.parentNode) return !1;
-                const n = t.get(e.parentNode);
-                return !!n && (!!n.selected || CC(n, t))
+                const n = e.parentNode || e.parentId;
+                if (!n) return !1;
+                const o = t.get(n);
+                return !!o && (!!o.selected || CC(o, t))
             }
 
             function NC(e, t, n) {
                 let o = e;
                 do {
                     if (o?.matches(t)) return !0;
                     if (o === n.current) return !1;
                     o = o.parentElement
                 } while (o);
                 return !1
             }
 
             function MC(e, t, n, o) {
-                return Array.from(e.values()).filter((n => (n.selected || n.id === o) && (!n.parentNode || !CC(n, e)) && (n.draggable || t && void 0 === n.draggable))).map((e => ({
+                return Array.from(e.values()).filter((n => (n.selected || n.id === o) && (!n.parentNode || n.parentId || !CC(n, e)) && (n.draggable || t && void 0 === n.draggable))).map((e => ({
                     id: e.id,
                     position: e.position || {
                         x: 0,
                         y: 0
                     },
                     positionAbsolute: e.positionAbsolute || {
                         x: 0,
@@ -28161,66 +28167,68 @@
                         y: n.y - (e.positionAbsolute?.y ?? 0)
                     },
                     delta: {
                         x: 0,
                         y: 0
                     },
                     extent: e.extent,
-                    parentNode: e.parentNode,
+                    parentNode: e.parentNode || e.parentId,
+                    parentId: e.parentNode || e.parentId,
                     width: e.width,
                     height: e.height,
                     expandParent: e.expandParent
                 })))
             }
 
             function kC(e, t, n, o, r = [0, 0], a) {
                 const s = function(e, t) {
                     return t && "parent" !== t ? [t[0],
                         [t[1][0] - (e.width || 0), t[1][1] - (e.height || 0)]
                     ] : t
                 }(e, e.extent || o);
                 let i = s;
+                const l = e.parentNode || e.parentId;
                 if ("parent" !== e.extent || e.expandParent) {
-                    if (e.extent && e.parentNode && "parent" !== e.extent) {
-                        const t = n.get(e.parentNode),
+                    if (e.extent && l && "parent" !== e.extent) {
+                        const t = n.get(l),
                             {
                                 x: o,
                                 y: a
                             } = ow(t, r).positionAbsolute;
                         i = [
                             [e.extent[0][0] + o, e.extent[0][1] + a],
                             [e.extent[1][0] + o, e.extent[1][1] + a]
                         ]
                     }
-                } else if (e.parentNode && e.width && e.height) {
-                    const t = n.get(e.parentNode),
+                } else if (l && e.width && e.height) {
+                    const t = n.get(l),
                         {
                             x: o,
                             y: a
                         } = ow(t, r).positionAbsolute;
                     i = t && xE(o) && xE(a) && xE(t.width) && xE(t.height) ? [
                         [o + e.width * r[0], a + e.height * r[1]],
                         [o + t.width - e.width + e.width * r[0], a + t.height - e.height + e.height * r[1]]
                     ] : i
                 } else a?.("005", nE.error005()), i = s;
-                let l = {
+                let d = {
                     x: 0,
                     y: 0
                 };
-                if (e.parentNode) {
-                    const t = n.get(e.parentNode);
-                    l = ow(t, r).positionAbsolute
+                if (l) {
+                    const e = n.get(l);
+                    d = ow(e, r).positionAbsolute
                 }
-                const d = i && "parent" !== i ? gE(t, i) : t;
+                const c = i && "parent" !== i ? gE(t, i) : t;
                 return {
                     position: {
-                        x: d.x - l.x,
-                        y: d.y - l.y
+                        x: c.x - d.x,
+                        y: c.y - d.y
                     },
-                    positionAbsolute: d
+                    positionAbsolute: c
                 }
             }
 
             function PC({
                 nodeId: e,
                 dragItems: t,
                 nodeInternals: n
@@ -28566,42 +28574,43 @@
                     disableKeyboardA11y: B,
                     ariaLabel: z,
                     rfId: $,
                     hasHandleBounds: T
                 }) => {
                     const L = aE(),
                         j = (0, r.useRef)(null),
-                        H = (0, r.useRef)(N),
-                        Y = (0, r.useRef)(M),
-                        X = (0, r.useRef)(n),
-                        V = v || b || g || h || p || f,
-                        Z = BC(),
+                        H = (0, r.useRef)(null),
+                        Y = (0, r.useRef)(N),
+                        X = (0, r.useRef)(M),
+                        V = (0, r.useRef)(n),
+                        Z = v || b || g || h || p || f,
+                        K = BC(),
                         F = IC(t, L.getState, h),
-                        K = IC(t, L.getState, p),
-                        U = IC(t, L.getState, f),
-                        W = IC(t, L.getState, m),
-                        G = IC(t, L.getState, y);
+                        U = IC(t, L.getState, p),
+                        W = IC(t, L.getState, f),
+                        G = IC(t, L.getState, m),
+                        q = IC(t, L.getState, y);
                     (0, r.useEffect)((() => () => {
-                        j.current && P?.unobserve(j.current)
+                        H.current && P?.unobserve(H.current)
                     }), []), (0, r.useEffect)((() => {
                         if (j.current && !k) {
                             const e = j.current;
-                            R && T || (P?.unobserve(e), P?.observe(e))
+                            R && T || (H.current && P?.unobserve(H.current), P?.observe(e), H.current = e)
                         }
                     }), [k, R, T]), (0, r.useEffect)((() => {
-                        const e = X.current !== n,
-                            o = H.current !== N,
-                            r = Y.current !== M;
-                        j.current && (e || o || r) && (e && (X.current = n), o && (H.current = N), r && (Y.current = M), L.getState().updateNodeDimensions([{
+                        const e = V.current !== n,
+                            o = Y.current !== N,
+                            r = X.current !== M;
+                        j.current && (e || o || r) && (e && (V.current = n), o && (Y.current = N), r && (X.current = M), L.getState().updateNodeDimensions([{
                             id: t,
                             nodeElement: j.current,
                             forceUpdate: !0
                         }]))
                     }), [t, n, N, M]);
-                    const q = RC({
+                    const Q = RC({
                         nodeRef: j,
                         disabled: k || !b,
                         noDragClassName: _,
                         handleSelector: O,
                         nodeId: t,
                         isSelectable: v,
                         selectNodesOnDrag: C
@@ -28609,30 +28618,30 @@
                     return k ? null : a().createElement("div", {
                         className: s(["react-flow__node", `react-flow__node-${n}`, {
                             [D]: b
                         }, x, {
                             selected: u,
                             selectable: v,
                             parent: A,
-                            dragging: q
+                            dragging: Q
                         }]),
                         ref: j,
                         style: {
                             zIndex: I,
                             transform: `translate(${d}px,${c}px)`,
-                            pointerEvents: V ? "all" : "none",
+                            pointerEvents: Z ? "all" : "none",
                             visibility: R ? "visible" : "hidden",
                             ...S
                         },
                         "data-id": t,
                         "data-testid": `rf__node-${t}`,
                         onMouseEnter: F,
-                        onMouseMove: K,
-                        onMouseLeave: U,
-                        onContextMenu: W,
+                        onMouseMove: U,
+                        onMouseLeave: W,
+                        onContextMenu: G,
                         onClick: e => {
                             const {
                                 nodeDragThreshold: n
                             } = L.getState();
                             if (v && (!C || !b || n > 0) && AC({
                                     id: t,
                                     store: L,
@@ -28640,28 +28649,28 @@
                                 }), g) {
                                 const n = L.getState().nodeInternals.get(t);
                                 n && g(e, {
                                     ...n
                                 })
                             }
                         },
-                        onDoubleClick: G,
+                        onDoubleClick: q,
                         onKeyDown: w ? e => {
-                            if (!wE(e))
+                            if (!wE(e) && !B)
                                 if (vE.includes(e.key) && v) {
                                     const n = "Escape" === e.key;
                                     AC({
                                         id: t,
                                         store: L,
                                         unselect: n,
                                         nodeRef: j
                                     })
-                                } else !B && b && u && Object.prototype.hasOwnProperty.call(zC, e.key) && (L.setState({
+                                } else b && u && Object.prototype.hasOwnProperty.call(zC, e.key) && (L.setState({
                                     ariaLiveMessage: `Moved selected node ${e.key.replace("Arrow","").toLowerCase()}. New position, x: ${~~i}, y: ${~~l}`
-                                }), Z({
+                                }), K({
                                     x: zC[e.key].x,
                                     y: zC[e.key].y,
                                     isShiftPressed: e.shiftKey
                                 }))
                         } : void 0,
                         tabIndex: w ? 0 : void 0,
                         role: w ? "button" : void 0,
@@ -28675,15 +28684,15 @@
                         type: n,
                         xPos: i,
                         yPos: l,
                         selected: u,
                         isConnectable: E,
                         sourcePosition: N,
                         targetPosition: M,
-                        dragging: q,
+                        dragging: Q,
                         dragHandle: O,
                         zIndex: I
                     })))
                 };
                 return t.displayName = "NodeWrapper", (0, r.memo)(t)
             };
             const TC = e => {
@@ -28782,29 +28791,29 @@
                     preventScrolling: D,
                     onSelectionContextMenu: R,
                     noWheelClassName: B,
                     noPanClassName: z,
                     disableKeyboardA11y: $
                 }) => {
                     const T = rE(jC),
-                        L = Fw(h),
-                        j = Fw(x),
+                        L = Kw(h),
+                        j = Kw(x),
                         H = j || P,
                         Y = j || C,
                         X = L || p && !0 !== H;
                     return (({
                         deleteKeyCode: e,
                         multiSelectionKeyCode: t
                     }) => {
                         const n = aE(),
                             {
                                 deleteElements: o
                             } = aC(),
-                            a = Fw(e, sC),
-                            s = Fw(t);
+                            a = Kw(e, sC),
+                            s = Kw(t);
                         (0, r.useEffect)((() => {
                             if (a) {
                                 const {
                                     edges: e,
                                     getNodes: t
                                 } = n.getState(), r = t().filter((e => e.selected)), a = e.filter((e => e.selected));
                                 o({
@@ -28984,16 +28993,16 @@
                             disableKeyboardA11y: e.disableKeyboardA11y,
                             ariaLabel: r.ariaLabel,
                             hasHandleBounds: !!r[bE]?.handleBounds
                         })
                     })))
                 };
             ZC.displayName = "NodeRenderer";
-            var FC = (0, r.memo)(ZC);
-            const KC = (e, t, n) => n === zE.Left ? e - t : n === zE.Right ? e + t : e,
+            var KC = (0, r.memo)(ZC);
+            const FC = (e, t, n) => n === zE.Left ? e - t : n === zE.Right ? e + t : e,
                 UC = (e, t, n) => n === zE.Top ? e - t : n === zE.Bottom ? e + t : e,
                 WC = "react-flow__edgeupdater",
                 GC = ({
                     position: e,
                     centerX: t,
                     centerY: n,
                     radius: o = 10,
@@ -29002,15 +29011,15 @@
                     onMouseOut: l,
                     type: d
                 }) => a().createElement("circle", {
                     onMouseDown: r,
                     onMouseEnter: i,
                     onMouseOut: l,
                     className: s([WC, `${WC}-${d}`]),
-                    cx: KC(t, o, e),
+                    cx: FC(t, o, e),
                     cy: UC(n, o, e),
                     r: o,
                     stroke: "transparent",
                     fill: "transparent"
                 }),
                 qC = () => !0;
             var QC = e => {
@@ -29053,97 +29062,98 @@
                     markerEnd: L,
                     markerStart: j,
                     rfId: H,
                     ariaLabel: Y,
                     isFocusable: X,
                     isUpdatable: V,
                     pathOptions: Z,
-                    interactionWidth: F
+                    interactionWidth: K,
+                    disableKeyboardA11y: F
                 }) => {
-                    const K = (0, r.useRef)(null),
-                        [U, W] = (0, r.useState)(!1),
-                        [G, q] = (0, r.useState)(!1),
-                        Q = aE(),
-                        J = (0, r.useMemo)((() => `url('#${ew(j,H)}')`), [j, H]),
-                        ee = (0, r.useMemo)((() => `url('#${ew(L,H)}')`), [L, H]);
+                    const U = (0, r.useRef)(null),
+                        [W, G] = (0, r.useState)(!1),
+                        [q, Q] = (0, r.useState)(!1),
+                        J = aE(),
+                        ee = (0, r.useMemo)((() => `url('#${ew(j,H)}')`), [j, H]),
+                        te = (0, r.useMemo)((() => `url('#${ew(L,H)}')`), [L, H]);
                     if (P) return null;
-                    const te = PE(t, Q.getState, d),
-                        ne = PE(t, Q.getState, A),
-                        oe = PE(t, Q.getState, _),
-                        re = PE(t, Q.getState, D),
-                        ae = PE(t, Q.getState, R),
-                        se = (e, n) => {
+                    const ne = PE(t, J.getState, d),
+                        oe = PE(t, J.getState, A),
+                        re = PE(t, J.getState, _),
+                        ae = PE(t, J.getState, D),
+                        se = PE(t, J.getState, R),
+                        ie = (e, n) => {
                             if (0 !== e.button) return;
                             const {
                                 edges: o,
                                 isValidConnection: r
-                            } = Q.getState(), a = n ? b : x, s = (n ? I : O) || null, i = n ? "target" : "source", l = r || qC, d = n, c = o.find((e => e.id === t));
-                            q(!0), $?.(e, c, i), mw({
+                            } = J.getState(), a = n ? b : x, s = (n ? I : O) || null, i = n ? "target" : "source", l = r || qC, d = n, c = o.find((e => e.id === t));
+                            Q(!0), $?.(e, c, i), mw({
                                 event: e,
                                 handleId: s,
                                 nodeId: a,
                                 onConnect: e => z?.(c, e),
                                 isTarget: d,
-                                getState: Q.getState,
-                                setState: Q.setState,
+                                getState: J.getState,
+                                setState: J.setState,
                                 isValidConnection: l,
                                 edgeUpdaterType: i,
                                 onEdgeUpdateEnd: e => {
-                                    q(!1), T?.(e, c, i)
+                                    Q(!1), T?.(e, c, i)
                                 }
                             })
                         },
-                        ie = () => W(!0),
-                        le = () => W(!1),
-                        de = !k && !l;
+                        le = () => G(!0),
+                        de = () => G(!1),
+                        ce = !k && !l;
                     return a().createElement("g", {
                         className: s(["react-flow__edge", `react-flow__edge-${o}`, n, {
                             selected: c,
                             animated: u,
-                            inactive: de,
-                            updating: U
+                            inactive: ce,
+                            updating: W
                         }]),
                         onClick: e => {
                             const {
                                 edges: n,
                                 addSelectedEdges: o,
                                 unselectNodesAndEdges: r,
                                 multiSelectionActive: a
-                            } = Q.getState(), s = n.find((e => e.id === t));
-                            s && (k && (Q.setState({
+                            } = J.getState(), s = n.find((e => e.id === t));
+                            s && (k && (J.setState({
                                 nodesSelectionActive: !1
                             }), s.selected && a ? (r({
                                 nodes: [],
                                 edges: [s]
-                            }), K.current?.blur()) : o([t])), l && l(e, s))
+                            }), U.current?.blur()) : o([t])), l && l(e, s))
                         },
-                        onDoubleClick: te,
-                        onContextMenu: ne,
-                        onMouseEnter: oe,
-                        onMouseMove: re,
-                        onMouseLeave: ae,
+                        onDoubleClick: ne,
+                        onContextMenu: oe,
+                        onMouseEnter: re,
+                        onMouseMove: ae,
+                        onMouseLeave: se,
                         onKeyDown: X ? e => {
-                            if (vE.includes(e.key) && k) {
+                            if (!F && vE.includes(e.key) && k) {
                                 const {
                                     unselectNodesAndEdges: n,
                                     addSelectedEdges: o,
                                     edges: r
-                                } = Q.getState();
-                                "Escape" === e.key ? (K.current?.blur(), n({
+                                } = J.getState();
+                                "Escape" === e.key ? (U.current?.blur(), n({
                                     edges: [r.find((e => e.id === t))]
                                 })) : o([t])
                             }
                         } : void 0,
                         tabIndex: X ? 0 : void 0,
                         role: X ? "button" : "img",
                         "data-testid": `rf__edge-${t}`,
                         "aria-label": null === Y ? void 0 : Y || `Edge from ${x} to ${b}`,
                         "aria-describedby": X ? `${Hw}-${H}` : void 0,
-                        ref: K
-                    }, !G && a().createElement(e, {
+                        ref: U
+                    }, !q && a().createElement(e, {
                         id: t,
                         source: x,
                         target: b,
                         selected: c,
                         animated: u,
                         label: g,
                         labelStyle: h,
@@ -29157,35 +29167,35 @@
                         sourceY: E,
                         targetX: w,
                         targetY: C,
                         sourcePosition: N,
                         targetPosition: M,
                         sourceHandleId: O,
                         targetHandleId: I,
-                        markerStart: J,
-                        markerEnd: ee,
+                        markerStart: ee,
+                        markerEnd: te,
                         pathOptions: Z,
-                        interactionWidth: F
+                        interactionWidth: K
                     }), V && a().createElement(a().Fragment, null, ("source" === V || !0 === V) && a().createElement(GC, {
                         position: N,
                         centerX: v,
                         centerY: E,
                         radius: B,
-                        onMouseDown: e => se(e, !0),
-                        onMouseEnter: ie,
-                        onMouseOut: le,
+                        onMouseDown: e => ie(e, !0),
+                        onMouseEnter: le,
+                        onMouseOut: de,
                         type: "source"
                     }), ("target" === V || !0 === V) && a().createElement(GC, {
                         position: M,
                         centerX: w,
                         centerY: C,
                         radius: B,
-                        onMouseDown: e => se(e, !1),
-                        onMouseEnter: ie,
-                        onMouseOut: le,
+                        onMouseDown: e => ie(e, !1),
+                        onMouseEnter: le,
+                        onMouseOut: de,
                         type: "target"
                     })))
                 };
                 return t.displayName = "EdgeWrapper", (0, r.memo)(t)
             };
 
             function JC(e) {
@@ -29361,26 +29371,27 @@
                     onEdgeMouseMove: g,
                     onEdgeMouseLeave: h,
                     onEdgeClick: p,
                     edgeUpdaterRadius: m,
                     onEdgeDoubleClick: y,
                     onEdgeUpdateStart: S,
                     onEdgeUpdateEnd: x,
-                    children: b
+                    children: b,
+                    disableKeyboardA11y: v
                 }) => {
                     const {
-                        edgesFocusable: v,
-                        edgesUpdatable: E,
-                        elementsSelectable: w,
-                        width: C,
-                        height: N,
-                        connectionMode: M,
-                        nodeInternals: k,
-                        onError: P
-                    } = rE(lN, f), O = function(e, t, n) {
+                        edgesFocusable: E,
+                        edgesUpdatable: w,
+                        elementsSelectable: C,
+                        width: N,
+                        height: M,
+                        connectionMode: k,
+                        nodeInternals: P,
+                        onError: O
+                    } = rE(lN, f), I = function(e, t, n) {
                         return function(e, t, n = !1) {
                             let o = -1;
                             const r = e.reduce(((e, r) => {
                                     const a = xE(r.zIndex);
                                     let s = a ? r.zIndex : 0;
                                     if (n) {
                                         const e = t.get(r.target),
@@ -29444,64 +29455,64 @@
                                 targetWidth: r.width,
                                 targetHeight: r.height,
                                 width: n.width,
                                 height: n.height,
                                 transform: n.transform
                             })
                         })) : n.edges), [e, t])), t, n)
-                    }(t, k, n);
-                    return C ? a().createElement(a().Fragment, null, O.map((({
+                    }(t, P, n);
+                    return N ? a().createElement(a().Fragment, null, I.map((({
                         level: t,
                         edges: n,
                         isMaxLevel: r
                     }) => a().createElement("svg", {
                         key: t,
                         style: {
                             zIndex: t
                         },
-                        width: C,
-                        height: N,
+                        width: N,
+                        height: M,
                         className: "react-flow__edges react-flow__container"
                     }, r && a().createElement(iN, {
                         defaultColor: e,
                         rfId: o
                     }), a().createElement("g", null, n.map((e => {
-                        const [t, n, r] = nN(k.get(e.source)), [f, b, C] = nN(k.get(e.target));
-                        if (!r || !C) return null;
-                        let N = e.type || "default";
-                        i[N] || (P?.("011", nE.error011(N)), N = "default");
-                        const O = i[N] || i.default,
-                            I = M === AE.Strict ? b.target : (b.target ?? []).concat(b.source ?? []),
-                            A = tN(n.source, e.sourceHandle),
-                            _ = tN(I, e.targetHandle),
-                            D = A?.position || zE.Bottom,
-                            R = _?.position || zE.Top,
-                            B = !!(e.focusable || v && void 0 === e.focusable),
-                            z = void 0 !== d && (e.updatable || E && void 0 === e.updatable);
-                        if (!A || !_) return P?.("008", nE.error008(A, e)), null;
+                        const [t, n, r] = nN(P.get(e.source)), [f, b, N] = nN(P.get(e.target));
+                        if (!r || !N) return null;
+                        let M = e.type || "default";
+                        i[M] || (O?.("011", nE.error011(M)), M = "default");
+                        const I = i[M] || i.default,
+                            A = k === AE.Strict ? b.target : (b.target ?? []).concat(b.source ?? []),
+                            _ = tN(n.source, e.sourceHandle),
+                            D = tN(A, e.targetHandle),
+                            R = _?.position || zE.Bottom,
+                            B = D?.position || zE.Top,
+                            z = !!(e.focusable || E && void 0 === e.focusable),
+                            $ = void 0 !== d && (e.updatable || w && void 0 === e.updatable);
+                        if (!_ || !D) return O?.("008", nE.error008(_, e)), null;
                         const {
-                            sourceX: $,
-                            sourceY: T,
-                            targetX: L,
-                            targetY: j
+                            sourceX: T,
+                            sourceY: L,
+                            targetX: j,
+                            targetY: H
                         } = ((e, t, n, o, r, a) => {
                             const s = eN(n, e, t),
                                 i = eN(a, o, r);
                             return {
                                 sourceX: s.x,
                                 sourceY: s.y,
                                 targetX: i.x,
                                 targetY: i.y
                             }
-                        })(t, A, D, f, _, R);
-                        return a().createElement(O, {
+                        })(t, _, R, f, D, B);
+                        return a().createElement(I, {
                             key: e.id,
                             id: e.id,
                             className: s([e.className, l]),
-                            type: N,
+                            type: M,
                             data: e.data,
                             selected: !!e.selected,
                             animated: !!e.animated,
                             hidden: !!e.hidden,
                             label: e.label,
                             labelStyle: e.labelStyle,
                             labelShowBg: e.labelShowBg,
@@ -29511,37 +29522,38 @@
                             style: e.style,
                             source: e.source,
                             target: e.target,
                             sourceHandleId: e.sourceHandle,
                             targetHandleId: e.targetHandle,
                             markerEnd: e.markerEnd,
                             markerStart: e.markerStart,
-                            sourceX: $,
-                            sourceY: T,
-                            targetX: L,
-                            targetY: j,
-                            sourcePosition: D,
-                            targetPosition: R,
-                            elementsSelectable: w,
+                            sourceX: T,
+                            sourceY: L,
+                            targetX: j,
+                            targetY: H,
+                            sourcePosition: R,
+                            targetPosition: B,
+                            elementsSelectable: C,
                             onEdgeUpdate: d,
                             onContextMenu: c,
                             onMouseEnter: u,
                             onMouseMove: g,
                             onMouseLeave: h,
                             onClick: p,
                             edgeUpdaterRadius: m,
                             onEdgeDoubleClick: y,
                             onEdgeUpdateStart: S,
                             onEdgeUpdateEnd: x,
                             rfId: o,
                             ariaLabel: e.ariaLabel,
-                            isFocusable: B,
-                            isUpdatable: z,
+                            isFocusable: z,
+                            isUpdatable: $,
                             pathOptions: "pathOptions" in e ? e.pathOptions : void 0,
-                            interactionWidth: e.interactionWidth
+                            interactionWidth: e.interactionWidth,
+                            disableKeyboardA11y: v
                         })
                     })))))), b) : null
                 };
             dN.displayName = "EdgeRenderer";
             var cN = (0, r.memo)(dN);
             const uN = e => `translate(${e.transform[0]}px,${e.transform[1]}px) scale(${e.transform[2]})`;
 
@@ -29710,16 +29722,16 @@
                 zoomOnScroll: L,
                 zoomOnPinch: j,
                 panOnScroll: H,
                 panOnScrollSpeed: Y,
                 panOnScrollMode: X,
                 zoomOnDoubleClick: V,
                 panOnDrag: Z,
-                onPaneClick: F,
-                onPaneMouseEnter: K,
+                onPaneClick: K,
+                onPaneMouseEnter: F,
                 onPaneMouseMove: U,
                 onPaneMouseLeave: W,
                 onPaneScroll: G,
                 onPaneContextMenu: q,
                 onEdgeUpdate: Q,
                 onEdgeContextMenu: J,
                 onEdgeMouseEnter: ee,
@@ -29742,16 +29754,16 @@
                 return function(e) {
                     const t = aC(),
                         n = (0, r.useRef)(!1);
                     (0, r.useEffect)((() => {
                         !n.current && t.viewportInitialized && e && (setTimeout((() => e(t)), 1), n.current = !0)
                     }), [e, t.viewportInitialized])
                 }(i), a().createElement(YC, {
-                    onPaneClick: F,
-                    onPaneMouseEnter: K,
+                    onPaneClick: K,
+                    onPaneMouseEnter: F,
                     onPaneMouseMove: U,
                     onPaneMouseLeave: W,
                     onPaneContextMenu: q,
                     onPaneScroll: G,
                     deleteKeyCode: O,
                     selectionKeyCode: w,
                     selectionOnDrag: C,
@@ -29803,15 +29815,15 @@
                 }, a().createElement(mN, {
                     style: b,
                     type: x,
                     component: v,
                     containerStyle: E
                 })), a().createElement("div", {
                     className: "react-flow__edgelabel-renderer"
-                }), a().createElement(FC, {
+                }), a().createElement(KC, {
                     nodeTypes: pe,
                     onNodeClick: l,
                     onNodeDoubleClick: c,
                     onNodeMouseEnter: g,
                     onNodeMouseMove: h,
                     onNodeMouseLeave: p,
                     onNodeContextMenu: f,
@@ -29943,15 +29955,22 @@
                             if (!c) return;
                             const u = window.getComputedStyle(c),
                                 {
                                     m22: g
                                 } = new window.DOMMatrixReadOnly(u.transform),
                                 h = n.reduce(((e, t) => {
                                     const n = r.get(t.id);
-                                    if (n) {
+                                    if (n?.hidden) r.set(n.id, {
+                                        ...n,
+                                        [bE]: {
+                                            ...n[bE],
+                                            handleBounds: void 0
+                                        }
+                                    });
+                                    else if (n) {
                                         const o = cE(t.nodeElement);
                                         o.width && o.height && (n.width !== o.width || n.height !== o.height || t.forceUpdate) && (r.set(n.id, {
                                             ...n,
                                             [bE]: {
                                                 ...n[bE],
                                                 handleBounds: {
                                                     source: OC(".source", t.nodeElement, g, d),
@@ -30205,16 +30224,16 @@
                     connectionLineStyle: L,
                     connectionLineComponent: j,
                     connectionLineContainerStyle: H,
                     deleteKeyCode: Y = "Backspace",
                     selectionKeyCode: X = "Shift",
                     selectionOnDrag: V = !1,
                     selectionMode: Z = DE.Full,
-                    panActivationKeyCode: F = "Space",
-                    multiSelectionKeyCode: K = (ME() ? "Meta" : "Control"),
+                    panActivationKeyCode: K = "Space",
+                    multiSelectionKeyCode: F = (ME() ? "Meta" : "Control"),
                     zoomActivationKeyCode: U = (ME() ? "Meta" : "Control"),
                     snapToGrid: W = !1,
                     snapGrid: G = kN,
                     onlyRenderVisibleElements: q = !1,
                     selectNodesOnDrag: Q = !0,
                     nodesDraggable: J,
                     nodesConnectable: ee,
@@ -30259,16 +30278,16 @@
                     noWheelClassName: Le = "nowheel",
                     noPanClassName: je = "nopan",
                     fitView: He = !1,
                     fitViewOptions: Ye,
                     connectOnClick: Xe = !0,
                     attributionPosition: Ve,
                     proOptions: Ze,
-                    defaultEdgeOptions: Fe,
-                    elevateNodesOnSelect: Ke = !0,
+                    defaultEdgeOptions: Ke,
+                    elevateNodesOnSelect: Fe = !0,
                     elevateEdgesOnSelect: Ue = !1,
                     disableKeyboardA11y: We = !1,
                     autoPanOnConnect: Ge = !0,
                     autoPanOnNodeDrag: qe = !0,
                     connectionRadius: Qe = 20,
                     isValidConnection: Je,
                     onError: et,
@@ -30306,16 +30325,16 @@
                         connectionLineStyle: L,
                         connectionLineComponent: j,
                         connectionLineContainerStyle: H,
                         selectionKeyCode: X,
                         selectionOnDrag: V,
                         selectionMode: Z,
                         deleteKeyCode: Y,
-                        multiSelectionKeyCode: K,
-                        panActivationKeyCode: F,
+                        multiSelectionKeyCode: F,
+                        panActivationKeyCode: K,
                         zoomActivationKeyCode: U,
                         onlyRenderVisibleElements: q,
                         selectNodesOnDrag: Q,
                         defaultViewport: se,
                         translateExtent: de,
                         minZoom: ie,
                         maxZoom: le,
@@ -30366,26 +30385,26 @@
                         onClickConnectEnd: x,
                         nodesDraggable: J,
                         nodesConnectable: ee,
                         nodesFocusable: te,
                         edgesFocusable: oe,
                         edgesUpdatable: re,
                         elementsSelectable: ae,
-                        elevateNodesOnSelect: Ke,
+                        elevateNodesOnSelect: Fe,
                         minZoom: ie,
                         maxZoom: le,
                         nodeExtent: ue,
                         onNodesChange: ze,
                         onEdgesChange: $e,
                         snapToGrid: W,
                         snapGrid: G,
                         connectionMode: $,
                         translateExtent: de,
                         connectOnClick: Xe,
-                        defaultEdgeOptions: Fe,
+                        defaultEdgeOptions: Ke,
                         fitView: He,
                         fitViewOptions: Ye,
                         onNodesDelete: P,
                         onEdgesDelete: O,
                         onNodeDragStart: N,
                         onNodeDrag: M,
                         onNodeDragStop: k,
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/713.672682fff3504f6c1da4.js.LICENSE.txt` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/713.a7e0851307239af436d3.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/remoteEntry.b2c83b834b57cd054825.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/remoteEntry.3f9ee25d572774e2a4f2.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, a, i, l, u, f, s, p, c, d, h, v, m, b, g, y, w = {
+    var e, r, t, n, o, a, i, l, u, s, c, f, p, d, h, v, m, b, g, y, w = {
             212: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(345), t.e(581)]).then((() => () => t(581))),
-                        "./extension": () => Promise.all([t.e(345), t.e(581)]).then((() => () => t(581))),
+                        "./index": () => Promise.all([t.e(345), t.e(736)]).then((() => () => t(736))),
+                        "./extension": () => Promise.all([t.e(345), t.e(736)]).then((() => () => t(736))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     a = (e, r) => {
                         if (t.S) {
@@ -43,55 +43,55 @@
         }), r
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
-        345: "de49bbff53600e2e5ba6",
+        345: "5110416d57db1c92d66e",
         432: "df81fd96e756f14c54d0",
-        581: "303d96e32a4c90e28d98",
-        628: "82e0acc77e82f2f867e2",
-        713: "672682fff3504f6c1da4"
+        628: "859da3aec42bcfc412c5",
+        713: "a7e0851307239af436d3",
+        736: "61ace78c7785abf59833"
     } [e] + ".js?v=" + {
-        345: "de49bbff53600e2e5ba6",
+        345: "5110416d57db1c92d66e",
         432: "df81fd96e756f14c54d0",
-        581: "303d96e32a4c90e28d98",
-        628: "82e0acc77e82f2f867e2",
-        713: "672682fff3504f6c1da4"
+        628: "859da3aec42bcfc412c5",
+        713: "a7e0851307239af436d3",
+        736: "61ace78c7785abf59833"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-core:", P.l = (t, n, o, a) => {
         if (e[t]) e[t].push(n);
         else {
             var i, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        i = s;
+                for (var u = document.getElementsByTagName("script"), s = 0; s < u.length; s++) {
+                    var c = u[s];
+                    if (c.getAttribute("src") == t || c.getAttribute("data-webpack") == r + o) {
+                        i = c;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + o), i.src = t), e[t] = [n];
-            var p = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(c);
+            var f = (r, n) => {
+                    i.onerror = i.onload = null, clearTimeout(p);
                     var o = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                c = setTimeout(p.bind(null, void 0, {
+                p = setTimeout(f.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = p.bind(null, i.onerror), i.onload = p.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -113,15 +113,15 @@
                         (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (o[r] = {
                             get: t,
                             from: i,
                             eager: !!n
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-components-core", "0.1.3", (() => Promise.all([P.e(345), P.e(581)]).then((() => () => P(581))))), l("reactflow", "11.7.2", (() => Promise.all([P.e(713), P.e(345), P.e(628)]).then((() => () => P(713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-components-core", "0.1.6", (() => Promise.all([P.e(345), P.e(736)]).then((() => () => P(736))))), l("reactflow", "11.7.2", (() => Promise.all([P.e(713), P.e(345), P.e(628)]).then((() => () => P(713)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -171,73 +171,73 @@
     }, a = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, p = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == p ? l > n && !o : "" == p != o);
-                if ("u" == s) {
-                    if (!u || "u" != p) return !1
+                var s, c, f = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (c = (typeof(s = r[i]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
+                if ("u" == c) {
+                    if (!u || "u" != f) return !1
                 } else if (u)
-                    if (p == s)
+                    if (f == c)
                         if (l <= n) {
-                            if (f != e[l]) return !1
+                            if (s != e[l]) return !1
                         } else {
-                            if (o ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (o ? s > e[l] : s < e[l]) return !1;
+                            s != e[l] && (u = !1)
                         }
-                else if ("s" != p && "n" != p) {
+                else if ("s" != f && "n" != f) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < p != o) return !1;
+                    if (l <= n || c < f != o) return !1;
                     u = !1
-                } else "s" != p && "n" != p && (u = !1, l--)
+                } else "s" != f && "n" != f && (u = !1, l--)
             }
         }
-        var c = [],
-            d = c.pop.bind(c);
+        var p = [],
+            d = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            c.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
+            p.push(1 == h ? d() | d() : 2 == h ? d() & d() : h ? a(h, r) : !d())
         }
         return !!d()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", s = (e, r, t, n) => {
         var o = l(e, t);
-        return a(n, o) || p(u(e, t, o, n)), c(e[t][o])
-    }, s = (e, r, t) => {
+        return a(n, o) || f(u(e, t, o, n)), p(e[t][o])
+    }, c = (e, r, t) => {
         var o = e[r];
         return (r = Object.keys(o).reduce(((e, r) => !a(t, r) || e && !n(e, r) ? e : r), 0)) && o[r]
-    }, p = e => {
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, c = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
+    }, p = e => (e.loaded = 1, e.get()), h = (d = e => function(r, t, n, o) {
         var a = P.I(r);
         return a && a.then ? a.then(e.bind(e, r, P.S[r], t, n, o)) : e(r, P.S[r], t, n, o)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), v = d(((e, r, t, n, o) => {
-        var a = r && P.o(r, t) && s(r, t, n);
-        return a ? c(a) : o()
+    })(((e, r, t, n) => (i(e, t), s(r, 0, t, n)))), v = d(((e, r, t, n, o) => {
+        var a = r && P.o(r, t) && c(r, t, n);
+        return a ? p(a) : o()
     })), m = {}, b = {
         345: () => h("default", "react", [1, 18, 2, 0]),
-        153: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
         254: () => h("default", "@amphi/pipeline-components-manager", [0]),
         473: () => v("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([P.e(713), P.e(628)]).then((() => () => P(713))))),
+        664: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
         628: () => h("default", "react-dom", [1, 18, 2, 0])
     }, g = {
         345: [345],
-        581: [153, 254, 473],
-        628: [628]
+        628: [628],
+        736: [254, 473, 664]
     }, y = {}, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
             if (P.o(m, e)) return r.push(m[e]);
             if (!y[e]) {
                 var t = r => {
                     m[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-core/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-core/static/third-party-licenses.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9943181818181819%*

 * *Differences: {"'packages'": "{6: {'versionInfo': '5.0.5'}, 7: {'versionInfo': '6.11.0'}}"}*

```diff
@@ -36,21 +36,21 @@
             "name": "@reactflow/node-toolbar",
             "versionInfo": "1.2.1"
         },
         {
             "extractedText": "Copyright \u00a9 Jorge Bucaran <<https://jorgebucaran.com>>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "classcat",
-            "versionInfo": "5.0.4"
+            "versionInfo": "5.0.5"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "Copyright 2010-2022 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
             "licenseId": "ISC",
             "name": "d3-color",
             "versionInfo": "3.1.0"
         },
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/package.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9648719336219336%*

 * *Differences: {"'dependencies'": "{'antd': '^5.16.0', 'react-dnd': '^16.0.1', 'react-dnd-html5-backend': "*

 * *                   "'^16.0.1', 'styled-components': '^6.1.8', delete: ['@headlessui/react']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.ab2053fa193201a8aa0a.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -3,21 +3,24 @@
         "email": "tgourdel@amphi.ai",
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
-        "@headlessui/react": "^1.7.18",
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.1.5",
         "@lumino/widgets": "^2.0.0",
+        "antd": "^5.16.0",
+        "react-dnd": "^16.0.1",
+        "react-dnd-html5-backend": "^16.0.1",
         "react-dom": "^18.2.0",
         "react-flow-renderer": "^10.3.17",
-        "react-select": "^5.8.0"
+        "react-select": "^5.8.0",
+        "styled-components": "^6.1.8"
     },
     "description": "Amphi Pipeline Components Manager",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
@@ -41,15 +44,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.3ff8b1671edf3719adc7.js",
+            "load": "static/remoteEntry.ab2053fa193201a8aa0a.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-components-manager",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundle": false,
@@ -90,9 +93,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.6"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/432.0488919b1f7178c806d4.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/432.5fd4f051d4b18df45075.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -1,22 +1,22 @@
 "use strict";
 (self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || []).push([
     [432], {
-        296: (e, t, n) => {
+        4296: (e, t, n) => {
             n.d(t, {
                 A: () => c
             });
-            var r = n(758),
+            var r = n(6758),
                 a = n.n(r),
-                o = n(935),
+                o = n(6173),
                 i = n.n(o)()(a());
             i.push([e.id, "/*-----------------------------------------------------------------------------\n| Copyright (c) Jupyter Development Team.\n| Distributed under the terms of the Modified BSD License.\n|----------------------------------------------------------------------------*/\n\n/* stylelint-disable selector-class-pattern */\n.jp-TopAreaText {\n    display: flex;\n    justify-content: center;\n    align-items: center;\n    margin-left: auto;\n    margin-right:10px;\n  }", ""]);
             const c = i
         },
-        935: e => {
+        6173: e => {
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
                         var n = "",
                             r = void 0 !== t[5];
                         return t[4] && (n += "@supports (".concat(t[4], ") {")), t[2] && (n += "@media ".concat(t[2], " {")), r && (n += "@layer".concat(t[5].length > 0 ? " ".concat(t[5]) : "", " {")), n += e(t), r && (n += "}"), t[2] && (n += "}"), t[4] && (n += "}"), n
@@ -34,20 +34,20 @@
                     for (var u = 0; u < e.length; u++) {
                         var p = [].concat(e[u]);
                         r && i[p[0]] || (void 0 !== o && (void 0 === p[5] || (p[1] = "@layer".concat(p[5].length > 0 ? " ".concat(p[5]) : "", " {").concat(p[1], "}")), p[5] = o), n && (p[2] ? (p[1] = "@media ".concat(p[2], " {").concat(p[1], "}"), p[2] = n) : p[2] = n), a && (p[4] ? (p[1] = "@supports (".concat(p[4], ") {").concat(p[1], "}"), p[4] = a) : p[4] = "".concat(a)), t.push(p))
                     }
                 }, t
             }
         },
-        758: e => {
+        6758: e => {
             e.exports = function(e) {
                 return e[1]
             }
         },
-        591: e => {
+        2591: e => {
             var t = [];
 
             function n(e) {
                 for (var n = -1, r = 0; r < t.length; r++)
                     if (t[r].identifier === e) {
                         n = r;
                         break
@@ -105,15 +105,15 @@
                         var p = n(o[u]);
                         0 === t[p].references && (t[p].updater(), t.splice(p, 1))
                     }
                     o = s
                 }
             }
         },
-        128: e => {
+        8128: e => {
             var t = {};
             e.exports = function(e, n) {
                 var r = function(e) {
                     if (void 0 === t[e]) {
                         var n = document.querySelector(e);
                         if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
                             n = n.contentDocument.head
@@ -124,27 +124,27 @@
                     }
                     return t[e]
                 }(e);
                 if (!r) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
                 r.appendChild(n)
             }
         },
-        51: e => {
+        3051: e => {
             e.exports = function(e) {
                 var t = document.createElement("style");
                 return e.setAttributes(t, e.attributes), e.insert(t, e.options), t
             }
         },
         855: (e, t, n) => {
             e.exports = function(e) {
                 var t = n.nc;
                 t && e.setAttribute("nonce", t)
             }
         },
-        740: e => {
+        1740: e => {
             e.exports = function(e) {
                 if ("undefined" == typeof document) return {
                     update: function() {},
                     remove: function() {}
                 };
                 var t = e.insertStyleElement(e);
                 return {
@@ -163,36 +163,36 @@
                             if (null === e.parentNode) return !1;
                             e.parentNode.removeChild(e)
                         }(t)
                     }
                 }
             }
         },
-        656: e => {
+        3656: e => {
             e.exports = function(e, t) {
                 if (t.styleSheet) t.styleSheet.cssText = e;
                 else {
                     for (; t.firstChild;) t.removeChild(t.firstChild);
                     t.appendChild(document.createTextNode(e))
                 }
             }
         },
-        432: (e, t, n) => {
+        1432: (e, t, n) => {
             n.r(t);
-            var r = n(591),
+            var r = n(2591),
                 a = n.n(r),
-                o = n(740),
+                o = n(1740),
                 i = n.n(o),
-                c = n(128),
+                c = n(8128),
                 s = n.n(c),
                 u = n(855),
                 p = n.n(u),
-                l = n(51),
+                l = n(3051),
                 f = n.n(l),
-                d = n(656),
+                d = n(3656),
                 m = n.n(d),
-                v = n(296),
+                v = n(4296),
                 h = {};
             h.styleTagTransform = m(), h.setAttributes = p(), h.insert = s().bind(null, "head"), h.domAPI = i(), h.insertStyleElement = f(), a()(v.A, h), v.A && v.A.locals && v.A.locals
         }
     }
 ]);
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/remoteEntry.3ff8b1671edf3719adc7.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-components-manager/static/remoteEntry.ab2053fa193201a8aa0a.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -1,304 +1,313 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, a, o, i, l, u, f, s, d, p, c, h, m, v, b, g, y, w = {
-            548: (e, r, t) => {
-                var n = {
-                        "./index": () => Promise.all([t.e(969), t.e(638), t.e(298)]).then((() => () => t(298))),
-                        "./extension": () => Promise.all([t.e(969), t.e(638), t.e(298)]).then((() => () => t(298))),
-                        "./style": () => t.e(432).then((() => () => t(432)))
+    var e, r, t, a, n, o, i, l, f, u, d, c, s, p, h, m, b, v, g, y, w = {
+            5548: (e, r, t) => {
+                var a = {
+                        "./index": () => Promise.all([t.e(143), t.e(379), t.e(345), t.e(628), t.e(893)]).then((() => () => t(893))),
+                        "./extension": () => Promise.all([t.e(143), t.e(379), t.e(345), t.e(628), t.e(893)]).then((() => () => t(893))),
+                        "./style": () => t.e(432).then((() => () => t(1432)))
                     },
-                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
+                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
-                            var n = "default",
-                                a = t.S[n];
-                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[n] = e, t.I(n, r)
+                            var a = "default",
+                                n = t.S[a];
+                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[a] = e, t.I(a, r)
                         }
                     };
                 t.d(r, {
-                    get: () => a,
+                    get: () => n,
                     init: () => o
                 })
             }
         },
         S = {};
 
     function P(e) {
         var r = S[e];
         if (void 0 !== r) return r.exports;
         var t = S[e] = {
             id: e,
             exports: {}
         };
-        return w[e](t, t.exports, P), t.exports
+        return w[e].call(t.exports, t, t.exports, P), t.exports
     }
     P.m = w, P.c = S, P.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return P.d(r, {
             a: r
         }), r
     }, P.d = (e, r) => {
         for (var t in r) P.o(r, t) && !P.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, P.f = {}, P.e = e => Promise.all(Object.keys(P.f).reduce(((r, t) => (P.f[t](e, r), r)), [])), P.u = e => e + "." + {
-        2: "5ff850f38644d809e786",
-        298: "73d1171d6e28e5430245",
-        432: "0488919b1f7178c806d4",
-        621: "8e6964da49a7b28e9978",
-        638: "e2b9768060399c681ec9",
-        649: "6d49d9cc69cbb76697fb",
-        969: "848e74820ca03d893303"
+        12: "e1b4412a18535c560cd1",
+        85: "227e3aea03a3014cd80a",
+        143: "c7653d290fba1605b212",
+        345: "3292eea9d7af2efbde78",
+        379: "1427c0520c9ac5a71632",
+        432: "5fd4f051d4b18df45075",
+        454: "b60aaa09eed0e7e4a124",
+        628: "9846ca5c6c20882d89fe",
+        893: "7652ea10634779c3ef2f",
+        974: "866b25e149fe0014eb94"
     } [e] + ".js?v=" + {
-        2: "5ff850f38644d809e786",
-        298: "73d1171d6e28e5430245",
-        432: "0488919b1f7178c806d4",
-        621: "8e6964da49a7b28e9978",
-        638: "e2b9768060399c681ec9",
-        649: "6d49d9cc69cbb76697fb",
-        969: "848e74820ca03d893303"
+        12: "e1b4412a18535c560cd1",
+        85: "227e3aea03a3014cd80a",
+        143: "c7653d290fba1605b212",
+        345: "3292eea9d7af2efbde78",
+        379: "1427c0520c9ac5a71632",
+        432: "5fd4f051d4b18df45075",
+        454: "b60aaa09eed0e7e4a124",
+        628: "9846ca5c6c20882d89fe",
+        893: "7652ea10634779c3ef2f",
+        974: "866b25e149fe0014eb94"
     } [e], P.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-manager:", P.l = (t, n, a, o) => {
-        if (e[t]) e[t].push(n);
+    }(), P.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-components-manager:", P.l = (t, a, n, o) => {
+        if (e[t]) e[t].push(a);
         else {
             var i, l;
-            if (void 0 !== a)
-                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
-                    var s = u[f];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + a) {
-                        i = s;
+            if (void 0 !== n)
+                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
+                    var d = f[u];
+                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
+                        i = d;
                         break
                     }
                 }
-            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + a), i.src = t), e[t] = [n];
-            var d = (r, n) => {
-                    i.onerror = i.onload = null, clearTimeout(p);
-                    var a = e[t];
-                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), a && a.forEach((e => e(n))), r) return r(n)
+            i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, P.nc && i.setAttribute("nonce", P.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
+            var c = (r, a) => {
+                    i.onerror = i.onload = null, clearTimeout(s);
+                    var n = e[t];
+                    if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(d.bind(null, void 0, {
+                s = setTimeout(c.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = d.bind(null, i.onerror), i.onload = d.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = c.bind(null, i.onerror), i.onload = c.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, P.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         P.S = {};
         var e = {},
             r = {};
-        P.I = (t, n) => {
-            n || (n = []);
-            var a = r[t];
-            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
-                if (n.push(a), e[t]) return e[t];
+        P.I = (t, a) => {
+            a || (a = []);
+            var n = r[t];
+            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
+                if (a.push(n), e[t]) return e[t];
                 P.o(P.S, t) || (P.S[t] = {});
                 var o = P.S[t],
                     i = "@amphi/pipeline-components-manager",
-                    l = (e, r, t, n) => {
-                        var a = o[e] = o[e] || {},
-                            l = a[r];
-                        (!l || !l.loaded && (!n != !l.eager ? n : i > l.from)) && (a[r] = {
+                    l = (e, r, t, a) => {
+                        var n = o[e] = o[e] || {},
+                            l = n[r];
+                        (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
-                            eager: !!n
+                            eager: !!a
                         })
                     },
-                    u = [];
-                return "default" === t && (l("@amphi/pipeline-components-manager", "0.1.3", (() => Promise.all([P.e(969), P.e(638), P.e(298)]).then((() => () => P(298))))), l("@headlessui/react", "1.7.18", (() => Promise.all([P.e(649), P.e(638)]).then((() => () => P(649))))), l("react-select", "5.8.0", (() => Promise.all([P.e(969), P.e(638), P.e(2)]).then((() => () => P(2)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                    f = [];
+                return "default" === t && (l("@amphi/pipeline-components-manager", "0.1.6", (() => Promise.all([P.e(143), P.e(379), P.e(345), P.e(628), P.e(893)]).then((() => () => P(893))))), l("antd", "5.16.1", (() => Promise.all([P.e(974), P.e(143), P.e(345), P.e(628)]).then((() => () => P(1974))))), l("react-dnd-html5-backend", "16.0.1", (() => P.e(454).then((() => () => P(6454))))), l("react-dnd", "16.0.1", (() => Promise.all([P.e(12), P.e(345), P.e(85)]).then((() => () => P(4631)))))), e[t] = f.length ? Promise.all(f).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         P.g.importScripts && (e = P.g.location + "");
         var r = P.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
+                for (var a = t.length - 1; a > -1 && (!e || !/^http(s?):/.test(e));) e = t[a--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), P.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            n = t[1] ? r(t[1]) : [];
-        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
-    }, n = (e, r) => {
+            a = t[1] ? r(t[1]) : [];
+        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
+    }, a = (e, r) => {
         e = t(e), r = t(r);
-        for (var n = 0;;) {
-            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
-            var a = e[n],
-                o = (typeof a)[0];
-            if (n >= r.length) return "u" == o;
-            var i = r[n],
+        for (var a = 0;;) {
+            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
+            var n = e[a],
+                o = (typeof n)[0];
+            if (a >= r.length) return "u" == o;
+            var i = r[a],
                 l = (typeof i)[0];
             if (o != l) return "o" == o && "n" == l || "s" == l || "u" == o;
-            if ("o" != o && "u" != o && a != i) return a < i;
-            n++
+            if ("o" != o && "u" != o && n != i) return n < i;
+            a++
         }
-    }, a = e => {
+    }, n = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
+            for (var a = 1, o = 1; o < e.length; o++) a--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
             return t
         }
         var i = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            i.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? i.pop() + " " + i.pop() : a(l))
+            i.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? i.pop() + " " + i.pop() : n(l))
         }
-        return u();
+        return f();
 
-        function u() {
+        function f() {
             return i.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var n = e[0],
-                a = n < 0;
-            a && (n = -n - 1);
-            for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(f = r[i]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
-                if ("u" == s) {
-                    if (!u || "u" != d) return !1
-                } else if (u)
-                    if (d == s)
-                        if (l <= n) {
-                            if (f != e[l]) return !1
+            var a = e[0],
+                n = a < 0;
+            n && (a = -a - 1);
+            for (var i = 0, l = 1, f = !0;; l++, i++) {
+                var u, d, c = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (d = (typeof(u = r[i]))[0])) return !f || ("u" == c ? l > a && !n : "" == c != n);
+                if ("u" == d) {
+                    if (!f || "u" != c) return !1
+                } else if (f)
+                    if (c == d)
+                        if (l <= a) {
+                            if (u != e[l]) return !1
                         } else {
-                            if (a ? f > e[l] : f < e[l]) return !1;
-                            f != e[l] && (u = !1)
+                            if (n ? u > e[l] : u < e[l]) return !1;
+                            u != e[l] && (f = !1)
                         }
-                else if ("s" != d && "n" != d) {
-                    if (a || l <= n) return !1;
-                    u = !1, l--
+                else if ("s" != c && "n" != c) {
+                    if (n || l <= a) return !1;
+                    f = !1, l--
                 } else {
-                    if (l <= n || s < d != a) return !1;
-                    u = !1
-                } else "s" != d && "n" != d && (u = !1, l--)
+                    if (l <= a || d < c != n) return !1;
+                    f = !1
+                } else "s" != c && "n" != c && (f = !1, l--)
             }
         }
-        var p = [],
-            c = p.pop.bind(p);
+        var s = [],
+            p = s.pop.bind(s);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
-            p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
+            s.push(1 == h ? p() | p() : 2 == h ? p() & p() : h ? o(h, r) : !p())
         }
-        return !!c()
+        return !!p()
     }, i = (e, r) => {
         var t = P.S[e];
         if (!t || !P.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", f = (e, r, t, n) => {
-        var a = l(e, t);
-        return o(n, a) || d(u(e, t, a, n)), p(e[t][a])
-    }, s = (e, r, t) => {
-        var a = e[r];
-        return (r = Object.keys(a).reduce(((e, r) => !o(t, r) || e && !n(e, r) ? e : r), 0)) && a[r]
-    }, d = e => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
+    }, f = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", u = (e, r, t, a) => {
+        var n = l(e, t);
+        return o(a, n) || c(f(e, t, n, a)), s(e[t][n])
+    }, d = (e, r, t) => {
+        var n = e[r];
+        return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
+    }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, p = e => (e.loaded = 1, e.get()), h = (c = e => function(r, t, n, a) {
+    }, s = e => (e.loaded = 1, e.get()), h = (p = e => function(r, t, a, n) {
         var o = P.I(r);
-        return o && o.then ? o.then(e.bind(e, r, P.S[r], t, n, a)) : e(r, P.S[r], t, n, a)
-    })(((e, r, t, n) => (i(e, t), f(r, 0, t, n)))), m = c(((e, r, t, n, a) => {
-        var o = r && P.o(r, t) && s(r, t, n);
-        return o ? p(o) : a()
-    })), v = {}, b = {
-        345: () => h("default", "react", [1, 18, 2, 0]),
-        628: () => h("default", "react-dom", [1, 18, 2, 0]),
-        98: () => m("default", "@headlessui/react", [1, 1, 7, 18], (() => P.e(649).then((() => () => P(649))))),
-        153: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        228: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
-        243: () => m("default", "react-select", [1, 5, 8, 0], (() => P.e(621).then((() => () => P(2))))),
-        256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
-        262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        700: () => h("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
-        707: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 5])
+        return o && o.then ? o.then(e.bind(e, r, P.S[r], t, a, n)) : e(r, P.S[r], t, a, n)
+    })(((e, r, t, a) => (i(e, t), u(r, 0, t, a)))), m = p(((e, r, t, a, n) => {
+        var o = r && P.o(r, t) && d(r, t, a);
+        return o ? s(o) : n()
+    })), b = {}, v = {
+        3345: () => h("default", "react", [1, 18, 2, 0]),
+        7628: () => h("default", "react-dom", [1, 18, 2, 0]),
+        1029: () => m("default", "react-dnd-html5-backend", [1, 16, 0, 1], (() => P.e(454).then((() => () => P(6454))))),
+        2283: () => m("default", "antd", [1, 5, 16, 0], (() => P.e(974).then((() => () => P(1974))))),
+        5256: () => h("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
+        5709: () => m("default", "react-dnd", [1, 16, 0, 1], (() => P.e(12).then((() => () => P(4631))))),
+        6597: () => h("default", "@jupyterlab/coreutils", [1, 6, 1, 6]),
+        7262: () => h("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        7638: () => h("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        7664: () => h("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        9221: () => h("default", "@jupyterlab/filebrowser", [1, 4, 1, 6])
     }, g = {
-        298: [98, 153, 228, 243, 256, 262, 700, 707],
-        638: [345, 628]
+        345: [3345],
+        628: [7628],
+        893: [1029, 2283, 5256, 5709, 6597, 7262, 7638, 7664, 9221]
     }, y = {}, P.f.consumes = (e, r) => {
         P.o(g, e) && g[e].forEach((e => {
-            if (P.o(v, e)) return r.push(v[e]);
+            if (P.o(b, e)) return r.push(b[e]);
             if (!y[e]) {
                 var t = r => {
-                    v[e] = 0, P.m[e] = t => {
+                    b[e] = 0, P.m[e] = t => {
                         delete P.c[e], t.exports = r()
                     }
                 };
                 y[e] = !0;
-                var n = r => {
-                    delete v[e], P.m[e] = t => {
+                var a = r => {
+                    delete b[e], P.m[e] = t => {
                         throw delete P.c[e], r
                     }
                 };
                 try {
-                    var a = b[e]();
-                    a.then ? r.push(v[e] = a.then(t).catch(n)) : t(a)
+                    var n = v[e]();
+                    n.then ? r.push(b[e] = n.then(t).catch(a)) : t(n)
                 } catch (e) {
-                    n(e)
+                    a(e)
                 }
             }
         }))
     }, (() => {
         var e = {
             508: 0
         };
         P.f.j = (r, t) => {
-            var n = P.o(e, r) ? e[r] : void 0;
-            if (0 !== n)
-                if (n) t.push(n[2]);
-                else if (638 != r) {
-                var a = new Promise(((t, a) => n = e[r] = [t, a]));
-                t.push(n[2] = a);
+            var a = P.o(e, r) ? e[r] : void 0;
+            if (0 !== a)
+                if (a) t.push(a[2]);
+                else if (/^(345|628)$/.test(r)) e[r] = 0;
+            else {
+                var n = new Promise(((t, n) => a = e[r] = [t, n]));
+                t.push(a[2] = n);
                 var o = P.p + P.u(r),
                     i = new Error;
                 P.l(o, (t => {
-                    if (P.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var a = t && ("load" === t.type ? "missing" : t.type),
+                    if (P.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
+                        var n = t && ("load" === t.type ? "missing" : t.type),
                             o = t && t.target && t.target.src;
-                        i.message = "Loading chunk " + r + " failed.\n(" + a + ": " + o + ")", i.name = "ChunkLoadError", i.type = a, i.request = o, n[1](i)
+                        i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
-            } else e[r] = 0
+            }
         };
         var r = (r, t) => {
-                var n, a, [o, i, l] = t,
-                    u = 0;
+                var a, n, [o, i, l] = t,
+                    f = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in i) P.o(i, n) && (P.m[n] = i[n]);
+                    for (a in i) P.o(i, a) && (P.m[a] = i[a]);
                     l && l(P)
                 }
-                for (r && r(t); u < o.length; u++) a = o[u], P.o(e, a) && e[a] && e[a][0](), e[a] = 0
+                for (r && r(t); f < o.length; f++) n = o[f], P.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amphi_pipeline_components_manager = self.webpackChunk_amphi_pipeline_components_manager || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), P.nc = void 0;
-    var E = P(548);
+    var E = P(5548);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-components-manager"] = E
 })();
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-components-manager/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/third-party-licenses.json`

 * *Files 22% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7115384615384616%*

 * *Differences: {"'packages'": "{0: {'name': '@ant-design/colors', 'versionInfo': '7.0.2', 'extractedText': 'MIT "*

 * *               'LICENSE\\n\\nCopyright (c) 2018-present Ant UED, '*

 * *               'https://xtech.antfin.com/\\n\\nPermission is hereby granted, free of charge, to '*

 * *               'any person obtaining\\na copy of this software and associated documentation files '*

 * *               '(the\\n"Software"), to deal in the Software without restriction, '*

 * *               'including\\nwithout limitation the rights to use, […]*

```diff
@@ -1,148 +1,238 @@
 {
     "packages": [
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2014-present Sebastian McKenzie and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "extractedText": "MIT LICENSE\n\nCopyright (c) 2018-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@babel/runtime",
-            "versionInfo": "7.24.1"
+            "name": "@ant-design/colors",
+            "versionInfo": "7.0.2"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/cache",
-            "versionInfo": "11.11.0"
+            "name": "@ant-design/cssinjs",
+            "versionInfo": "1.19.1"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "MIT LICENSE\n\nCopyright (c) 2018-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/hash",
-            "versionInfo": "0.9.1"
+            "name": "@ant-design/icons",
+            "versionInfo": "5.3.6"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "",
             "licenseId": "MIT",
-            "name": "@emotion/memoize",
-            "versionInfo": "0.8.1"
+            "name": "@ant-design/icons-svg",
+            "versionInfo": "4.4.2"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2014-present Sebastian McKenzie and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/react",
-            "versionInfo": "11.11.4"
+            "name": "@babel/runtime",
+            "versionInfo": "7.24.4"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "Copyright (c) Scott Cooper <scttcper@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/serialize",
-            "versionInfo": "1.1.3"
+            "name": "@ctrl/tinycolor",
+            "versionInfo": "3.6.1"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/sheet",
-            "versionInfo": "1.2.2"
+            "name": "@emotion/hash",
+            "versionInfo": "0.8.0"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "@emotion/unitless",
-            "versionInfo": "0.8.1"
+            "versionInfo": "0.7.5"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/use-insertion-effect-with-fallbacks",
-            "versionInfo": "1.0.1"
+            "name": "@reactflow/background",
+            "versionInfo": "11.3.4"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Emotion team and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@emotion/utils",
-            "versionInfo": "1.2.1"
+            "name": "@reactflow/controls",
+            "versionInfo": "11.2.4"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2021-present Floating UI contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of\nthe Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@floating-ui/dom",
-            "versionInfo": "1.6.3"
+            "name": "@reactflow/core",
+            "versionInfo": "11.9.4"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2021-present Floating UI contributors\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of\nthis software and associated documentation files (the \"Software\"), to deal in\nthe Software without restriction, including without limitation the rights to\nuse, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of\nthe Software, and to permit persons to whom the Software is furnished to do so,\nsubject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS\nFOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR\nCOPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER\nIN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN\nCONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@floating-ui/utils",
-            "versionInfo": "0.2.1"
+            "name": "@reactflow/minimap",
+            "versionInfo": "11.7.4"
         },
         {
-            "extractedText": "",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "@reactflow/node-resizer",
+            "versionInfo": "2.2.4"
+        },
+        {
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "@reactflow/node-toolbar",
+            "versionInfo": "1.3.4"
+        },
+        {
+            "extractedText": "MIT LICENSE\n\nCopyright (c) 2015-present Ant UED, https://xtech.antfin.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@headlessui/react",
-            "versionInfo": "1.7.18"
+            "name": "antd",
+            "versionInfo": "5.16.1"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2021-present Tanner Linsley\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "Copyright \u00a9 Jorge Bucaran <<https://jorgebucaran.com>>\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@tanstack/react-virtual",
-            "versionInfo": "3.2.0"
+            "name": "classcat",
+            "versionInfo": "5.0.5"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2021-present Tanner Linsley\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2018 Jed Watson\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "@tanstack/virtual-core",
-            "versionInfo": "3.2.0"
+            "name": "classnames",
+            "versionInfo": "2.5.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
+        },
+        {
+            "extractedText": "Copyright 2010-2022 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-color",
+            "versionInfo": "3.1.0"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-dispatch",
+            "versionInfo": "3.0.1"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-drag",
+            "versionInfo": "3.0.0"
         },
         {
-            "extractedText": "Software License Agreement (BSD License)\n========================================\n\nCopyright (c) 2015, Yahoo! Inc. All rights reserved.\n----------------------------------------------------\n\nRedistribution and use of this software in source and binary forms, with or\nwithout modification, are permitted provided that the following conditions are\nmet:\n\n  * Redistributions of source code must retain the above copyright notice, this\n    list of conditions and the following disclaimer.\n  * Redistributions in binary form must reproduce the above copyright notice,\n    this list of conditions and the following disclaimer in the documentation\n    and/or other materials provided with the distribution.\n  * Neither the name of Yahoo! Inc. nor the names of YUI's contributors may be\n    used to endorse or promote products derived from this software without\n    specific prior written permission of Yahoo! Inc.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND\nANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED\nWARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR\nANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES\n(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;\nLOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON\nANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT\n(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS\nSOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
+            "extractedText": "Copyright 2010-2021 Mike Bostock\nCopyright 2001 Robert Penner\nAll rights reserved.\n\nRedistribution and use in source and binary forms, with or without modification,\nare permitted provided that the following conditions are met:\n\n* Redistributions of source code must retain the above copyright notice, this\n  list of conditions and the following disclaimer.\n\n* Redistributions in binary form must reproduce the above copyright notice,\n  this list of conditions and the following disclaimer in the documentation\n  and/or other materials provided with the distribution.\n\n* Neither the name of the author nor the names of contributors may be used to\n  endorse or promote products derived from this software without specific prior\n  written permission.\n\nTHIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS \"AS IS\" AND\nANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED\nWARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE\nDISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR\nANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES\n(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;\nLOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON\nANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT\n(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS\nSOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.\n",
             "licenseId": "BSD-3-Clause",
-            "name": "hoist-non-react-statics",
-            "versionInfo": "3.3.2"
+            "name": "d3-ease",
+            "versionInfo": "3.0.1"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) 2019 Alexander Reardon\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.",
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-interpolate",
+            "versionInfo": "3.0.1"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-selection",
+            "versionInfo": "3.0.0"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-timer",
+            "versionInfo": "3.0.1"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-transition",
+            "versionInfo": "3.0.1"
+        },
+        {
+            "extractedText": "Copyright 2010-2021 Mike Bostock\n\nPermission to use, copy, modify, and/or distribute this software for any purpose\nwith or without fee is hereby granted, provided that the above copyright notice\nand this permission notice appear in all copies.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH\nREGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND\nFITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,\nINDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM LOSS\nOF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR OTHER\nTORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF\nTHIS SOFTWARE.\n",
+            "licenseId": "ISC",
+            "name": "d3-zoom",
+            "versionInfo": "3.0.0"
+        },
+        {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "memoize-one",
-            "versionInfo": "6.0.0"
+            "name": "rc-motion",
+            "versionInfo": "2.9.0"
         },
         {
-            "extractedText": "(The MIT License)\n\nCopyright (c) 2013 Roman Shtylman <shtylman@gmail.com>\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2019-present afc163\n\nPermission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the \"Software\"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "process",
-            "versionInfo": "0.11.10"
+            "name": "rc-resize-observer",
+            "versionInfo": "1.4.0"
+        },
+        {
+            "extractedText": "MIT LICENSE\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n\"Software\"), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND\nNONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE\nLIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION\nOF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION\nWITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "rc-tree",
+            "versionInfo": "5.8.5"
+        },
+        {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2014-present yiminghe\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "rc-util",
+            "versionInfo": "5.39.1"
+        },
+        {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2015-present Alipay.com, https://www.alipay.com/\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in\nall copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS \nOR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF \nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. \nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY \nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, \nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE \nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "rc-virtual-list",
+            "versionInfo": "3.11.4"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "react-is",
-            "versionInfo": "16.13.1"
+            "versionInfo": "18.2.0"
         },
         {
-            "extractedText": "",
+            "extractedText": "MIT License\n\nCopyright (c) 2019-2023 webkid GmbH\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "react-select",
-            "versionInfo": "5.8.0"
+            "name": "reactflow",
+            "versionInfo": "11.9.4"
+        },
+        {
+            "extractedText": "The MIT License (MIT)\n\nCopyright (c) 2016 Denis Rul\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "resize-observer-polyfill",
+            "versionInfo": "1.5.1"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         },
         {
             "extractedText": "MIT License\n\nCopyright (c) 2016-present Sultan Tarimo\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
             "name": "stylis",
-            "versionInfo": "4.2.0"
+            "versionInfo": "4.3.1"
+        },
+        {
+            "extractedText": "MIT License\n\nCopyright (c) Facebook, Inc. and its affiliates.\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "licenseId": "MIT",
+            "name": "use-sync-external-store",
+            "versionInfo": "1.2.0"
         },
         {
-            "extractedText": "MIT License\n\nCopyright (c) Mateusz Burzy\u0144ski\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
+            "extractedText": "MIT License\n\nCopyright (c) 2019 Paul Henschel\n\nPermission is hereby granted, free of charge, to any person obtaining a copy\nof this software and associated documentation files (the \"Software\"), to deal\nin the Software without restriction, including without limitation the rights\nto use, copy, modify, merge, publish, distribute, sublicense, and/or sell\ncopies of the Software, and to permit persons to whom the Software is\nfurnished to do so, subject to the following conditions:\n\nThe above copyright notice and this permission notice shall be included in all\ncopies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED \"AS IS\", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR\nIMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,\nFITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE\nAUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER\nLIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,\nOUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE\nSOFTWARE.\n",
             "licenseId": "MIT",
-            "name": "use-isomorphic-layout-effect",
-            "versionInfo": "1.1.2"
+            "name": "zustand",
+            "versionInfo": "4.5.2"
         }
     ]
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-editor/package.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-editor/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9742063492063492%*

 * *Differences: {"'dependencies'": "{delete: ['@headlessui/react']}",*

 * * "'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c3796f919885e692bcd0.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -4,15 +4,14 @@
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
         "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
-        "@headlessui/react": "^1.7.18",
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.1.9",
         "@jupyterlab/docmanager-extension": "^4.1.5",
         "@jupyterlab/filebrowser": "^4.1.5",
         "@jupyterlab/launcher": "^4.1.5",
         "@jupyterlab/logconsole": "^4.1.5",
         "@jupyterlab/mainmenu": "^4.1.5",
@@ -47,15 +46,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.4ac616cbeaf9f2f09472.js",
+            "load": "static/remoteEntry.c3796f919885e692bcd0.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-editor",
         "sharedPackages": {
             "@amphi/pipeline-components-manager": {
                 "bundled": false,
@@ -103,9 +102,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.6"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,13 @@
-/*! For license information please see 285.4eef7e98cbfad514e073.js.LICENSE.txt */
+/*! For license information please see 285.f1fef15430d9554bfba0.js.LICENSE.txt */
 "use strict";
 (self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || []).push([
     [285], {
-        26: (e, t, n) => {
-            var o = n(345),
+        4026: (e, t, n) => {
+            var o = n(3345),
                 r = "function" == typeof Object.is ? Object.is : function(e, t) {
                     return e === t && (0 !== e || 1 / e == 1 / t) || e != e && t != t
                 },
                 i = o.useState,
                 a = o.useEffect,
                 s = o.useLayoutEffect,
                 l = o.useDebugValue;
@@ -46,17 +46,17 @@
                             inst: r
                         })
                     }))
                 }), [e]), l(n), n
             };
             t.useSyncExternalStore = void 0 !== o.useSyncExternalStore ? o.useSyncExternalStore : u
         },
-        965: (e, t, n) => {
-            var o = n(345),
-                r = n(139),
+        4965: (e, t, n) => {
+            var o = n(3345),
+                r = n(8139),
                 i = "function" == typeof Object.is ? Object.is : function(e, t) {
                     return e === t && (0 !== e || 1 / e == 1 / t) || e != e && t != t
                 },
                 a = r.useSyncExternalStore,
                 s = o.useRef,
                 l = o.useEffect,
                 c = o.useMemo,
@@ -93,21 +93,21 @@
                 }), [t, n, o, r]);
                 var f = a(e, d[0], d[1]);
                 return l((function() {
                     h.hasValue = !0, h.value = f
                 }), [f]), u(f), f
             }
         },
-        139: (e, t, n) => {
-            e.exports = n(26)
+        8139: (e, t, n) => {
+            e.exports = n(4026)
         },
-        121: (e, t, n) => {
-            e.exports = n(965)
+        7121: (e, t, n) => {
+            e.exports = n(4965)
         },
-        285: (e, t, n) => {
+        1285: (e, t, n) => {
             n.r(t), n.d(t, {
                 Background: () => Xs,
                 BackgroundVariant: () => Rs,
                 BaseEdge: () => Ho,
                 BezierEdge: () => ur,
                 ConnectionLineType: () => Uo,
                 ConnectionMode: () => Wo,
@@ -168,27 +168,27 @@
                 useOnViewportChange: () => hs,
                 useReactFlow: () => Mi,
                 useStore: () => ho,
                 useStoreApi: () => fo,
                 useUpdateNodeInternals: () => ns,
                 useViewport: () => ls
             });
-            var o = n(345),
+            var o = n(3345),
                 r = n.n(o);
 
             function i(e) {
                 if ("string" == typeof e || "number" == typeof e) return "" + e;
                 let t = "";
                 if (Array.isArray(e))
                     for (let n, o = 0; o < e.length; o++) "" !== (n = i(e[o])) && (t += (t && " ") + n);
                 else
                     for (let n in e) e[n] && (t += (t && " ") + n);
                 return t
             }
-            var a = n(121);
+            var a = n(7121);
             const s = e => {
                     let t;
                     const n = new Set,
                         o = (e, o) => {
                             const r = "function" == typeof e ? e(t) : e;
                             if (!Object.is(r, t)) {
                                 const e = t;
@@ -2704,15 +2704,15 @@
                     return arguments.length ? (d = (e = +e) * e, h) : Math.sqrt(d)
                 }, h
             }
             eo.prototype.on = function() {
                 var e = this._.on.apply(this._, arguments);
                 return e === this._ ? this : e
             };
-            var ao = n(628);
+            var ao = n(7628);
             const so = (0, o.createContext)(null),
                 lo = so.Provider,
                 co = {
                     error001: () => "[React Flow]: Seems like you have not used zustand provider as an ancestor. Help: https://reactflow.dev/error#001",
                     error002: () => "It looks like you've created a new nodeTypes or edgeTypes object. If this wasn't on purpose please define the nodeTypes/edgeTypes outside of the component or memoize them.",
                     error003: e => `Node type "${e}" not found. Using fallback type "default".`,
                     error004: () => "The React Flow parent container needs a width and a height to render the graph.",
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/285.4eef7e98cbfad514e073.js.LICENSE.txt` & `jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/285.f1fef15430d9554bfba0.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-editor/static/remoteEntry.4ac616cbeaf9f2f09472.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-editor/static/remoteEntry.c3796f919885e692bcd0.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,16 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, o, i, l, u, d, s, f, p, c, h, v, b, m, g, y, w, j, P, S, E = {
-            535: (e, r, t) => {
+    var e, r, t, a, n, o, i, l, u, d, f, s, p, c, h, v, m, b, g, y, w, j, S, P, E = {
+            8535: (e, r, t) => {
                 var a = {
-                        "./index": () => Promise.all([t.e(550), t.e(345), t.e(378)]).then((() => () => t(378))),
-                        "./extension": () => Promise.all([t.e(550), t.e(345), t.e(378)]).then((() => () => t(378))),
-                        "./style": () => Promise.all([t.e(550), t.e(631)]).then((() => () => t(631)))
+                        "./index": () => Promise.all([t.e(756), t.e(550), t.e(638), t.e(219)]).then((() => () => t(3219))),
+                        "./extension": () => Promise.all([t.e(756), t.e(550), t.e(638), t.e(219)]).then((() => () => t(3219))),
+                        "./style": () => Promise.all([t.e(550), t.e(121)]).then((() => () => t(7631)))
                     },
                     n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var a = "default",
@@ -43,57 +43,57 @@
         }), r
     }, _.d = (e, r) => {
         for (var t in r) _.o(r, t) && !_.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, _.f = {}, _.e = e => Promise.all(Object.keys(_.f).reduce(((r, t) => (_.f[t](e, r), r)), [])), _.u = e => e + "." + {
-        285: "4eef7e98cbfad514e073",
-        345: "6caf4262497eb1d0b5d6",
-        378: "8d63007918eb0fb399f9",
-        550: "fc24af3aaabe117c3a69",
-        628: "4378428a320303a7edb2",
-        631: "2e42de0a30aaca0133f5"
+        121: "8c540e5dd43820941920",
+        219: "660cd7be25b20ac30f25",
+        285: "f1fef15430d9554bfba0",
+        550: "7ad263262b92cbc9bbee",
+        638: "28f4ea302090a6e9a404",
+        756: "cbe8df68f480d40f4c7e"
     } [e] + ".js?v=" + {
-        285: "4eef7e98cbfad514e073",
-        345: "6caf4262497eb1d0b5d6",
-        378: "8d63007918eb0fb399f9",
-        550: "fc24af3aaabe117c3a69",
-        628: "4378428a320303a7edb2",
-        631: "2e42de0a30aaca0133f5"
+        121: "8c540e5dd43820941920",
+        219: "660cd7be25b20ac30f25",
+        285: "f1fef15430d9554bfba0",
+        550: "7ad263262b92cbc9bbee",
+        638: "28f4ea302090a6e9a404",
+        756: "cbe8df68f480d40f4c7e"
     } [e], _.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), _.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-editor:", _.l = (t, a, n, o) => {
         if (e[t]) e[t].push(a);
         else {
             var i, l;
             if (void 0 !== n)
                 for (var u = document.getElementsByTagName("script"), d = 0; d < u.length; d++) {
-                    var s = u[d];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + n) {
-                        i = s;
+                    var f = u[d];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + n) {
+                        i = f;
                         break
                     }
                 }
             i || (l = !0, (i = document.createElement("script")).charset = "utf-8", i.timeout = 120, _.nc && i.setAttribute("nonce", _.nc), i.setAttribute("data-webpack", r + n), i.src = t), e[t] = [a];
-            var f = (r, a) => {
+            var s = (r, a) => {
                     i.onerror = i.onload = null, clearTimeout(p);
                     var n = e[t];
                     if (delete e[t], i.parentNode && i.parentNode.removeChild(i), n && n.forEach((e => e(a))), r) return r(a)
                 },
-                p = setTimeout(f.bind(null, void 0, {
+                p = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: i
                 }), 12e4);
-            i.onerror = f.bind(null, i.onerror), i.onload = f.bind(null, i.onload), l && document.head.appendChild(i)
+            i.onerror = s.bind(null, i.onerror), i.onload = s.bind(null, i.onload), l && document.head.appendChild(i)
         }
     }, _.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -115,15 +115,15 @@
                         (!l || !l.loaded && (!a != !l.eager ? a : i > l.from)) && (n[r] = {
                             get: t,
                             from: i,
                             eager: !!a
                         })
                     },
                     u = [];
-                return "default" === t && (l("@amphi/pipeline-editor", "0.1.3", (() => Promise.all([_.e(550), _.e(345), _.e(378)]).then((() => () => _(378))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(345), _.e(628)]).then((() => () => _(285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
+                return "default" === t && (l("@amphi/pipeline-editor", "0.1.6", (() => Promise.all([_.e(756), _.e(550), _.e(638), _.e(219)]).then((() => () => _(3219))))), l("reactflow", "11.9.4", (() => Promise.all([_.e(285), _.e(638)]).then((() => () => _(1285)))))), e[t] = u.length ? Promise.all(u).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         _.g.importScripts && (e = _.g.location + "");
         var r = _.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -173,33 +173,33 @@
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var a = e[0],
                 n = a < 0;
             n && (a = -a - 1);
             for (var i = 0, l = 1, u = !0;; l++, i++) {
-                var d, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (i >= r.length || "o" == (s = (typeof(d = r[i]))[0])) return !u || ("u" == f ? l > a && !n : "" == f != n);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
+                var d, f, s = l < e.length ? (typeof e[l])[0] : "";
+                if (i >= r.length || "o" == (f = (typeof(d = r[i]))[0])) return !u || ("u" == s ? l > a && !n : "" == s != n);
+                if ("u" == f) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (f == s)
+                    if (s == f)
                         if (l <= a) {
                             if (d != e[l]) return !1
                         } else {
                             if (n ? d > e[l] : d < e[l]) return !1;
                             d != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (n || l <= a) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || s < f != n) return !1;
+                    if (l <= a || f < s != n) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (i = 1; i < e.length; i++) {
             var h = e[i];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
@@ -211,64 +211,62 @@
         return t
     }, l = (e, r) => {
         var t = e[r];
         return (r = Object.keys(t).reduce(((e, r) => !e || a(e, r) ? r : e), 0)) && t[r]
     }, u = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", s = (e, r, t, a) => {
+    }, d = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", f = (e, r, t, a) => {
         var n = u(e, t);
         return o(a, n) || c(d(e, t, n, a)), v(e[t][n])
-    }, f = (e, r, t) => {
+    }, s = (e, r, t) => {
         var n = e[r];
         return (r = Object.keys(n).reduce(((e, r) => !o(t, r) || e && !a(e, r) ? e : r), 0)) && n[r]
     }, p = (e, r, t, a) => {
         var o = e[t];
         return "No satisfying version (" + n(a) + ") of shared module " + t + " found in shared scope " + r + ".\nAvailable versions: " + Object.keys(o).map((e => e + " from " + o[e].from)).join(", ")
     }, c = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, h = (e, r, t, a) => {
         c(p(e, r, t, a))
-    }, v = e => (e.loaded = 1, e.get()), m = (b = e => function(r, t, a, n) {
+    }, v = e => (e.loaded = 1, e.get()), b = (m = e => function(r, t, a, n) {
         var o = _.I(r);
         return o && o.then ? o.then(e.bind(e, r, _.S[r], t, a, n)) : e(r, _.S[r], t, a, n)
-    })(((e, r, t, a) => (i(e, t), v(f(r, t, a) || h(r, e, t, a) || l(r, t))))), g = b(((e, r, t, a) => (i(e, t), s(r, 0, t, a)))), y = b(((e, r, t, a, n) => {
-        var o = r && _.o(r, t) && f(r, t, a);
+    })(((e, r, t, a) => (i(e, t), v(s(r, t, a) || h(r, e, t, a) || l(r, t))))), g = m(((e, r, t, a) => (i(e, t), f(r, 0, t, a)))), y = m(((e, r, t, a, n) => {
+        var o = r && _.o(r, t) && s(r, t, a);
         return o ? v(o) : n()
     })), w = {}, j = {
-        345: () => g("default", "react", [1, 18, 2, 0]),
-        102: () => g("default", "@jupyterlab/launcher", [1, 4, 1, 5]),
-        107: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 5]),
-        153: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
-        208: () => m("default", "@jupyterlab/docregistry", [1, 4, 1, 5]),
-        228: () => g("default", "@jupyterlab/coreutils", [1, 6, 1, 5]),
-        254: () => g("default", "@amphi/pipeline-components-manager", [0]),
-        262: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        406: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
-        613: () => y("default", "reactflow", [4, 11, 9, 4], (() => Promise.all([_.e(285), _.e(628)]).then((() => () => _(285))))),
-        700: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 5]),
-        707: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        743: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 5]),
-        852: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 5]),
-        976: () => g("default", "@jupyterlab/application", [1, 4, 1, 5]),
-        628: () => g("default", "react-dom", [1, 18, 2, 0])
-    }, P = {
-        345: [345],
-        378: [102, 107, 153, 208, 228, 254, 262, 406, 613, 700, 707, 743, 852, 976],
-        628: [628]
-    }, S = {}, _.f.consumes = (e, r) => {
-        _.o(P, e) && P[e].forEach((e => {
+        3345: () => g("default", "react", [1, 18, 2, 0]),
+        7628: () => g("default", "react-dom", [1, 18, 2, 0]),
+        723: () => g("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        1381: () => g("default", "@jupyterlab/mainmenu", [1, 4, 1, 6]),
+        1595: () => g("default", "@jupyterlab/launcher", [1, 4, 1, 6]),
+        3254: () => g("default", "@amphi/pipeline-components-manager", [0]),
+        3613: () => y("default", "reactflow", [4, 11, 9, 4], (() => _.e(285).then((() => () => _(1285))))),
+        5465: () => g("default", "@jupyterlab/application", [1, 4, 1, 6]),
+        7262: () => g("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        7638: () => g("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        7664: () => g("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        8014: () => g("default", "@jupyterlab/statusbar", [1, 4, 1, 6]),
+        8859: () => b("default", "@jupyterlab/docregistry", [1, 4, 1, 6]),
+        9221: () => g("default", "@jupyterlab/filebrowser", [1, 4, 1, 6]),
+        9618: () => g("default", "@jupyterlab/settingregistry", [1, 4, 1, 6])
+    }, S = {
+        219: [723, 1381, 1595, 3254, 3613, 5465, 7262, 7638, 7664, 8014, 8859, 9221, 9618],
+        638: [3345, 7628]
+    }, P = {}, _.f.consumes = (e, r) => {
+        _.o(S, e) && S[e].forEach((e => {
             if (_.o(w, e)) return r.push(w[e]);
-            if (!S[e]) {
+            if (!P[e]) {
                 var t = r => {
                     w[e] = 0, _.m[e] = t => {
                         delete _.c[e], t.exports = r()
                     }
                 };
-                S[e] = !0;
+                P[e] = !0;
                 var a = r => {
                     delete w[e], _.m[e] = t => {
                         throw delete _.c[e], r
                     }
                 };
                 try {
                     var n = j[e]();
@@ -282,37 +280,36 @@
         var e = {
             685: 0
         };
         _.f.j = (r, t) => {
             var a = _.o(e, r) ? e[r] : void 0;
             if (0 !== a)
                 if (a) t.push(a[2]);
-                else if (/^(345|628)$/.test(r)) e[r] = 0;
-            else {
+                else if (638 != r) {
                 var n = new Promise(((t, n) => a = e[r] = [t, n]));
                 t.push(a[2] = n);
                 var o = _.p + _.u(r),
                     i = new Error;
                 _.l(o, (t => {
                     if (_.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
                         var n = t && ("load" === t.type ? "missing" : t.type),
                             o = t && t.target && t.target.src;
                         i.message = "Loading chunk " + r + " failed.\n(" + n + ": " + o + ")", i.name = "ChunkLoadError", i.type = n, i.request = o, a[1](i)
                     }
                 }), "chunk-" + r, r)
-            }
+            } else e[r] = 0
         };
         var r = (r, t) => {
                 var a, n, [o, i, l] = t,
                     u = 0;
                 if (o.some((r => 0 !== e[r]))) {
                     for (a in i) _.o(i, a) && (_.m[a] = i[a]);
                     l && l(_)
                 }
                 for (r && r(t); u < o.length; u++) n = o[u], _.o(e, n) && e[n] && e[n][0](), e[n] = 0
             },
             t = self.webpackChunk_amphi_pipeline_editor = self.webpackChunk_amphi_pipeline_editor || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), _.nc = void 0;
-    var T = _(535);
+    var T = _(8535);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-editor"] = T
 })();
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/package.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9756944444444444%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.a3e4311f433709c80b81.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.957754cc111445ec7cb1.js",
+            "load": "static/remoteEntry.a3e4311f433709c80b81.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-log-console",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -98,9 +98,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.6"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/432.34312e1a7db2f3637c41.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/432.34312e1a7db2f3637c41.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/534.b949d24467a749a658b1.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/534.8692c2c01fee4d696319.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,18 +1,18 @@
 "use strict";
 (self.webpackChunk_amphi_pipeline_log_console = self.webpackChunk_amphi_pipeline_log_console || []).push([
     [534], {
         534: (e, t, s) => {
             s.r(t), s.d(t, {
                 default: () => k
             });
-            var n = s(707),
-                o = s(976),
-                i = s(406),
-                a = s(153),
+            var n = s(638),
+                o = s(465),
+                i = s(723),
+                a = s(664),
                 r = s(881),
                 l = s(602);
             class c {
                 constructor(e) {
                     this._isDisposed = !1, this._disposed = new l.Signal(this), this._rendermime = null, this._connector = e
                 }
                 get disposed() {
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/remoteEntry.957754cc111445ec7cb1.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/remoteEntry.a3e4311f433709c80b81.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, o, i, a, l, u, p, s, f, d, c, h, v, g, m = {
+    var e, r, t, n, o, i, a, l, u, f, p, s, d, c, h, v, g, m = {
             383: (e, r, t) => {
                 var n = {
                         "./index": () => t.e(534).then((() => () => t(534))),
                         "./extension": () => t.e(534).then((() => () => t(534))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
                     o = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
@@ -44,48 +44,48 @@
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         432: "34312e1a7db2f3637c41",
-        534: "b949d24467a749a658b1"
+        534: "8692c2c01fee4d696319"
     } [e] + ".js?v=" + {
         432: "34312e1a7db2f3637c41",
-        534: "b949d24467a749a658b1"
+        534: "8692c2c01fee4d696319"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-log-console:", y.l = (t, n, o, i) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== o)
-                for (var u = document.getElementsByTagName("script"), p = 0; p < u.length; p++) {
-                    var s = u[p];
-                    if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + o) {
-                        a = s;
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var p = u[f];
+                    if (p.getAttribute("src") == t || p.getAttribute("data-webpack") == r + o) {
+                        a = p;
                         break
                     }
                 }
             a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, y.nc && a.setAttribute("nonce", y.nc), a.setAttribute("data-webpack", r + o), a.src = t), e[t] = [n];
-            var f = (r, n) => {
+            var s = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(d);
                     var o = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), o && o.forEach((e => e(n))), r) return r(n)
                 },
-                d = setTimeout(f.bind(null, void 0, {
+                d = setTimeout(s.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
-            a.onerror = f.bind(null, a.onerror), a.onload = f.bind(null, a.onload), l && document.head.appendChild(a)
+            a.onerror = s.bind(null, a.onerror), a.onload = s.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
@@ -106,15 +106,15 @@
                     var o = i[e] = i[e] || {},
                         l = o[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (o[r] = {
                         get: () => y.e(534).then((() => () => y(534))),
                         from: a,
                         eager: !1
                     })
-                })("@amphi/pipeline-log-console", "0.1.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-log-console", "0.1.6"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
@@ -164,33 +164,33 @@
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 o = n < 0;
             o && (n = -n - 1);
             for (var a = 0, l = 1, u = !0;; l++, a++) {
-                var p, s, f = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(p = r[a]))[0])) return !u || ("u" == f ? l > n && !o : "" == f != o);
-                if ("u" == s) {
-                    if (!u || "u" != f) return !1
+                var f, p, s = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (p = (typeof(f = r[a]))[0])) return !u || ("u" == s ? l > n && !o : "" == s != o);
+                if ("u" == p) {
+                    if (!u || "u" != s) return !1
                 } else if (u)
-                    if (f == s)
+                    if (s == p)
                         if (l <= n) {
-                            if (p != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (o ? p > e[l] : p < e[l]) return !1;
-                            p != e[l] && (u = !1)
+                            if (o ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
+                else if ("s" != s && "n" != s) {
                     if (o || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= n || s < f != o) return !1;
+                    if (l <= n || p < s != o) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != s && "n" != s && (u = !1, l--)
             }
         }
         var d = [],
             c = d.pop.bind(d);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             d.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
@@ -199,33 +199,33 @@
     }, a = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", p = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + o(n) + ")", f = (e, r, t, n) => {
         var o = l(e, t);
-        return i(n, o) || s(u(e, t, o, n)), f(e[t][o])
-    }, s = e => {
+        return i(n, o) || p(u(e, t, o, n)), s(e[t][o])
+    }, p = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
+    }, s = e => (e.loaded = 1, e.get()), d = (e => function(r, t, n, o) {
         var i = y.I(r);
         return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, o)) : e(r, y.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), p(r, 0, t, n)))), c = {}, h = {
-        153: () => d("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
+    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), c = {}, h = {
         256: () => d("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         262: () => d("default", "@lumino/coreutils", [1, 2, 0, 0]),
-        406: () => d("default", "@jupyterlab/rendermime", [1, 4, 1, 5]),
+        465: () => d("default", "@jupyterlab/application", [1, 4, 1, 6]),
         602: () => d("default", "@lumino/signaling", [1, 2, 0, 0]),
-        707: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        881: () => d("default", "@amphi/pipeline-editor", [0]),
-        976: () => d("default", "@jupyterlab/application", [1, 4, 1, 5])
+        638: () => d("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        664: () => d("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        723: () => d("default", "@jupyterlab/rendermime", [1, 4, 1, 6]),
+        881: () => d("default", "@amphi/pipeline-editor", [0])
     }, v = {
-        534: [153, 256, 262, 406, 602, 707, 881, 976]
+        534: [256, 262, 465, 602, 638, 664, 723, 881]
     }, g = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
             if (y.o(c, e)) return r.push(c[e]);
             if (!g[e]) {
                 var t = r => {
                     c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-log-console/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-log-console/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.11.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/package.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9744791666666666%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.c4969e0c2f708b845d0d.js'}}",*

 * * "'version'": "'0.1.6'"}*

```diff
@@ -51,15 +51,15 @@
         "style/*.css",
         "style/index.js"
     ],
     "homepage": "https://github.com/amphi-ai/jupyterlab-amphi",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.1751f4c48e4c86d64c78.js",
+            "load": "static/remoteEntry.c4969e0c2f708b845d0d.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "../../amphi/pipeline-metadata-panel",
         "sharedPackages": {
             "@amphi/pipeline-editor": {
                 "bundled": false,
@@ -95,9 +95,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.3"
+    "version": "0.1.6"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/432.85c783ba5ff02c0acd68.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/432.85c783ba5ff02c0acd68.js`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/732.b7777d3d4826271f6ab3.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/732.cb2b06b77f00d8ec6e69.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -2,18 +2,18 @@
 (self.webpackChunk_amphi_pipeline_metadata_panel = self.webpackChunk_amphi_pipeline_metadata_panel || []).push([
     [732], {
         732: (e, t, n) => {
             n.r(t), n.d(t, {
                 VariableInspectionHandler: () => p,
                 default: () => v
             });
-            var a = n(707),
-                s = n(976),
-                i = n(965),
-                r = n(153),
+            var a = n(638),
+                s = n(465),
+                i = n(44),
+                r = n(664),
                 o = n(881),
                 _ = n(602),
                 d = n(88);
             class l {
                 constructor(e) {
                     this._isDisposed = !1, this._disposed = new _.Signal(this), this._inspected = new _.Signal(this), this._rendermime = null, this._connector = e
                 }
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/remoteEntry.1751f4c48e4c86d64c78.js` & `jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/remoteEntry.c4969e0c2f708b845d0d.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -1,285 +1,285 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, a, n, i, o, l, u, p, d, f, s, h, c, v, m, b = {
+    var e, r, t, n, a, i, o, l, u, p, f, d, s, c, h, v, m, g = {
             320: (e, r, t) => {
-                var a = {
+                var n = {
                         "./index": () => t.e(732).then((() => () => t(732))),
                         "./extension": () => t.e(732).then((() => () => t(732))),
                         "./style": () => t.e(432).then((() => () => t(432)))
                     },
-                    n = (e, r) => (t.R = r, r = t.o(a, e) ? a[e]() : Promise.resolve().then((() => {
+                    a = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     i = (e, r) => {
                         if (t.S) {
-                            var a = "default",
-                                n = t.S[a];
-                            if (n && n !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
-                            return t.S[a] = e, t.I(a, r)
+                            var n = "default",
+                                a = t.S[n];
+                            if (a && a !== e) throw new Error("Container initialization failed as it has already been initialized with a different share scope");
+                            return t.S[n] = e, t.I(n, r)
                         }
                     };
                 t.d(r, {
-                    get: () => n,
+                    get: () => a,
                     init: () => i
                 })
             }
         },
-        g = {};
+        b = {};
 
     function y(e) {
-        var r = g[e];
+        var r = b[e];
         if (void 0 !== r) return r.exports;
-        var t = g[e] = {
+        var t = b[e] = {
             id: e,
             exports: {}
         };
-        return b[e](t, t.exports, y), t.exports
+        return g[e](t, t.exports, y), t.exports
     }
-    y.m = b, y.c = g, y.n = e => {
+    y.m = g, y.c = b, y.n = e => {
         var r = e && e.__esModule ? () => e.default : () => e;
         return y.d(r, {
             a: r
         }), r
     }, y.d = (e, r) => {
         for (var t in r) y.o(r, t) && !y.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
     }, y.f = {}, y.e = e => Promise.all(Object.keys(y.f).reduce(((r, t) => (y.f[t](e, r), r)), [])), y.u = e => e + "." + {
         432: "85c783ba5ff02c0acd68",
-        732: "b7777d3d4826271f6ab3"
+        732: "cb2b06b77f00d8ec6e69"
     } [e] + ".js?v=" + {
         432: "85c783ba5ff02c0acd68",
-        732: "b7777d3d4826271f6ab3"
+        732: "cb2b06b77f00d8ec6e69"
     } [e], y.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-metadata-panel:", y.l = (t, a, n, i) => {
-        if (e[t]) e[t].push(a);
+    }(), y.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "@amphi/pipeline-metadata-panel:", y.l = (t, n, a, i) => {
+        if (e[t]) e[t].push(n);
         else {
             var o, l;
-            if (void 0 !== n)
+            if (void 0 !== a)
                 for (var u = document.getElementsByTagName("script"), p = 0; p < u.length; p++) {
-                    var d = u[p];
-                    if (d.getAttribute("src") == t || d.getAttribute("data-webpack") == r + n) {
-                        o = d;
+                    var f = u[p];
+                    if (f.getAttribute("src") == t || f.getAttribute("data-webpack") == r + a) {
+                        o = f;
                         break
                     }
                 }
-            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, y.nc && o.setAttribute("nonce", y.nc), o.setAttribute("data-webpack", r + n), o.src = t), e[t] = [a];
-            var f = (r, a) => {
+            o || (l = !0, (o = document.createElement("script")).charset = "utf-8", o.timeout = 120, y.nc && o.setAttribute("nonce", y.nc), o.setAttribute("data-webpack", r + a), o.src = t), e[t] = [n];
+            var d = (r, n) => {
                     o.onerror = o.onload = null, clearTimeout(s);
-                    var n = e[t];
-                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), n && n.forEach((e => e(a))), r) return r(a)
+                    var a = e[t];
+                    if (delete e[t], o.parentNode && o.parentNode.removeChild(o), a && a.forEach((e => e(n))), r) return r(n)
                 },
-                s = setTimeout(f.bind(null, void 0, {
+                s = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: o
                 }), 12e4);
-            o.onerror = f.bind(null, o.onerror), o.onload = f.bind(null, o.onload), l && document.head.appendChild(o)
+            o.onerror = d.bind(null, o.onerror), o.onload = d.bind(null, o.onload), l && document.head.appendChild(o)
         }
     }, y.r = e => {
         "undefined" != typeof Symbol && Symbol.toStringTag && Object.defineProperty(e, Symbol.toStringTag, {
             value: "Module"
         }), Object.defineProperty(e, "__esModule", {
             value: !0
         })
     }, (() => {
         y.S = {};
         var e = {},
             r = {};
-        y.I = (t, a) => {
-            a || (a = []);
-            var n = r[t];
-            if (n || (n = r[t] = {}), !(a.indexOf(n) >= 0)) {
-                if (a.push(n), e[t]) return e[t];
+        y.I = (t, n) => {
+            n || (n = []);
+            var a = r[t];
+            if (a || (a = r[t] = {}), !(n.indexOf(a) >= 0)) {
+                if (n.push(a), e[t]) return e[t];
                 y.o(y.S, t) || (y.S[t] = {});
                 var i = y.S[t],
                     o = "@amphi/pipeline-metadata-panel",
                     l = [];
-                return "default" === t && ((e, r, t, a) => {
-                    var n = i[e] = i[e] || {},
-                        l = n[r];
-                    (!l || !l.loaded && (1 != !l.eager ? a : o > l.from)) && (n[r] = {
+                return "default" === t && ((e, r, t, n) => {
+                    var a = i[e] = i[e] || {},
+                        l = a[r];
+                    (!l || !l.loaded && (1 != !l.eager ? n : o > l.from)) && (a[r] = {
                         get: () => y.e(732).then((() => () => y(732))),
                         from: o,
                         eager: !1
                     })
-                })("@amphi/pipeline-metadata-panel", "0.1.3"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("@amphi/pipeline-metadata-panel", "0.1.6"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
         y.g.importScripts && (e = y.g.location + "");
         var r = y.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
-                for (var a = t.length - 1; a > -1 && (!e || !/^http(s?):/.test(e));) e = t[a--].src
+                for (var n = t.length - 1; n > -1 && (!e || !/^http(s?):/.test(e));) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
         e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), y.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
-            a = t[1] ? r(t[1]) : [];
-        return t[2] && (a.length++, a.push.apply(a, r(t[2]))), t[3] && (a.push([]), a.push.apply(a, r(t[3]))), a
-    }, a = (e, r) => {
+            n = t[1] ? r(t[1]) : [];
+        return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
+    }, n = (e, r) => {
         e = t(e), r = t(r);
-        for (var a = 0;;) {
-            if (a >= e.length) return a < r.length && "u" != (typeof r[a])[0];
-            var n = e[a],
-                i = (typeof n)[0];
-            if (a >= r.length) return "u" == i;
-            var o = r[a],
+        for (var n = 0;;) {
+            if (n >= e.length) return n < r.length && "u" != (typeof r[n])[0];
+            var a = e[n],
+                i = (typeof a)[0];
+            if (n >= r.length) return "u" == i;
+            var o = r[n],
                 l = (typeof o)[0];
             if (i != l) return "o" == i && "n" == l || "s" == l || "u" == i;
-            if ("o" != i && "u" != i && n != o) return n < o;
-            a++
+            if ("o" != i && "u" != i && a != o) return a < o;
+            n++
         }
-    }, n = e => {
+    }, a = e => {
         var r = e[0],
             t = "";
         if (1 === e.length) return "*";
         if (r + .5) {
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
-            for (var a = 1, i = 1; i < e.length; i++) a--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (a > 0 ? "." : "") + (a = 2, l);
+            for (var n = 1, i = 1; i < e.length; i++) n--, t += "u" == (typeof(l = e[i]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var o = [];
         for (i = 1; i < e.length; i++) {
             var l = e[i];
-            o.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? o.pop() + " " + o.pop() : n(l))
+            o.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? o.pop() + " " + o.pop() : a(l))
         }
         return u();
 
         function u() {
             return o.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, i = (e, r) => {
         if (0 in e) {
             r = t(r);
-            var a = e[0],
-                n = a < 0;
-            n && (a = -a - 1);
+            var n = e[0],
+                a = n < 0;
+            a && (n = -n - 1);
             for (var o = 0, l = 1, u = !0;; l++, o++) {
-                var p, d, f = l < e.length ? (typeof e[l])[0] : "";
-                if (o >= r.length || "o" == (d = (typeof(p = r[o]))[0])) return !u || ("u" == f ? l > a && !n : "" == f != n);
-                if ("u" == d) {
-                    if (!u || "u" != f) return !1
+                var p, f, d = l < e.length ? (typeof e[l])[0] : "";
+                if (o >= r.length || "o" == (f = (typeof(p = r[o]))[0])) return !u || ("u" == d ? l > n && !a : "" == d != a);
+                if ("u" == f) {
+                    if (!u || "u" != d) return !1
                 } else if (u)
-                    if (f == d)
-                        if (l <= a) {
+                    if (d == f)
+                        if (l <= n) {
                             if (p != e[l]) return !1
                         } else {
-                            if (n ? p > e[l] : p < e[l]) return !1;
+                            if (a ? p > e[l] : p < e[l]) return !1;
                             p != e[l] && (u = !1)
                         }
-                else if ("s" != f && "n" != f) {
-                    if (n || l <= a) return !1;
+                else if ("s" != d && "n" != d) {
+                    if (a || l <= n) return !1;
                     u = !1, l--
                 } else {
-                    if (l <= a || d < f != n) return !1;
+                    if (l <= n || f < d != a) return !1;
                     u = !1
-                } else "s" != f && "n" != f && (u = !1, l--)
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var s = [],
-            h = s.pop.bind(s);
+            c = s.pop.bind(s);
         for (o = 1; o < e.length; o++) {
-            var c = e[o];
-            s.push(1 == c ? h() | h() : 2 == c ? h() & h() : c ? i(c, r) : !h())
+            var h = e[o];
+            s.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? i(h, r) : !c())
         }
-        return !!h()
+        return !!c()
     }, o = (e, r) => {
         var t = y.S[e];
         if (!t || !y.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
-        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && a(e, r) ? r : e), 0)
-    }, u = (e, r, t, a) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + n(a) + ")", p = (e, r, t, a) => {
-        var n = l(e, t);
-        return i(a, n) || d(u(e, t, n, a)), f(e[t][n])
-    }, d = e => {
+        return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + a(n) + ")", p = (e, r, t, n) => {
+        var a = l(e, t);
+        return i(n, a) || f(u(e, t, a, n)), d(e[t][a])
+    }, f = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
-    }, f = e => (e.loaded = 1, e.get()), s = (e => function(r, t, a, n) {
+    }, d = e => (e.loaded = 1, e.get()), s = (e => function(r, t, n, a) {
         var i = y.I(r);
-        return i && i.then ? i.then(e.bind(e, r, y.S[r], t, a, n)) : e(r, y.S[r], t, a)
-    })(((e, r, t, a) => (o(e, t), p(r, 0, t, a)))), h = {}, c = {
+        return i && i.then ? i.then(e.bind(e, r, y.S[r], t, n, a)) : e(r, y.S[r], t, n)
+    })(((e, r, t, n) => (o(e, t), p(r, 0, t, n)))), c = {}, h = {
+        44: () => s("default", "@jupyterlab/console", [1, 4, 1, 6]),
         88: () => s("default", "@lumino/datagrid", [1, 2, 3, 0, , "alpha", 0]),
-        153: () => s("default", "@jupyterlab/ui-components", [1, 4, 1, 5]),
         256: () => s("default", "@lumino/widgets", [1, 2, 3, 1, , "alpha", 0]),
         262: () => s("default", "@lumino/coreutils", [1, 2, 0, 0]),
+        465: () => s("default", "@jupyterlab/application", [1, 4, 1, 6]),
         602: () => s("default", "@lumino/signaling", [1, 2, 0, 0]),
-        707: () => s("default", "@jupyterlab/apputils", [1, 4, 2, 5]),
-        881: () => s("default", "@amphi/pipeline-editor", [0]),
-        965: () => s("default", "@jupyterlab/console", [1, 4, 1, 5]),
-        976: () => s("default", "@jupyterlab/application", [1, 4, 1, 5])
+        638: () => s("default", "@jupyterlab/apputils", [1, 4, 2, 6]),
+        664: () => s("default", "@jupyterlab/ui-components", [1, 4, 1, 6]),
+        881: () => s("default", "@amphi/pipeline-editor", [0])
     }, v = {
-        732: [88, 153, 256, 262, 602, 707, 881, 965, 976]
+        732: [44, 88, 256, 262, 465, 602, 638, 664, 881]
     }, m = {}, y.f.consumes = (e, r) => {
         y.o(v, e) && v[e].forEach((e => {
-            if (y.o(h, e)) return r.push(h[e]);
+            if (y.o(c, e)) return r.push(c[e]);
             if (!m[e]) {
                 var t = r => {
-                    h[e] = 0, y.m[e] = t => {
+                    c[e] = 0, y.m[e] = t => {
                         delete y.c[e], t.exports = r()
                     }
                 };
                 m[e] = !0;
-                var a = r => {
-                    delete h[e], y.m[e] = t => {
+                var n = r => {
+                    delete c[e], y.m[e] = t => {
                         throw delete y.c[e], r
                     }
                 };
                 try {
-                    var n = c[e]();
-                    n.then ? r.push(h[e] = n.then(t).catch(a)) : t(n)
+                    var a = h[e]();
+                    a.then ? r.push(c[e] = a.then(t).catch(n)) : t(a)
                 } catch (e) {
-                    a(e)
+                    n(e)
                 }
             }
         }))
     }, (() => {
         var e = {
             680: 0
         };
         y.f.j = (r, t) => {
-            var a = y.o(e, r) ? e[r] : void 0;
-            if (0 !== a)
-                if (a) t.push(a[2]);
+            var n = y.o(e, r) ? e[r] : void 0;
+            if (0 !== n)
+                if (n) t.push(n[2]);
                 else {
-                    var n = new Promise(((t, n) => a = e[r] = [t, n]));
-                    t.push(a[2] = n);
+                    var a = new Promise(((t, a) => n = e[r] = [t, a]));
+                    t.push(n[2] = a);
                     var i = y.p + y.u(r),
                         o = new Error;
                     y.l(i, (t => {
-                        if (y.o(e, r) && (0 !== (a = e[r]) && (e[r] = void 0), a)) {
-                            var n = t && ("load" === t.type ? "missing" : t.type),
+                        if (y.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var a = t && ("load" === t.type ? "missing" : t.type),
                                 i = t && t.target && t.target.src;
-                            o.message = "Loading chunk " + r + " failed.\n(" + n + ": " + i + ")", o.name = "ChunkLoadError", o.type = n, o.request = i, a[1](o)
+                            o.message = "Loading chunk " + r + " failed.\n(" + a + ": " + i + ")", o.name = "ChunkLoadError", o.type = a, o.request = i, n[1](o)
                         }
                     }), "chunk-" + r, r)
                 }
         };
         var r = (r, t) => {
-                var a, n, [i, o, l] = t,
+                var n, a, [i, o, l] = t,
                     u = 0;
                 if (i.some((r => 0 !== e[r]))) {
-                    for (a in o) y.o(o, a) && (y.m[a] = o[a]);
+                    for (n in o) y.o(o, n) && (y.m[n] = o[n]);
                     l && l(y)
                 }
-                for (r && r(t); u < i.length; u++) n = i[u], y.o(e, n) && e[n] && e[n][0](), e[n] = 0
+                for (r && r(t); u < i.length; u++) a = i[u], y.o(e, a) && e[a] && e[a][0](), e[a] = 0
             },
             t = self.webpackChunk_amphi_pipeline_metadata_panel = self.webpackChunk_amphi_pipeline_metadata_panel || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
     })(), y.nc = void 0;
     var w = y(320);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB)["@amphi/pipeline-metadata-panel"] = w
 })();
```

### Comparing `jupyterlab_amphi-0.1.4/amphi/pipeline-metadata-panel/static/third-party-licenses.json` & `jupyterlab_amphi-0.2.0/amphi/pipeline-metadata-panel/static/third-party-licenses.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'packages'": "{0: {'versionInfo': '6.11.0'}}"}*

```diff
@@ -1,14 +1,14 @@
 {
     "packages": [
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "css-loader",
-            "versionInfo": "6.10.0"
+            "versionInfo": "6.11.0"
         },
         {
             "extractedText": "Copyright JS Foundation and other contributors\n\nPermission is hereby granted, free of charge, to any person obtaining\na copy of this software and associated documentation files (the\n'Software'), to deal in the Software without restriction, including\nwithout limitation the rights to use, copy, modify, merge, publish,\ndistribute, sublicense, and/or sell copies of the Software, and to\npermit persons to whom the Software is furnished to do so, subject to\nthe following conditions:\n\nThe above copyright notice and this permission notice shall be\nincluded in all copies or substantial portions of the Software.\n\nTHE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,\nEXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF\nMERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.\nIN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY\nCLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,\nTORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE\nSOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.\n",
             "licenseId": "MIT",
             "name": "style-loader",
             "versionInfo": "3.3.4"
         }
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/package.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/package.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9653679653679654%*

 * *Differences: {"'dependencies'": "{'antd': '^5.16.0', 'react-dnd': '^16.0.1', 'react-dnd-html5-backend': "*

 * *                   "'^16.0.1', 'styled-components': '^6.1.8', delete: ['@headlessui/react']}",*

 * * "'version'": "'0.2.0'"}*

```diff
@@ -3,21 +3,24 @@
         "email": "tgourdel@amphi.ai",
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
-        "@headlessui/react": "^1.7.18",
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.1.5",
         "@lumino/widgets": "^2.0.0",
+        "antd": "^5.16.0",
+        "react-dnd": "^16.0.1",
+        "react-dnd-html5-backend": "^16.0.1",
         "react-dom": "^18.2.0",
         "react-flow-renderer": "^10.3.17",
-        "react-select": "^5.8.0"
+        "react-select": "^5.8.0",
+        "styled-components": "^6.1.8"
     },
     "description": "Amphi Pipeline Components Manager",
     "devDependencies": {
         "@jupyterlab/builder": "^4.1.5",
         "@typescript-eslint/eslint-plugin": "^4.8.1",
         "@typescript-eslint/parser": "^4.8.1",
         "eslint": "^7.14.0",
@@ -85,9 +88,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/tsconfig.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/tsconfig.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958333333333332%*

 * *Differences: {"'compilerOptions'": "{'noImplicitAny': False}"}*

```diff
@@ -5,15 +5,15 @@
         "declaration": true,
         "esModuleInterop": true,
         "incremental": true,
         "jsx": "react",
         "module": "esnext",
         "moduleResolution": "node",
         "noEmitOnError": true,
-        "noImplicitAny": true,
+        "noImplicitAny": false,
         "noUnusedLocals": false,
         "outDir": "lib",
         "preserveWatchOutput": true,
         "resolveJsonModule": true,
         "rootDir": "src",
         "skipLibCheck": true,
         "strict": false,
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/BrowseFileDialog.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/BrowseFileDialog.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/CustomHandle.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/CustomHandle.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/PipelineComponent.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/PipelineComponent.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -5,33 +5,32 @@
 
   return class implements ComponentItem {
 
     public static instance: T;
     public _name: string;
     public _id: string;
     public _type: string;
-    public _icon: LabIcon;
+    public _icon: any;
     public _default: object;
     public _form: object;
 
     public constructor() { }
 
     public static getInstance(): T {
       if (!this.instance) {
-        this.instance = new this() as T;
+        this.instance = new this() as unknown as T;
       }
       return this.instance;
     }
 
     public static get Name() {
       const instance = this.getInstance();
       return instance._name;
     }
 
-    // Static getter for the icon
     public static get Type() {
       const instance = this.getInstance();
       return instance._type;
     }
 
     // Static getter for the icon
     public static get Icon() {
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/icons.ts` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/index.ts` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/index.ts`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import {
   JupyterFrontEnd,
   JupyterFrontEndPlugin
 } from '@jupyterlab/application';
 import { LabIcon } from '@jupyterlab/ui-components';
 import { Token } from '@lumino/coreutils';
 
-export { setDefaultConfig, onChange, generateUIFormComponent } from './configUtils';
+export { setDefaultConfig, onChange, generateUIFormComponent, FieldDescriptor } from './configUtils';
 export { renderComponentUI, renderHandle } from './rendererUtils'
 export { PipelineComponent } from './PipelineComponent'
+export { CodeGenerator } from './CodeGenerator'
+export { PipelineService } from './PipelineService'
 
 
 interface ComponentItem {
   _id: string;
   _name: string;
   _type: string;
   _icon: LabIcon;
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/forms/keyValueForm.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/keyValueForm.tsx`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import React, { useState } from 'react';
 import { FieldDescriptor } from '../configUtils'
 import { minusIcon, plusIcon } from '../icons';
+import { Form, Divider, Input, Select, Space, Button } from 'antd';
+import { MinusCircleOutlined, PlusOutlined, MenuOutlined } from '@ant-design/icons';
 
 // Define a type for your component's props
 interface KeyValueFormProps {
   field: FieldDescriptor;
   handleChange: (values: any, fieldId: string) => void;
   initialValues?: { key: string; value: string }[]; // Add this line
 }
@@ -35,45 +37,45 @@
 
     setKeyValuePairs(updatedKeyValuePairs);
     handleChange(updatedKeyValuePairs, field.id);
 
   };
 
   return (
-    <div>
-      {keyValuePairs.map((pair, index) => (
-        <div key={index} className="col-span-1 flex items-center space-x-2">
-          <input
-            type="text"
-            name={`${field.id}_key_${index}`}
-            placeholder="Key"
-            id={`${field.id}_key_${index}`}
-            value={pair.key}
-            onChange={(e) => handleChangeKV(e, index, 'key')}
-            className="mt-1 h-6 w-full rounded-sm border-gray-200 shadow-sm sm:text-xs"
-          />
-          <input
-            type="text"
-            name={`${field.id}_value_${index}`}
-            placeholder="Value"
-            id={`${field.id}_value_${index}`}
-            value={pair.value}
-            onChange={(e) => handleChangeKV(e, index, 'value')}
-            className="mt-1 h-6 w-full rounded-sm border-gray-200 shadow-sm sm:text-xs"
-          />
-          <button type="button"
-            onClick={() => handleRemovePair(index)}
-            className="nodrag flex flex-col justify-center items-center mt-1 w-9 h-6 rounded-sm bg-gray-500 text-white shadow-sm sm:text-xs">
-            <minusIcon.react className="" />
-          </button>
-        </div>
-      ))}
-      <button type="button"
-        onClick={handleAddPair}
-        className="nodrag flex flex-col justify-center items-center mt-2 w-9 h-6 rounded-sm bg-gray-500 text-white shadow-sm sm:text-xs">
-        <plusIcon.react className="" />
-      </button>
-    </div>
+    <Form.List name="keyValue">
+      {(fields, { add, remove }) => (
+        <>
+          <Form.Item>
+            {keyValuePairs.map((pair, index) => (
+              <Space style={{ display: 'flex', marginBottom: 8 }} align="baseline">
+                <Input
+                  name={`${field.id}_key_${index}`}
+                  placeholder={field.placeholder?.key || 'key'}
+                  id={`${field.id}_key_${index}`}
+                  value={pair.key}
+                  onChange={(e) => handleChangeKV(e, index, 'key')}
+                  autoComplete="off"
+                />
+                <Input
+                  name={`${field.id}_value_${index}`}
+                  placeholder={field.placeholder?.value || 'value'}
+                  id={`${field.id}_value_${index}`}
+                  value={pair.value}
+                  onChange={(e) => handleChangeKV(e, index, 'value')} 
+                  autoComplete="off"
+                  />
+                <MinusCircleOutlined onClick={() => handleRemovePair(index)} />
+              </Space>
+            ))}
+          </Form.Item>
+          <Form.Item>
+            <Button type="dashed" onClick={handleAddPair} block icon={<PlusOutlined />}>
+              Add {field.elementName ? field.elementName : 'item'}
+            </Button>
+          </Form.Item>
+        </>
+      )}
+    </Form.List>
   );
 };
 
 export default KeyValueForm;
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/src/forms/valuesListForm.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/src/forms/valuesListForm.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/alert-triangle-fill-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/settings-16.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/settings-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/settings-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/settings-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/trash-16.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/trash-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/trash-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/trash-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-components-manager/style/icons/x-square-16.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-components-manager/style/icons/x-square-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/package.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9747023809523809%*

 * *Differences: {"'dependencies'": "{delete: ['@headlessui/react']}", "'version'": "'0.2.0'"}*

```diff
@@ -4,15 +4,14 @@
         "name": "Thibaut Gourdel"
     },
     "bugs": {
         "url": "https://github.com/amphi-ai/jupyterlab-amphi/issues"
     },
     "dependencies": {
         "@amphi/pipeline-components-manager": "file:./../pipeline-components-manager",
-        "@headlessui/react": "^1.7.18",
         "@jupyterlab/application": "^4.1.5",
         "@jupyterlab/apputils": "^4.1.9",
         "@jupyterlab/docmanager-extension": "^4.1.5",
         "@jupyterlab/filebrowser": "^4.1.5",
         "@jupyterlab/launcher": "^4.1.5",
         "@jupyterlab/logconsole": "^4.1.5",
         "@jupyterlab/mainmenu": "^4.1.5",
@@ -98,9 +97,9 @@
     "sideEffects": [
         "style/*.css",
         "style/index.js"
     ],
     "style": "style/index.css",
     "styleModule": "style/index.js",
     "types": "lib/index.d.ts",
-    "version": "0.1.4"
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/pipeline-16.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/pipeline-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/pipeline-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/pipeline-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/tsconfig.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/schema/plugin copy.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/schema/plugin copy.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/schema/plugin.json` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/schema/plugin.json`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/Dropzone.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/Dropzone.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/PipelineEditorWidget.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/PipelineEditorWidget.tsx`

 * *Files 4% similar despite different names*

```diff
@@ -22,33 +22,40 @@
   getIncomers,
   getOutgoers,
   useEdgesState,
   useNodesState,
   useReactFlow
 } from 'reactflow';
 
-import { CodeGenerator } from './CodeGenerator';
+import { Tree } from 'antd';
+import type { GetProps, TreeDataNode } from 'antd';
+import { DownOutlined } from '@ant-design/icons';
+
+type DirectoryTreeProps = GetProps<typeof Tree.DirectoryTree>;
+
+const { DirectoryTree } = Tree;
+
+import { CodeGenerator, PipelineService } from '@amphi/pipeline-components-manager';
 import CustomEdge from './customEdge';
 import 'reactflow/dist/style.css';
 import '../style/output.css';
 import { pipelineIcon } from './icons';
-import { PipelineService } from './PipelineService';
 import { Dropzone } from './Dropzone';
 
 const PIPELINE_CLASS = 'amphi-PipelineEditor';
 
 export const commandIDs = {
   openDocManager: 'docmanager:open',
   newDocManager: 'docmanager:new-untitled',
   saveDocManager: 'docmanager:save',
 };
 
 export const FitViewOptions = {
   padding: 10,
-  maxZoom: 0.5
+  maxZoom: 1.0
 }
 
 /**
  * Initialization: The class extends ReactWidget and initializes the pipeline editor widget. It sets up the initial properties and state for the widget.
  */
 export class PipelineEditorWidget extends ReactWidget {
   browserFactory: IFileBrowserFactory;
@@ -141,17 +148,17 @@
 
   const edgeTypes = {
     'custom-edge': CustomEdge
   }
 
   const nodeTypes = componentService.getComponents().reduce((acc, component: any) => {
     const id = component._id;
-    const ComponentUI = (props) => <component.UIComponent context={context} manager={manager} commands={commands} {...props} />;
+    const ComponentUI = (props) => <component.UIComponent context={context} componentService={componentService} manager={manager} commands={commands} {...props} />;
 
-    acc[id] = (props) => <ComponentUI context={context} manager={manager} commands={commands} {...props} />;
+    acc[id] = (props) => <ComponentUI context={context} componentService={componentService}  manager={manager} commands={commands} {...props} />;
     return acc;
   }, {});
 
 
   const getNodeId = () => `node_${+new Date()}`;
 
   function PipelineFlow(context) {
@@ -296,15 +303,15 @@
         };
 
         setNodes((nds) => nds.concat(newNode));
       },
       [reactFlowInstance]
     );
 
-
+    
     return (
       <div className="reactflow-wrapper" ref={reactFlowWrapper}>
        <Dropzone onDrop={handleFileDrop}>
         <ReactFlow
           id={pipelineId}
           nodes={nodes}
           edges={edges}
@@ -315,17 +322,18 @@
           onDrop={onDrop}
           onDragOver={onDragOver}
           onInit={setRfInstance}
           edgeTypes={edgeTypes}
           nodeTypes={nodeTypes}
           snapToGrid={true}
           snapGrid={[15, 15]}
-          fitViewOptions={{ minZoom: 0.5, maxZoom: 1.2 }}
+          fitViewOptions={{ minZoom: 0.5, maxZoom: 1.0 }}
           fitView
           defaultViewport={defaultViewport}
+          deleteKeyCode={[]}
         > 
           <Panel position="top-right">
           </Panel>
           <Controls />
           <Background color="#aaa" gap={15} />
         </ReactFlow>
         </Dropzone>
@@ -346,75 +354,61 @@
       // Here, you can add more data as needed
       event.dataTransfer.setData('additionalData', config);
       event.dataTransfer.effectAllowed = 'move';
     };
 
     const categorizedComponents = {
       input: [],
-      output: [],
       transform: [],
+      output: [],
       other: []
     };
 
     componentService.getComponents().forEach(component => {
       const category = categorizedComponents[component._category] || categorizedComponents['other'];
       category.push(component);
     });
 
+
+    const treeData = Object.keys(categorizedComponents).map((category, index) => ({
+      title: category.charAt(0).toUpperCase() + category.slice(1),
+      key: `${index}`,
+      children: categorizedComponents[category].map((component, childIndex) => ({
+          title: (
+            <span
+              draggable
+              onDragStart={(event) => onDragStart(event, component._id, component.getDefaultConfig ? component.getDefaultConfig() : '')}
+            >
+              {component._name}
+            </span>
+          ),
+          key: `${index}-${childIndex}`,
+          isLeaf: true,
+          icon: <component._icon.react height="14px" width="14px;"/>
+      }))
+  }));
+
+
+
     return (
 
       <aside className={sidebarClass} title={'Components'}>
 
         <div className="description">
           <extensionIcon.react tag="span" width="24px" float="left" marginRight="8px" />
           Drag and drop components.
         </div>
+        <DirectoryTree
+          multiple
+          switcherIcon={<DownOutlined />}
+          showLine
+          defaultExpandAll
 
-        <ul className="mt-6 space-y-1">
-
-          {Object.keys(categorizedComponents).map((category, index) => (
-
-            <li key={category}>
-              <details className="group [&_summary::-webkit-details-marker]:hidden" open={index === 0 || index === 1 || index === 2}>
-
-                <summary
-                  className="flex cursor-pointer items-center justify-between rounded-lg px-4 py-2 text-gray-500 hover:bg-grey-100 hover:text-gray-700">
-                  <span className="text-sm font-medium"> {category.charAt(0).toUpperCase() + category.slice(1)}</span>
-                  <span className="shrink-0 transition duration-300 group-open:-rotate-180">
-                    <svg
-                      xmlns="http://www.w3.org/2000/svg"
-                      className="h-5 w-5"
-                      viewBox="0 0 20 20"
-                      fill="currentColor">
-                      <path
-                        fillRule="evenodd"
-                        d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
-                        clipRule="evenodd"/>
-                    </svg>
-                  </span>
-                </summary>
-
-                <ul className="mt-2 space-y-1 px-4">
-                  {categorizedComponents[category].map(component => (
-                    <li key={component._id}>
-                      <div
-                        key={component._id}
-                        className="draggable_component"
-                        onDragStart={(event) => onDragStart(event, component._id, component.getDefaultConfig ? component.getDefaultConfig() : '')}
-                        draggable
-                      >
-                        <component._icon.react height="16px" strokeWidth="1px" marginRight="8px" margin="0px" padding="0px" width="16px;" color="var(--cds-brand-01)" /> {component._name}
-                      </div>
-                    </li>
-                  ))}
-                </ul>
-              </details>
-            </li>
-          ))}
-        </ul>
+          treeData={treeData}
+        />
       </aside>
     );
   }
 
   return (
     <div className="palette" id="pipeline-panel">
       <ReactFlowProvider>
@@ -455,15 +449,15 @@
       browserFactory: this.browserFactory,
       defaultFileBrowser: this.defaultFileBrowser,
       context: context,
       settings: this.settings,
       componentService: this.componentService,
     };
 
-    // context.sessionContext.kernelPreference = {autoStartDefault:true, name: 'python', shutdownOnDispose: true};
+    context.sessionContext.kernelPreference = {autoStartDefault:true, name: 'python', shutdownOnDispose: false};
 
     const content = new PipelineEditorWidget(props);
     const widget = new DocumentWidget({ content, context });
 
     // Add save button
     // const saveButton = DocToolbarItems.createSaveButton(this.commands, context.fileChanged);
     const saveButton = new ToolbarButton({
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/customEdge.tsx` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/customEdge.tsx`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/icons.ts` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/icons.ts`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/src/index.ts` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/src/index.ts`

 * *Files 0% similar despite different names*

```diff
@@ -18,19 +18,18 @@
 import { ISettingRegistry } from '@jupyterlab/settingregistry';
 import { ILauncher } from '@jupyterlab/launcher';
 import { IDefaultFileBrowser, IFileBrowserFactory } from '@jupyterlab/filebrowser';
 import { IRenderMimeRegistry } from '@jupyterlab/rendermime';
 import { IStatusBar } from '@jupyterlab/statusbar';
 import { PromiseDelegate, ReadonlyJSONValue, ReadonlyPartialJSONObject, Token } from '@lumino/coreutils';
 
-import { ComponentManager } from '@amphi/pipeline-components-manager';
+import { ComponentManager, CodeGenerator, PipelineService } from '@amphi/pipeline-components-manager';
 import { pipelineCategoryIcon, pipelineBrandIcon } from './icons';
 import { PipelineEditorFactory, commandIDs } from './PipelineEditorWidget';
-import { CodeGenerator } from './CodeGenerator';
-import { PipelineService, Node, Flow } from './PipelineService';
+
 import { LabIcon } from '@jupyterlab/ui-components';
 import React from 'react';
 
 /**
  * The command IDs used by the Amphi pipeline editor plugin.
  */
 namespace CommandIDs {
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/canvas.css` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/canvas.css`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,18 @@
   @apply absolute top-[54px] right-[-3px] w-[6px] h-[25px] rounded-[2px] bg-[#778899];
 }
 
 .component .handle-left {
   @apply absolute top-[54px] left-[-3px] w-[6px] h-[25px] rounded-[2px] bg-[#778899];
 }
 
+.component .second-handle-left {
+  @apply absolute top-[114px] left-[-3px] w-[6px] h-[25px] rounded-[2px] bg-[#778899];
+}
+
 .component .handle-bottom {
   @apply absolute bottom-[-3px] w-[25px] h-[6px] rounded-[2px] bg-[#c6cfd6];
 }
 
 .component_label {
   @apply block mt-1 text-xs font-medium text-black;
 }
@@ -59,24 +63,38 @@
   @apply flex justify-center items-center align-middle h-[80px];
 }
 
 .placeholder svg {
   @apply align-middle;
 }
 
+.ant-form-item {
+  margin-bottom: 0px;
+}
+
+.ant-form-item-label {
+  font-size: 16px;
+  padding: 0 0 3px;
+}
+
+:global .ant-row .ant-form-item-row {
+  margin-top: 5px;
+}
+
 /*
 Components palette sidebar
 */
 
 .palette {
   @apply flex flex-col flex-grow h-full;
 }
 
 .palette aside {
   @apply border-r border-l border-[#eee] border-l-[#E0E0E0] p-[20px_6px] text-[12px] bg-white;
+  height: 95%;
 }
 
 .palette aside .description {
   @apply mr-[8px] mb-[10px];
 }
 
 .palette .draggable_component {
@@ -93,24 +111,24 @@
 
 @media screen and (min-width: 768px) {
   .palette {
     @apply flex flex-row; /* Sets the flex direction to row */
   }
 
   .palette aside {
-   @apply fixed top-0 right-0 h-full w-[200px] z-10 overflow-auto
+   @apply fixed top-0 right-0 h-full w-[220px] z-10 overflow-auto
   }
 }
   
 /*
 Edges 
 */
 
 .edgebutton {
-  @apply w-[20px] h-[20px] bg-[#eee] border border-white cursor-pointer rounded-full text-[12px] leading-none;
+  @apply w-[20px] h-[20px] bg-[#eee] border border-white bg-[#F2F4F7] cursor-pointer rounded-full text-[12px] leading-none;
 }
 
 .edgebutton:hover {
   @apply shadow-lg;
 }
   
 /*
```

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/pipeline-category-icon.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/pipeline-category-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/react-icon.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/react-icon.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/api-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/api-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/file-plus-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/file-plus-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/file-text-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/file-text-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/pipeline-brand-16.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/pipeline-brand-16.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/packages/pipeline-editor/style/icons/pipeline-brand-24.svg` & `jupyterlab_amphi-0.2.0/packages/pipeline-editor/style/icons/pipeline-brand-24.svg`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/LICENSE` & `jupyterlab_amphi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/README.md` & `jupyterlab_amphi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/pyproject.toml` & `jupyterlab_amphi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_amphi-0.1.4/PKG-INFO` & `jupyterlab_amphi-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: jupyterlab-amphi
-Version: 0.1.4
+Version: 0.2.0
 Dynamic: Keywords
 Summary: Amphi is a micro ETL for Jupyterlab.
 Project-URL: Homepage, https://amphi.ai
 Project-URL: Bug Tracker, https://github.com/amphi-ai/jupyterlab-amphi/issues
 Project-URL: Repository, https://github.com/amphi-ai/jupyterlab-amphi.git
 Author-email: Thibaut Gourdel <tgourdel@amphi.ai>
 License: Elastic License 2.0 \(ELv2\)
```

