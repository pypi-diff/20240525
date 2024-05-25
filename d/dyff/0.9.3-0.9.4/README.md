# Comparing `tmp/dyff-0.9.3.tar.gz` & `tmp/dyff-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyff-0.9.3.tar", last modified: Mon Jan 22 21:55:11 2024, max compression
+gzip compressed data, was "dyff-0.9.4.tar", last modified: Mon Jan 29 21:07:47 2024, max compression
```

## Comparing `dyff-0.9.3.tar` & `dyff-0.9.4.tar`

### file list

```diff
@@ -1,549 +1,545 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.896777 dyff-0.9.3/
--rw-rw-rw-   0 root         (0) root         (0)     1570 2024-01-22 21:55:02.000000 dyff-0.9.3/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)     1541 2024-01-22 21:55:02.000000 dyff-0.9.3/.gcloudignore
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-22 21:55:02.000000 dyff-0.9.3/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     4826 2024-01-22 21:55:02.000000 dyff-0.9.3/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      349 2024-01-22 21:55:02.000000 dyff-0.9.3/.helmignore
--rw-rw-rw-   0 root         (0) root         (0)      556 2024-01-22 21:55:02.000000 dyff-0.9.3/.licenserc.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2840 2024-01-22 21:55:02.000000 dyff-0.9.3/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-22 21:55:02.000000 dyff-0.9.3/.prettierignore
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-01-22 21:55:02.000000 dyff-0.9.3/.python-version
--rw-rw-rw-   0 root         (0) root         (0)     5503 2024-01-22 21:55:02.000000 dyff-0.9.3/CODE_OF_CONDUCT.md
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-22 21:55:02.000000 dyff-0.9.3/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)    11357 2024-01-22 21:55:02.000000 dyff-0.9.3/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-01-22 21:55:02.000000 dyff-0.9.3/NOTICE
--rw-r--r--   0 root         (0) root         (0)     1955 2024-01-22 21:55:11.896777 dyff-0.9.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-22 21:55:02.000000 dyff-0.9.3/README.client.md
--rw-rw-rw-   0 root         (0) root         (0)     3185 2024-01-22 21:55:02.000000 dyff-0.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.796775 dyff-0.9.3/apps/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.797775 dyff-0.9.3/apps/dyff_admin/
--rw-rw-rw-   0 root         (0) root         (0)      499 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      434 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/deploy.yaml
--rw-rw-rw-   0 root         (0) root         (0)      370 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     1613 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/dyff_admin/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.799775 dyff-0.9.3/apps/evaluation_client/
--rw-rw-rw-   0 root         (0) root         (0)      722 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25096 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/main.py
--rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     2926 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/evaluation_client/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.800775 dyff-0.9.3/apps/fetch_model/
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3417 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/main.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     3272 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/fetch_model/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.800775 dyff-0.9.3/apps/mocks/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.801775 dyff-0.9.3/apps/mocks/inferenceservice/
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      608 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1791 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/mocks/inferenceservice/server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.803775 dyff-0.9.3/apps/run_report/
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1789 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/main.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     2577 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/run_report/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.803775 dyff-0.9.3/apps/runners/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.804775 dyff-0.9.3/apps/runners/bentoml_service_openllm/
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/bentoml_service_openllm/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/bentoml_service_openllm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/bentoml_service_openllm/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/bentoml_service_openllm/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     7190 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/bentoml_service_openllm/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.805775 dyff-0.9.3/apps/runners/vllm/
--rw-rw-rw-   0 root         (0) root         (0)      905 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/vllm/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/vllm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/vllm/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4590 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/vllm/main.py
--rw-rw-rw-   0 root         (0) root         (0)      328 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/runners/vllm/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.807775 dyff-0.9.3/apps/verify_evaluation_output/
--rw-rw-rw-   0 root         (0) root         (0)      743 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      448 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)     5653 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/main.py
--rw-rw-rw-   0 root         (0) root         (0)      163 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     2470 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/verify_evaluation_output/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.809775 dyff-0.9.3/apps/workflows_informer/
--rw-rw-rw-   0 root         (0) root         (0)        5 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      943 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/Dockerfile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.809775 dyff-0.9.3/apps/workflows_informer/agent/
--rw-rw-rw-   0 root         (0) root         (0)    12223 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/agent/agent.go
--rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/gcloud-build.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2084 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/go.mod
--rw-rw-rw-   0 root         (0) root         (0)   249396 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/go.sum
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.809775 dyff-0.9.3/apps/workflows_informer/k8s/
--rw-rw-rw-   0 root         (0) root         (0)      392 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/k8s/configmap.yaml
--rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/k8s/deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/k8s/rbac.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2927 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/main.go
--rw-rw-rw-   0 root         (0) root         (0)      243 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_informer/makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.811775 dyff-0.9.3/apps/workflows_sink/
--rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      753 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/README.md
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/gcloud-build.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.811775 dyff-0.9.3/apps/workflows_sink/k8s/
--rw-rw-rw-   0 root         (0) root         (0)      386 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/k8s/configmap.yaml
--rw-rw-rw-   0 root         (0) root         (0)      665 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/k8s/deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)       59 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.812775 dyff-0.9.3/apps/workflows_sink/workflows_sink/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/workflows_sink/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/workflows_sink/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     4324 2024-01-22 21:55:02.000000 dyff-0.9.3/apps/workflows_sink/workflows_sink/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.773775 dyff-0.9.3/charts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.813775 dyff-0.9.3/charts/dyff/
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/Chart.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4286 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.813775 dyff-0.9.3/charts/dyff/templates/
--rw-rw-rw-   0 root         (0) root         (0)     3168 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/_helpers.tpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.815775 dyff-0.9.3/charts/dyff/templates/api/
--rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-configmap.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3065 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-deployment.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1022 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-hpa.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2129 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-ingress.yaml
--rw-rw-rw-   0 root         (0) root         (0)      289 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-secret-key-signing.yaml
--rw-rw-rw-   0 root         (0) root         (0)      260 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-secret.yaml
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-service.yaml
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/api/api-serviceaccount.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.816775 dyff-0.9.3/charts/dyff/templates/orchestrator/
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-configmap.yaml
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-secret.yaml
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-service.yaml
--rw-rw-rw-   0 root         (0) root         (0)      450 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-serviceaccount.yaml
--rw-rw-rw-   0 root         (0) root         (0)     3218 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-statefulset.yaml
--rw-rw-rw-   0 root         (0) root         (0)     5100 2024-01-22 21:55:02.000000 dyff-0.9.3/charts/dyff/values.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.774775 dyff-0.9.3/doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.820775 dyff-0.9.3/doc/internal/
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/admin.md
--rw-rw-rw-   0 root         (0) root         (0)    12354 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/api-server.md
--rw-rw-rw-   0 root         (0) root         (0)     7401 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/audits.md
--rw-rw-rw-   0 root         (0) root         (0)    11249 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/data-schemas.md
--rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/evaluations.md
--rw-rw-rw-   0 root         (0) root         (0)    26010 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/gcloud-notes.md
--rw-rw-rw-   0 root         (0) root         (0)     3594 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/go-operators.md
--rw-rw-rw-   0 root         (0) root         (0)    14563 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/kafkaesque.md
--rw-rw-rw-   0 root         (0) root         (0)     3244 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/models.md
--rw-rw-rw-   0 root         (0) root         (0)    14307 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/mongodb.md
--rw-rw-rw-   0 root         (0) root         (0)     7912 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/operators.md
--rw-rw-rw-   0 root         (0) root         (0)     3282 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/roadmap.md
--rw-rw-rw-   0 root         (0) root         (0)     2759 2024-01-22 21:55:02.000000 dyff-0.9.3/doc/internal/user-facing-api.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.820775 dyff-0.9.3/docker/
--rw-rw-rw-   0 root         (0) root         (0)     1131 2024-01-22 21:55:02.000000 dyff-0.9.3/docker/Dockerfile-init-workload-identity
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-01-22 21:55:02.000000 dyff-0.9.3/docker/Dockerfile-kafka-cli
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.821776 dyff-0.9.3/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.822775 dyff-0.9.3/docs/_extensions/
--rw-rw-rw-   0 root         (0) root         (0)     1687 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/_extensions/pyarrow_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.823776 dyff-0.9.3/docs/api-reference/
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/audit.rst
--rw-rw-rw-   0 root         (0) root         (0)     1493 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/client.rst
--rw-rw-rw-   0 root         (0) root         (0)      134 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/models.rst
--rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/schema.adapters.rst
--rw-rw-rw-   0 root         (0) root         (0)     4029 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/api-reference/schema.rst
--rw-rw-rw-   0 root         (0) root         (0)     2827 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.824776 dyff-0.9.3/docs/deployment/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.824776 dyff-0.9.3/docs/deployment/architecture/
--rw-rw-rw-   0 root         (0) root         (0)       68 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/deployment/architecture/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1812 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/deployment/architecture/storage.rst
--rw-rw-rw-   0 root         (0) root         (0)    15464 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/deployment/configuration.rst
--rw-rw-rw-   0 root         (0) root         (0)      114 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/deployment/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2484 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/deployment/management.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.827776 dyff-0.9.3/docs/development/
--rw-rw-rw-   0 root         (0) root         (0)     4822 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/design.rst
--rw-rw-rw-   0 root         (0) root         (0)     5930 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/dyff-operator.rst
--rw-rw-rw-   0 root         (0) root         (0)    85194 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/dyff-service-diagram.drawio
--rw-rw-rw-   0 root         (0) root         (0)   101281 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/dyff-service-diagram.pdf
--rw-rw-rw-   0 root         (0) root         (0)   112234 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/dyff-service-diagram.svg
--rw-rw-rw-   0 root         (0) root         (0)     3216 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/evaluation.yaml
--rw-rw-rw-   0 root         (0) root         (0)      122 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     7721 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/principles.rst
--rw-rw-rw-   0 root         (0) root         (0)     4154 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/development/rbac.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.828776 dyff-0.9.3/docs/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.830776 dyff-0.9.3/docs/examples/client/
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-evaluation.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-evaluation.rst
--rw-rw-rw-   0 root         (0) root         (0)     2506 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-inferenceservice.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-inferenceservice.rst
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-inferencesession.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-inferencesession.rst
--rw-rw-rw-   0 root         (0) root         (0)      462 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-report.py
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-report.rst
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-upload-dataset.py
--rw-rw-rw-   0 root         (0) root         (0)      181 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/create-upload-dataset.rst
--rw-rw-rw-   0 root         (0) root         (0)      203 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/client/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3511 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)       87 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/index.rst
--rw-rw-rw-   0 root         (0) root         (0)   285889 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/examples/simple-audit.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1708 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.832776 dyff-0.9.3/docs/releases/
--rw-rw-rw-   0 root         (0) root         (0)      814 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.5.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.5.1.rst
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.6.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.7.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.7.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      148 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.8.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/0.9.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      197 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/releases/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)    11648 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.833776 dyff-0.9.3/docs/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)    27953 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/tutorials/creating-a-dataset.rst
--rw-rw-rw-   0 root         (0) root         (0)     6700 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/tutorials/creating-an-audit.rst
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/tutorials/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.834776 dyff-0.9.3/docs/user-guide/
--rw-rw-rw-   0 root         (0) root         (0)     9207 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/user-guide/core-resources.rst
--rw-rw-rw-   0 root         (0) root         (0)    15028 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/user-guide/data-schemas.rst
--rw-rw-rw-   0 root         (0) root         (0)      137 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/user-guide/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1118 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/user-guide/installation.rst
--rw-rw-rw-   0 root         (0) root         (0)     8498 2024-01-22 21:55:02.000000 dyff-0.9.3/docs/user-guide/resource-lifecycle.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.834776 dyff-0.9.3/dotenv/
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-22 21:55:02.000000 dyff-0.9.3/dotenv/mvp.env
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.835776 dyff-0.9.3/dyff/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.838776 dyff-0.9.3/dyff/api/
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    70584 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.838776 dyff-0.9.3/dyff/api/backend/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.839776 dyff-0.9.3/dyff/api/backend/base/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/base/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2626 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/base/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4631 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/base/command.py
--rw-rw-rw-   0 root         (0) root         (0)     7778 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/base/query.py
--rw-rw-rw-   0 root         (0) root         (0)     1473 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/base/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.840776 dyff-0.9.3/dyff/api/backend/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/gcloud/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4937 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/gcloud/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.840776 dyff-0.9.3/dyff/api/backend/kafka/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/kafka/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7537 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/kafka/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.841776 dyff-0.9.3/dyff/api/backend/mock/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/mock/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2614 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/mock/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.841776 dyff-0.9.3/dyff/api/backend/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/mongodb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6265 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/mongodb/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    13663 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/backend/mongodb/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.843776 dyff-0.9.3/dyff/api/bin/
--rw-rw-rw-   0 root         (0) root         (0)     1741 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/clone_audit_procedure.py
--rw-rw-rw-   0 root         (0) root         (0)     1636 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/fetch_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.843776 dyff-0.9.3/dyff/api/bin/gcloud/
--rw-rw-rw-   0 root         (0) root         (0)     5210 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/gcloud/build_bentoml_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2062 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/gcloud/build_model_container.py
--rw-rw-rw-   0 root         (0) root         (0)      738 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/ingest_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1824 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/run_audit.py
--rw-rw-rw-   0 root         (0) root         (0)     3901 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/bin/run_jupyterbook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.845776 dyff-0.9.3/dyff/api/data/
--rw-rw-rw-   0 root         (0) root         (0)     2023 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2297 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/archives.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/arrowtypes.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/fetch.py
--rw-rw-rw-   0 root         (0) root         (0)     8460 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/huggingface.py
--rw-rw-rw-   0 root         (0) root         (0)    16984 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/ingest.py
--rw-rw-rw-   0 root         (0) root         (0)     5822 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/sinks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.846776 dyff-0.9.3/dyff/api/data/sources/
--rw-rw-rw-   0 root         (0) root         (0)      142 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4093 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/sources/zenodo.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/data/text.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.847776 dyff-0.9.3/dyff/api/mgmt/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/mgmt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      766 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/mgmt/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1420 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/mgmt/accounts.py
--rw-rw-rw-   0 root         (0) root         (0)     3192 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/mgmt/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/sanitize.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/server.py
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/server_insecure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.847776 dyff-0.9.3/dyff/api/storage/
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1957 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/storage/paths.py
--rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/timestamp.py
--rw-rw-rw-   0 root         (0) root         (0)     5863 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/tokens.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/api/typing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.847776 dyff-0.9.3/dyff/audit/
--rw-rw-rw-   0 root         (0) root         (0)      139 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.848776 dyff-0.9.3/dyff/audit/data/
--rw-rw-rw-   0 root         (0) root         (0)      200 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2353 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/data/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.848776 dyff-0.9.3/dyff/audit/metrics/
--rw-rw-rw-   0 root         (0) root         (0)      216 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/metrics/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1050 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/metrics/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4421 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/metrics/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.849776 dyff-0.9.3/dyff/audit/schemas/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/schemas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.851776 dyff-0.9.3/dyff/audit/scoring/
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3855 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     3112 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/evaluator_code_syntax_rubrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/evaluator_misinfo_commonclaims.py
--rw-rw-rw-   0 root         (0) root         (0)     3404 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/evaluator_test_rubric.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/example.py
--rw-rw-rw-   0 root         (0) root         (0)    12003 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/scoring/text.py
--rw-rw-rw-   0 root         (0) root         (0)     5750 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/audit/workflows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.852776 dyff-0.9.3/dyff/client/
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.853776 dyff-0.9.3/dyff/client/_generated/
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5911 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1940 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)    81146 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/_serialization.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.854776 dyff-0.9.3/dyff/client/_generated/aio/
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6047 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/_client.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/_vendor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.856776 dyff-0.9.3/dyff/client/_generated/aio/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   497925 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      754 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/aio/operations/_patch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.857776 dyff-0.9.3/dyff/client/_generated/operations/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/operations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   532042 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/operations/_operations.py
--rw-rw-rw-   0 root         (0) root         (0)      975 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/operations/_patch.py
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/_generated/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    52477 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/client/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.857776 dyff-0.9.3/dyff/core/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/core/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9797 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/core/config.py
--rw-rw-rw-   0 root         (0) root         (0)      466 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/core/dynamic_import.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.858776 dyff-0.9.3/dyff/models/
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10203 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/api.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.859776 dyff-0.9.3/dyff/models/bentoml/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/bentoml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      271 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/bentoml/service.py-template
--rw-rw-rw-   0 root         (0) root         (0)     6274 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/bentoml/template_openllm_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/fetch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.859776 dyff-0.9.3/dyff/models/frameworks/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/frameworks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6984 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/frameworks/transformers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.860776 dyff-0.9.3/dyff/models/outputs/
--rw-rw-rw-   0 root         (0) root         (0)     1499 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/outputs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2885 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/outputs/classification.py
--rw-rw-rw-   0 root         (0) root         (0)     1804 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/outputs/text.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.861776 dyff-0.9.3/dyff/models/sources/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      547 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/sources/git_lfs.py
--rw-rw-rw-   0 root         (0) root         (0)     1106 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/sources/huggingface_hub.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/models/sources/open_llm.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.862776 dyff-0.9.3/dyff/orchestrator/
--rw-rw-rw-   0 root         (0) root         (0)      750 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     9916 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/crd.py
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/gcloud-build.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.863776 dyff-0.9.3/dyff/orchestrator/k8s/
--rw-rw-rw-   0 root         (0) root         (0)      472 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/k8s/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2244 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/k8s/conditions.py
--rw-rw-rw-   0 root         (0) root         (0)     6781 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/k8s/resources.py
--rw-rw-rw-   0 root         (0) root         (0)    27732 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/orchestrator/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.865776 dyff-0.9.3/dyff/schema/
--rw-rw-rw-   0 root         (0) root         (0)     1012 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1056 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/copydoc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.867776 dyff-0.9.3/dyff/schema/dataset/
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/dataset/vision.py
--rw-rw-rw-   0 root         (0) root         (0)     1407 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/ids.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.867776 dyff-0.9.3/dyff/schema/io/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     3773 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/quantity.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/requests.py
--rw-rw-rw-   0 root         (0) root         (0)      100 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.868776 dyff-0.9.3/dyff/schema/v0/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.869776 dyff-0.9.3/dyff/schema/v0/r1/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    23542 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)    17115 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.871776 dyff-0.9.3/dyff/schema/v0/r1/dataset/
--rw-rw-rw-   0 root         (0) root         (0)     2530 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12317 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/arrow.py
--rw-rw-rw-   0 root         (0) root         (0)      525 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/binary.py
--rw-rw-rw-   0 root         (0) root         (0)      292 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/classification.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/text.py
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/dataset/vision.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.871776 dyff-0.9.3/dyff/schema/v0/r1/io/
--rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/io/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5301 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/io/vllm.py
--rw-rw-rw-   0 root         (0) root         (0)    44058 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/platform.py
--rw-rw-rw-   0 root         (0) root         (0)     5878 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/requests.py
--rw-rw-rw-   0 root         (0) root         (0)    10503 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/test.py
--rw-rw-rw-   0 root         (0) root         (0)      344 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/v0/r1/version.py
--rw-rw-rw-   0 root         (0) root         (0)      353 2024-01-22 21:55:02.000000 dyff-0.9.3/dyff/schema/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.896777 dyff-0.9.3/dyff.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1955 2024-01-22 21:55:11.000000 dyff-0.9.3/dyff.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15024 2024-01-22 21:55:11.000000 dyff-0.9.3/dyff.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-22 21:55:11.000000 dyff-0.9.3/dyff.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-01-22 21:55:11.000000 dyff-0.9.3/dyff.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2024-01-22 21:55:11.000000 dyff-0.9.3/dyff.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.783775 dyff-0.9.3/gcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.873776 dyff-0.9.3/gcloud/build/
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/build/api-server-proxy.yaml
--rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/build/api-server.yaml
--rw-rw-rw-   0 root         (0) root         (0)      451 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/build/init-workload-identity.yaml
--rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/build/kafka-cli.yaml
--rw-rw-rw-   0 root         (0) root         (0)      421 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/build/orchestrator.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.873776 dyff-0.9.3/gcloud/datastore/
--rw-rw-rw-   0 root         (0) root         (0)      583 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/datastore/index.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.874776 dyff-0.9.3/gcloud/k8s/
--rw-rw-rw-   0 root         (0) root         (0)      262 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/k8s/keepalive.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/k8s/run-fetch-data.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1202 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/k8s/run-ingest-dataset.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1581 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/k8s/run-model-test.yaml
--rw-rw-rw-   0 root         (0) root         (0)      327 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud/k8s/workload-identity-test.yaml
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-01-22 21:55:02.000000 dyff-0.9.3/gcloud-build.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.875776 dyff-0.9.3/ingest/
--rw-rw-rw-   0 root         (0) root         (0)      824 2024-01-22 21:55:02.000000 dyff-0.9.3/ingest/imagenet-c.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2275 2024-01-22 21:55:02.000000 dyff-0.9.3/ingest/mnist-c.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-01-22 21:55:02.000000 dyff-0.9.3/ingest/test-imagenet-c.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.785775 dyff-0.9.3/k8s/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.876777 dyff-0.9.3/k8s/deploy/
--rw-rw-rw-   0 root         (0) root         (0)      116 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/api-key-signing-secret-placeholder.yaml
--rw-rw-rw-   0 root         (0) root         (0)      758 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/api-server-ingress.yaml
--rw-rw-rw-   0 root         (0) root         (0)      384 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/api-server-issuer-letsencrypt.yaml
--rw-rw-rw-   0 root         (0) root         (0)      182 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/api-server-secret-placeholder.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1850 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/api-server.yaml
--rw-rw-rw-   0 root         (0) root         (0)      249 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/gitlab-pull-secret-placeholder.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.877776 dyff-0.9.3/k8s/deploy/kafka/
--rw-rw-rw-   0 root         (0) root         (0)      246 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/kafka/cli.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2479 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/kafka/kafka.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.877776 dyff-0.9.3/k8s/deploy/kafka/topics/
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/kafka/topics/dyff-workflows.yaml
--rw-rw-rw-   0 root         (0) root         (0)      611 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/kafka/topics/test-workflows.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.878776 dyff-0.9.3/k8s/deploy/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)      232 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/mongodb/user-auth-backend.yaml
--rw-rw-rw-   0 root         (0) root         (0)      236 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/mongodb/user-query-backend.yaml
--rw-rw-rw-   0 root         (0) root         (0)      245 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/mongodb/user-workflows-sink.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2199 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/orchestrator.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.878776 dyff-0.9.3/k8s/deploy/test/
--rw-rw-rw-   0 root         (0) root         (0)      413 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/test/api-server-issuer-letsencrypt.yaml
--rw-rw-rw-   0 root         (0) root         (0)      626 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/deploy/test/api-server-mock.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.879777 dyff-0.9.3/k8s/network/
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/network/audit.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.879777 dyff-0.9.3/k8s/rbac/
--rw-rw-rw-   0 root         (0) root         (0)      574 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/rbac/api-server.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.879777 dyff-0.9.3/k8s/rbac/mongodb/
--rw-rw-rw-   0 root         (0) root         (0)      589 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/rbac/mongodb/mongodb-admin.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1591 2024-01-22 21:55:02.000000 dyff-0.9.3/k8s/rbac/orchestrator.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2722 2024-01-22 21:55:02.000000 dyff-0.9.3/makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.880777 dyff-0.9.3/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.884777 dyff-0.9.3/mongodb/deploy/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.885777 dyff-0.9.3/mongodb/deploy/backup/
--rw-rw-rw-   0 root         (0) root         (0)      254 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/backup/backup.yaml
--rw-rw-rw-   0 root         (0) root         (0)      625 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/backup/restore.yaml
--rw-rw-rw-   0 root         (0) root         (0)      210 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/backup-s3.yaml
--rw-rw-rw-   0 root         (0) root         (0)   883127 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/bundle.yaml
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/cr-minimal.yaml
--rw-rw-rw-   0 root         (0) root         (0)    17064 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/cr.yaml
--rw-rw-rw-   0 root         (0) root         (0)   879266 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/crd.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.786775 dyff-0.9.3/mongodb/deploy/csv/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.886777 dyff-0.9.3/mongodb/deploy/csv/redhat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.786775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.887777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/
--rw-rw-rw-   0 root         (0) root         (0)    60108 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/percona-server-mongodb-operator.v1.4.0.clusterserviceversion.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1161 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)      823 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)      946 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.887777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/metadata/annotations.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.787775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.888777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/
--rw-rw-rw-   0 root         (0) root         (0)    61754 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/percona-server-mongodb-operator.v1.5.0.clusterserviceversion.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1005 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.889777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/metadata/annotations.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.787775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.889777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.788775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.890777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/
--rw-rw-rw-   0 root         (0) root         (0)    62912 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/percona-server-mongodb-operator.v1.6.0.clusterserviceversion.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1064 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.890777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/metadata/annotations.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.788775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.890777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.789775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.891777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/
--rw-rw-rw-   0 root         (0) root         (0)    63701 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/percona-server-mongodb-operator.v1.7.0.clusterserviceversion.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.892777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/metadata/
--rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/metadata/annotations.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.789775 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.892777 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/
--rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/README.md
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.4.0.Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.5.0.Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.6.0.Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.7.0.Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)   883321 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/cw-bundle.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1262 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/cw-operator.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2785 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/cw-rbac.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1337 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/operator.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2516 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/rbac.yaml
--rw-rw-rw-   0 root         (0) root         (0)      633 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/secrets.yaml
--rw-rw-rw-   0 root         (0) root         (0)    12801 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/deploy/ssl-secrets.yaml
--rwxrwxrwx   0 root         (0) root         (0)     1550 2024-01-22 21:55:02.000000 dyff-0.9.3/mongodb/fetch-deploy-files-from-upstream.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.892777 dyff-0.9.3/openapi/
--rw-rw-rw-   0 root         (0) root         (0)   141209 2024-01-22 21:55:02.000000 dyff-0.9.3/openapi/dyff.json
--rw-rw-rw-   0 root         (0) root         (0)      317 2024-01-22 21:55:02.000000 dyff-0.9.3/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)       53 2024-01-22 21:55:02.000000 dyff-0.9.3/package.json
--rw-rw-rw-   0 root         (0) root         (0)     6640 2024-01-22 21:55:02.000000 dyff-0.9.3/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       76 2024-01-22 21:55:02.000000 dyff-0.9.3/requirements-orchestrator.in
--rw-rw-rw-   0 root         (0) root         (0)     1465 2024-01-22 21:55:02.000000 dyff-0.9.3/requirements-orchestrator.txt
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-01-22 21:55:02.000000 dyff-0.9.3/requirements.in
--rw-rw-rw-   0 root         (0) root         (0)     7250 2024-01-22 21:55:02.000000 dyff-0.9.3/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.894777 dyff-0.9.3/scripts/
--rwxrwxrwx   0 root         (0) root         (0)     1288 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/create-gcs-bucket.py
--rwxrwxrwx   0 root         (0) root         (0)     3366 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/fix-openapi.py
--rwxrwxrwx   0 root         (0) root         (0)     7444 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/generate-config-listing.py
--rwxrwxrwx   0 root         (0) root         (0)      569 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/generate-openapi-definitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.894777 dyff-0.9.3/scripts/inferenceservices/
--rw-rw-rw-   0 root         (0) root         (0)     2510 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/inferenceservices/tiiuae--falcon-7b--default.py
--rw-rw-rw-   0 root         (0) root         (0)     2443 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/k8s-secret-data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.895777 dyff-0.9.3/scripts/models/
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/models/databricks--dolly-v2-3b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1355 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/models/databricks--dolly-v2-3b.py
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/models/tiiuae--falcon-7b--rox.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1337 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/models/tiiuae--falcon-7b.py
--rw-rw-rw-   0 root         (0) root         (0)      725 2024-01-22 21:55:02.000000 dyff-0.9.3/scripts/rotate-api-key-signing-secret.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-22 21:55:11.896777 dyff-0.9.3/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      696 2024-01-22 21:55:02.000000 dyff-0.9.3/skaffold.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-22 21:55:11.895777 dyff-0.9.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-22 21:55:02.000000 dyff-0.9.3/tests/test_nothing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.346864 dyff-0.9.4/
+-rw-rw-rw-   0 root         (0) root         (0)     1570 2024-01-29 21:07:38.000000 dyff-0.9.4/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)     1541 2024-01-29 21:07:38.000000 dyff-0.9.4/.gcloudignore
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-29 21:07:38.000000 dyff-0.9.4/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     4826 2024-01-29 21:07:38.000000 dyff-0.9.4/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      349 2024-01-29 21:07:38.000000 dyff-0.9.4/.helmignore
+-rw-rw-rw-   0 root         (0) root         (0)      606 2024-01-29 21:07:38.000000 dyff-0.9.4/.licenserc.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-01-29 21:07:38.000000 dyff-0.9.4/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       77 2024-01-29 21:07:38.000000 dyff-0.9.4/.prettierignore
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-01-29 21:07:38.000000 dyff-0.9.4/.python-version
+-rw-rw-rw-   0 root         (0) root         (0)     5503 2024-01-29 21:07:38.000000 dyff-0.9.4/CODE_OF_CONDUCT.md
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-29 21:07:38.000000 dyff-0.9.4/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)      740 2024-01-29 21:07:38.000000 dyff-0.9.4/Dockerfile-api-server-insecure
+-rw-rw-rw-   0 root         (0) root         (0)    11357 2024-01-29 21:07:38.000000 dyff-0.9.4/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-01-29 21:07:38.000000 dyff-0.9.4/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     1955 2024-01-29 21:07:47.346864 dyff-0.9.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-01-29 21:07:38.000000 dyff-0.9.4/README.client.md
+-rw-rw-rw-   0 root         (0) root         (0)     3185 2024-01-29 21:07:38.000000 dyff-0.9.4/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.257948 dyff-0.9.4/apps/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.258865 dyff-0.9.4/apps/dyff_admin/
+-rw-rw-rw-   0 root         (0) root         (0)      499 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      434 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/deploy.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      370 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/dyff_admin/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.259781 dyff-0.9.4/apps/evaluation_client/
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    24820 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      198 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/evaluation_client/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.260698 dyff-0.9.4/apps/fetch_model/
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.260698 dyff-0.9.4/apps/fetch_model/fetch_model/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3407 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1273 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/fetch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.261615 dyff-0.9.4/apps/fetch_model/fetch_model/sources/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/sources/git_lfs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/sources/huggingface_hub.py
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/fetch_model/sources/open_llm.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     3272 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/fetch_model/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.261615 dyff-0.9.4/apps/mocks/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.264365 dyff-0.9.4/apps/mocks/inferenceservice/
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/mocks/inferenceservice/server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.265282 dyff-0.9.4/apps/run_report/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1789 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     2577 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/run_report/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.265282 dyff-0.9.4/apps/runners/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.266198 dyff-0.9.4/apps/runners/bentoml_service_openllm/
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/bentoml_service_openllm/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/bentoml_service_openllm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/bentoml_service_openllm/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/bentoml_service_openllm/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     7190 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/bentoml_service_openllm/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.267115 dyff-0.9.4/apps/runners/huggingface/
+-rw-rw-rw-   0 root         (0) root         (0)      558 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/huggingface/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/huggingface/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/huggingface/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4479 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/huggingface/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      352 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/huggingface/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.268031 dyff-0.9.4/apps/runners/vllm/
+-rw-rw-rw-   0 root         (0) root         (0)      905 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/vllm/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/vllm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/vllm/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4590 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/vllm/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      328 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/runners/vllm/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.269865 dyff-0.9.4/apps/verify_evaluation_output/
+-rw-rw-rw-   0 root         (0) root         (0)      743 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      448 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6135 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      163 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     2470 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/verify_evaluation_output/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.270781 dyff-0.9.4/apps/workflows_informer/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      943 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/Dockerfile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.270781 dyff-0.9.4/apps/workflows_informer/agent/
+-rw-rw-rw-   0 root         (0) root         (0)    12223 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/agent/agent.go
+-rw-rw-rw-   0 root         (0) root         (0)      406 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/gcloud-build.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2084 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/go.mod
+-rw-rw-rw-   0 root         (0) root         (0)   249396 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/go.sum
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.271698 dyff-0.9.4/apps/workflows_informer/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)      392 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/k8s/configmap.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      672 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/k8s/deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      867 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/k8s/rbac.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2927 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/main.go
+-rw-rw-rw-   0 root         (0) root         (0)      243 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_informer/makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.274448 dyff-0.9.4/apps/workflows_sink/
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      753 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/gcloud-build.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.274448 dyff-0.9.4/apps/workflows_sink/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)      386 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/k8s/configmap.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      665 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/k8s/deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)       59 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.275365 dyff-0.9.4/apps/workflows_sink/workflows_sink/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/workflows_sink/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/workflows_sink/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4324 2024-01-29 21:07:38.000000 dyff-0.9.4/apps/workflows_sink/workflows_sink/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.236865 dyff-0.9.4/charts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.275365 dyff-0.9.4/charts/dyff/
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/Chart.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4286 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.275365 dyff-0.9.4/charts/dyff/templates/
+-rw-rw-rw-   0 root         (0) root         (0)     3168 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/_helpers.tpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.278115 dyff-0.9.4/charts/dyff/templates/api/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-configmap.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3065 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-deployment.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1022 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-hpa.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2129 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-ingress.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      289 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-secret-key-signing.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      260 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-secret.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-service.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/api/api-serviceaccount.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.279031 dyff-0.9.4/charts/dyff/templates/orchestrator/
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-configmap.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-secret.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-service.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      450 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-serviceaccount.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     3218 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-statefulset.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     5100 2024-01-29 21:07:38.000000 dyff-0.9.4/charts/dyff/values.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.237782 dyff-0.9.4/doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.281781 dyff-0.9.4/doc/internal/
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/admin.md
+-rw-rw-rw-   0 root         (0) root         (0)    12354 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/api-server.md
+-rw-rw-rw-   0 root         (0) root         (0)     7401 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/audits.md
+-rw-rw-rw-   0 root         (0) root         (0)    11249 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/data-schemas.md
+-rw-rw-rw-   0 root         (0) root         (0)     1244 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/evaluations.md
+-rw-rw-rw-   0 root         (0) root         (0)    26010 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/gcloud-notes.md
+-rw-rw-rw-   0 root         (0) root         (0)     3594 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/go-operators.md
+-rw-rw-rw-   0 root         (0) root         (0)    14563 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/kafkaesque.md
+-rw-rw-rw-   0 root         (0) root         (0)     3244 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/models.md
+-rw-rw-rw-   0 root         (0) root         (0)    14307 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/mongodb.md
+-rw-rw-rw-   0 root         (0) root         (0)     7912 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/operators.md
+-rw-rw-rw-   0 root         (0) root         (0)     3282 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/roadmap.md
+-rw-rw-rw-   0 root         (0) root         (0)     2759 2024-01-29 21:07:38.000000 dyff-0.9.4/doc/internal/user-facing-api.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.281781 dyff-0.9.4/docker/
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2024-01-29 21:07:38.000000 dyff-0.9.4/docker/Dockerfile-init-workload-identity
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-01-29 21:07:38.000000 dyff-0.9.4/docker/Dockerfile-kafka-cli
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.282698 dyff-0.9.4/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.282698 dyff-0.9.4/docs/_extensions/
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/_extensions/pyarrow_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.285448 dyff-0.9.4/docs/api-reference/
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/audit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1493 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/client.rst
+-rw-rw-rw-   0 root         (0) root         (0)      134 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/models.rst
+-rw-rw-rw-   0 root         (0) root         (0)      172 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/schema.adapters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4029 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/api-reference/schema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2827 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.285448 dyff-0.9.4/docs/deployment/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.286365 dyff-0.9.4/docs/deployment/architecture/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/deployment/architecture/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1812 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/deployment/architecture/storage.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15722 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/deployment/configuration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      114 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/deployment/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2484 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/deployment/management.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.288198 dyff-0.9.4/docs/development/
+-rw-rw-rw-   0 root         (0) root         (0)     4822 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/design.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5930 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/dyff-operator.rst
+-rw-rw-rw-   0 root         (0) root         (0)    85194 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/dyff-service-diagram.drawio
+-rw-rw-rw-   0 root         (0) root         (0)   101281 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/dyff-service-diagram.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   112234 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/dyff-service-diagram.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3216 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/evaluation.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7721 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/principles.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4154 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/development/rbac.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.288198 dyff-0.9.4/docs/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.290948 dyff-0.9.4/docs/examples/client/
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-evaluation.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-evaluation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2506 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-inferenceservice.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-inferenceservice.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-inferencesession.py
+-rw-rw-rw-   0 root         (0) root         (0)      219 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-inferencesession.rst
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-report.py
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-report.rst
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-upload-dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)      181 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/create-upload-dataset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      203 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/client/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3511 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)       87 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)   285889 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/examples/simple-audit.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.292781 dyff-0.9.4/docs/releases/
+-rw-rw-rw-   0 root         (0) root         (0)      814 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.5.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.5.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1232 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.6.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.7.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.7.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      148 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.8.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      143 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/0.9.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      197 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/releases/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)    11648 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.292781 dyff-0.9.4/docs/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)    27953 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/tutorials/creating-a-dataset.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6700 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/tutorials/creating-an-audit.rst
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/tutorials/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.293698 dyff-0.9.4/docs/user-guide/
+-rw-rw-rw-   0 root         (0) root         (0)     9207 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/user-guide/core-resources.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15028 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/user-guide/data-schemas.rst
+-rw-rw-rw-   0 root         (0) root         (0)      137 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/user-guide/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1118 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/user-guide/installation.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8498 2024-01-29 21:07:38.000000 dyff-0.9.4/docs/user-guide/resource-lifecycle.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.294614 dyff-0.9.4/dotenv/
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-29 21:07:38.000000 dyff-0.9.4/dotenv/mvp.env
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.294614 dyff-0.9.4/dyff/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.298281 dyff-0.9.4/dyff/api/
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    70584 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.298281 dyff-0.9.4/dyff/api/backend/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.299198 dyff-0.9.4/dyff/api/backend/base/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/base/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2626 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/base/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4631 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/base/command.py
+-rw-rw-rw-   0 root         (0) root         (0)     7778 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/base/query.py
+-rw-rw-rw-   0 root         (0) root         (0)     1473 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/base/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.300114 dyff-0.9.4/dyff/api/backend/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/gcloud/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4937 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/gcloud/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.300114 dyff-0.9.4/dyff/api/backend/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/kafka/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7537 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/kafka/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.301031 dyff-0.9.4/dyff/api/backend/mock/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/mock/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2614 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/mock/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.301031 dyff-0.9.4/dyff/api/backend/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/mongodb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6265 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/mongodb/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    13663 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/backend/mongodb/query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.301948 dyff-0.9.4/dyff/api/bin/
+-rw-rw-rw-   0 root         (0) root         (0)     1741 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/clone_audit_procedure.py
+-rw-rw-rw-   0 root         (0) root         (0)     1636 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/fetch_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.302864 dyff-0.9.4/dyff/api/bin/gcloud/
+-rw-rw-rw-   0 root         (0) root         (0)     5210 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/gcloud/build_bentoml_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2062 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/gcloud/build_model_container.py
+-rw-rw-rw-   0 root         (0) root         (0)      738 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/ingest_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     1824 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/run_audit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3901 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/bin/run_jupyterbook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.304698 dyff-0.9.4/dyff/api/data/
+-rw-rw-rw-   0 root         (0) root         (0)     2023 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2297 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/archives.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/arrowtypes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/fetch.py
+-rw-rw-rw-   0 root         (0) root         (0)     8460 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/huggingface.py
+-rw-rw-rw-   0 root         (0) root         (0)    16984 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/ingest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5822 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/sinks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.304698 dyff-0.9.4/dyff/api/data/sources/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4093 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/sources/zenodo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2283 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/data/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.305614 dyff-0.9.4/dyff/api/mgmt/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/mgmt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      766 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/mgmt/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/mgmt/accounts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3192 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/mgmt/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)      918 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/sanitize.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/server.py
+-rw-rw-rw-   0 root         (0) root         (0)     1342 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/server_insecure.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.305614 dyff-0.9.4/dyff/api/storage/
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1957 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/storage/paths.py
+-rw-rw-rw-   0 root         (0) root         (0)      654 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/timestamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     5863 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/tokens.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/typing.py
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/api/web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.307448 dyff-0.9.4/dyff/audit/
+-rw-rw-rw-   0 root         (0) root         (0)      139 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.307448 dyff-0.9.4/dyff/audit/data/
+-rw-rw-rw-   0 root         (0) root         (0)      200 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2353 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/data/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.308364 dyff-0.9.4/dyff/audit/metrics/
+-rw-rw-rw-   0 root         (0) root         (0)      216 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/metrics/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1050 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/metrics/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4421 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/metrics/text.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.308364 dyff-0.9.4/dyff/audit/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/schemas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.310198 dyff-0.9.4/dyff/audit/scoring/
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3855 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)     3112 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/evaluator_code_syntax_rubrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/evaluator_misinfo_commonclaims.py
+-rw-rw-rw-   0 root         (0) root         (0)     5756 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/evaluator_personas.py
+-rw-rw-rw-   0 root         (0) root         (0)     3404 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/evaluator_test_rubric.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/example.py
+-rw-rw-rw-   0 root         (0) root         (0)    12003 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/scoring/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     5750 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/audit/workflows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.310198 dyff-0.9.4/dyff/client/
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.312031 dyff-0.9.4/dyff/client/_generated/
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5959 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1940 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      733 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)    81146 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/_serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.312948 dyff-0.9.4/dyff/client/_generated/aio/
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6095 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/_client.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/_vendor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.313864 dyff-0.9.4/dyff/client/_generated/aio/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   498240 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/aio/operations/_patch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.314781 dyff-0.9.4/dyff/client/_generated/operations/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/operations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   532357 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/operations/_operations.py
+-rw-rw-rw-   0 root         (0) root         (0)      975 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/operations/_patch.py
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/_generated/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    52477 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/client/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.315698 dyff-0.9.4/dyff/core/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9981 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/core/config.py
+-rw-rw-rw-   0 root         (0) root         (0)      466 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/core/dynamic_import.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.316614 dyff-0.9.4/dyff/orchestrator/
+-rw-rw-rw-   0 root         (0) root         (0)      750 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10337 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/crd.py
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/gcloud-build.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.316614 dyff-0.9.4/dyff/orchestrator/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)      472 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/k8s/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2244 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/k8s/conditions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6781 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/k8s/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)    27735 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/orchestrator/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.320281 dyff-0.9.4/dyff/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     1012 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1056 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/copydoc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.321198 dyff-0.9.4/dyff/schema/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/dataset/vision.py
+-rw-rw-rw-   0 root         (0) root         (0)     1407 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/ids.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.321198 dyff-0.9.4/dyff/schema/io/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     3773 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/quantity.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)      100 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.322114 dyff-0.9.4/dyff/schema/v0/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.323031 dyff-0.9.4/dyff/schema/v0/r1/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    23542 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)    17115 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.323948 dyff-0.9.4/dyff/schema/v0/r1/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)     2530 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12317 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/arrow.py
+-rw-rw-rw-   0 root         (0) root         (0)      525 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/classification.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/text.py
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/dataset/vision.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.324864 dyff-0.9.4/dyff/schema/v0/r1/io/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/io/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5301 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/io/vllm.py
+-rw-rw-rw-   0 root         (0) root         (0)    44090 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/platform.py
+-rw-rw-rw-   0 root         (0) root         (0)     5878 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/requests.py
+-rw-rw-rw-   0 root         (0) root         (0)    10503 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/test.py
+-rw-rw-rw-   0 root         (0) root         (0)      344 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/v0/r1/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      353 2024-01-29 21:07:38.000000 dyff-0.9.4/dyff/schema/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.345947 dyff-0.9.4/dyff.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1955 2024-01-29 21:07:47.000000 dyff-0.9.4/dyff.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15081 2024-01-29 21:07:47.000000 dyff-0.9.4/dyff.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-01-29 21:07:47.000000 dyff-0.9.4/dyff.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-01-29 21:07:47.000000 dyff-0.9.4/dyff.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2024-01-29 21:07:47.000000 dyff-0.9.4/dyff.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.246948 dyff-0.9.4/gcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.325781 dyff-0.9.4/gcloud/build/
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/build/api-server-proxy.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      430 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/build/api-server.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      451 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/build/init-workload-identity.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      412 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/build/kafka-cli.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      421 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/build/orchestrator.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.325781 dyff-0.9.4/gcloud/datastore/
+-rw-rw-rw-   0 root         (0) root         (0)      583 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/datastore/index.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.326697 dyff-0.9.4/gcloud/k8s/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/k8s/keepalive.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/k8s/run-fetch-data.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/k8s/run-ingest-dataset.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1581 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/k8s/run-model-test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      327 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud/k8s/workload-identity-test.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-01-29 21:07:38.000000 dyff-0.9.4/gcloud-build.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.327614 dyff-0.9.4/ingest/
+-rw-rw-rw-   0 root         (0) root         (0)      824 2024-01-29 21:07:38.000000 dyff-0.9.4/ingest/imagenet-c.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2275 2024-01-29 21:07:38.000000 dyff-0.9.4/ingest/mnist-c.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-01-29 21:07:38.000000 dyff-0.9.4/ingest/test-imagenet-c.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.247865 dyff-0.9.4/k8s/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.329448 dyff-0.9.4/k8s/deploy/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/api-key-signing-secret-placeholder.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      758 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/api-server-ingress.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/api-server-issuer-letsencrypt.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      182 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/api-server-secret-placeholder.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/api-server.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      249 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/gitlab-pull-secret-placeholder.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.330364 dyff-0.9.4/k8s/deploy/kafka/
+-rw-rw-rw-   0 root         (0) root         (0)      246 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/kafka/cli.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2479 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/kafka/kafka.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.330364 dyff-0.9.4/k8s/deploy/kafka/topics/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/kafka/topics/dyff-workflows.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      611 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/kafka/topics/test-workflows.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.331281 dyff-0.9.4/k8s/deploy/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/mongodb/user-auth-backend.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      236 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/mongodb/user-query-backend.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      245 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/mongodb/user-workflows-sink.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2199 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/orchestrator.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.331281 dyff-0.9.4/k8s/deploy/test/
+-rw-rw-rw-   0 root         (0) root         (0)      413 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/test/api-server-issuer-letsencrypt.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      626 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/deploy/test/api-server-mock.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.331281 dyff-0.9.4/k8s/network/
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/network/audit.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.332198 dyff-0.9.4/k8s/rbac/
+-rw-rw-rw-   0 root         (0) root         (0)      574 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/rbac/api-server.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.332198 dyff-0.9.4/k8s/rbac/mongodb/
+-rw-rw-rw-   0 root         (0) root         (0)      589 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/rbac/mongodb/mongodb-admin.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2024-01-29 21:07:38.000000 dyff-0.9.4/k8s/rbac/orchestrator.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-01-29 21:07:38.000000 dyff-0.9.4/makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.332198 dyff-0.9.4/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.336781 dyff-0.9.4/mongodb/deploy/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.336781 dyff-0.9.4/mongodb/deploy/backup/
+-rw-rw-rw-   0 root         (0) root         (0)      254 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/backup/backup.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      625 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/backup/restore.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      210 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/backup-s3.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   883127 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/bundle.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/cr-minimal.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    17064 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/cr.yaml
+-rw-rw-rw-   0 root         (0) root         (0)   879266 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/crd.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.248782 dyff-0.9.4/mongodb/deploy/csv/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.337697 dyff-0.9.4/mongodb/deploy/csv/redhat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.248782 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.338614 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)    60108 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/percona-server-mongodb-operator.v1.4.0.clusterserviceversion.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1161 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      823 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      946 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.338614 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      418 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/metadata/annotations.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.249698 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.340448 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)    61754 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/percona-server-mongodb-operator.v1.5.0.clusterserviceversion.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.340448 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/metadata/annotations.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.249698 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.341364 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.249698 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.342281 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)    62912 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/percona-server-mongodb-operator.v1.6.0.clusterserviceversion.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.342281 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/metadata/annotations.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.250615 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.342281 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.250615 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.343197 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/
+-rw-rw-rw-   0 root         (0) root         (0)    63701 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/percona-server-mongodb-operator.v1.7.0.clusterserviceversion.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1147 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      809 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.343197 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/metadata/
+-rw-rw-rw-   0 root         (0) root         (0)      428 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/metadata/annotations.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.250615 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.343197 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/
+-rw-rw-rw-   0 root         (0) root         (0)      808 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.4.0.Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.5.0.Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.6.0.Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1065 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.7.0.Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)   883321 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/cw-bundle.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/cw-operator.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2785 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/cw-rbac.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/operator.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2516 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/rbac.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      633 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/secrets.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    12801 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/deploy/ssl-secrets.yaml
+-rwxrwxrwx   0 root         (0) root         (0)     1550 2024-01-29 21:07:38.000000 dyff-0.9.4/mongodb/fetch-deploy-files-from-upstream.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.344114 dyff-0.9.4/openapi/
+-rw-rw-rw-   0 root         (0) root         (0)   141284 2024-01-29 21:07:38.000000 dyff-0.9.4/openapi/dyff.json
+-rw-rw-rw-   0 root         (0) root         (0)      317 2024-01-29 21:07:38.000000 dyff-0.9.4/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)       53 2024-01-29 21:07:38.000000 dyff-0.9.4/package.json
+-rw-rw-rw-   0 root         (0) root         (0)     6292 2024-01-29 21:07:38.000000 dyff-0.9.4/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       76 2024-01-29 21:07:38.000000 dyff-0.9.4/requirements-orchestrator.in
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2024-01-29 21:07:38.000000 dyff-0.9.4/requirements-orchestrator.txt
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-01-29 21:07:38.000000 dyff-0.9.4/requirements.in
+-rw-rw-rw-   0 root         (0) root         (0)     7250 2024-01-29 21:07:38.000000 dyff-0.9.4/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.345031 dyff-0.9.4/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)     1288 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/create-gcs-bucket.py
+-rwxrwxrwx   0 root         (0) root         (0)     3366 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/fix-openapi.py
+-rwxrwxrwx   0 root         (0) root         (0)     7444 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/generate-config-listing.py
+-rwxrwxrwx   0 root         (0) root         (0)      569 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/generate-openapi-definitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.345031 dyff-0.9.4/scripts/inferenceservices/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/inferenceservices/databricks--dolly-v2-3b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/inferenceservices/tiiuae--falcon-7b--default.py
+-rw-rw-rw-   0 root         (0) root         (0)     2443 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/k8s-secret-data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.345947 dyff-0.9.4/scripts/models/
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/models/databricks--dolly-v2-3b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1355 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/models/databricks--dolly-v2-3b.py
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/models/tiiuae--falcon-7b--rox.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/models/tiiuae--falcon-7b.py
+-rw-rw-rw-   0 root         (0) root         (0)      725 2024-01-29 21:07:38.000000 dyff-0.9.4/scripts/rotate-api-key-signing-secret.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-01-29 21:07:47.346864 dyff-0.9.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      696 2024-01-29 21:07:38.000000 dyff-0.9.4/skaffold.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-29 21:07:47.345947 dyff-0.9.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      104 2024-01-29 21:07:38.000000 dyff-0.9.4/tests/test_nothing.py
```

### Comparing `dyff-0.9.3/.dockerignore` & `dyff-0.9.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/.gcloudignore` & `dyff-0.9.4/.gcloudignore`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/.gitignore` & `dyff-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/.gitlab-ci.yml` & `dyff-0.9.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/.pre-commit-config.yaml` & `dyff-0.9.4/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
           - "--in-place"
           - "--expand-star-imports"
           - "--remove-duplicate-keys"
           - "--remove-unused-variables"
           # - "--remove-all-unused-imports"
 
   - repo: https://github.com/psf/black
-    rev: 23.12.1
+    rev: 24.1.1
     hooks:
       - id: black
 
   - repo: https://github.com/PyCQA/isort
     rev: "5.13.2"
     hooks:
       - id: isort
```

### Comparing `dyff-0.9.3/CODE_OF_CONDUCT.md` & `dyff-0.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/Dockerfile` & `dyff-0.9.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/LICENSE` & `dyff-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/PKG-INFO` & `dyff-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Python client library for the Dyff AI auditing platform.
 Project-URL: Home, https://dyff.io
 Project-URL: Docs, https://docs.dyff.io
 Project-URL: Code, https://gitlab.com/dyff/dyff
 Project-URL: Issues, https://gitlab.com/dyff/dyff/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-0.9.3/README.client.md` & `dyff-0.9.4/README.client.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/README.md` & `dyff-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/dyff_admin/requirements.txt` & `dyff-0.9.4/apps/dyff_admin/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/evaluation_client/Dockerfile` & `dyff-0.9.4/apps/evaluation_client/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/evaluation_client/main.py` & `dyff-0.9.4/apps/evaluation_client/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -323,17 +323,17 @@
     async with aiohttp.ClientSession(
         connector=aiohttp.TCPConnector(force_close=True)
     ) as session:
         # Propagate input queue limits
         work_queue: asyncio.Queue[tuple[ItemID, DataItem]] = asyncio.Queue(
             in_queue.maxsize
         )
-        result_queue: asyncio.Queue[
-            tuple[ItemID, list[DataItem] | None]
-        ] = asyncio.Queue()
+        result_queue: asyncio.Queue[tuple[ItemID, list[DataItem] | None]] = (
+            asyncio.Queue()
+        )
         retry_manager = RetryManager()
         monitor = _Monitor()
         processed_indices: set[ItemID] = set()
 
         worker_tasks = []
         worker_tasks.append(asyncio.create_task(_copy_output(result_queue, out_queue)))
         worker_tasks.append(asyncio.create_task(monitor()))
@@ -381,15 +381,15 @@
         out_queue.put((None, None))  # sentinel
 
         logging.info(f"Monitor event totals: {monitor.totals}")
         if monitor.totals_for_event("input") != monitor.totals_for_event("output"):
             logging.error("Monitor: 'input' != 'output'")
         failures = retry_manager.failures()
         if len(failures) > 0:
-            logging.error(f"failed indices: {failures.keys()}")
+            logging.error(f"failed indices: {failures}")
 
 
 def _output_thread(
     *,
     out_queue: queue.Queue[tuple[ItemID | None, list[DataItem] | None]],
     output_path: str,
     output_schema: pyarrow.Schema,
@@ -436,28 +436,21 @@
                     result_batch, schema=output_schema
                 )
                 result_batch = []
         if len(result_batch) > 0:
             logging.info(f"finished batch {batch_idx} (final batch)")
             yield pyarrow.RecordBatch.from_pylist(result_batch, schema=output_schema)
 
-    # If these fields are present, we want to represent them as partitions
-    partition_keys = ["_replication_"]
-    partition_fields = []
-    for partition_key in partition_keys:
-        field_index = output_schema.get_field_index(partition_key)
-        if field_index != -1:
-            partition_fields.append(output_schema.field(field_index))
-    partition_schema = pyarrow.schema(partition_fields) if partition_fields else None
-
+    # Note: We don't partition the outputs because that undermines our goal of
+    # writing small chunks frequently to preserve progress. We can re-partition
+    # in verify_evaluation_output if desired.
     arrow.write_dataset(
         batch_generator(output_schema),
         output_path=output_path,
         feature_schema=output_schema,
-        partition_schema=partition_schema,
         # Force frequent writes so we don't lose progress
         max_rows_per_file=batch_size,
         # pyarrow.lib.ArrowInvalid: max_rows_per_group must be less than or equal to max_rows_per_file
         max_rows_per_group=batch_size,
         # Use UUIDs so that we never overwrite old data. On a restart, we read
         # all the data that's already persisted and skip those indices.
         basename_template=f"{uuid.uuid4()}.{{i}}.parquet",
@@ -586,17 +579,17 @@
     service_address = _inference_service_address(evaluation)
     service_url = f"{service_address}/{inference_endpoint}"
 
     # Limit input queue to avoid memory limits
     work_queue: queue.Queue[tuple[ItemID, DataItem] | None] = queue.Queue(
         maxsize=(4 * batch_size)
     )
-    result_queue: queue.Queue[
-        tuple[ItemID | None, list[DataItem] | None]
-    ] = queue.Queue()
+    result_queue: queue.Queue[tuple[ItemID | None, list[DataItem] | None]] = (
+        queue.Queue()
+    )
 
     logging.info("starting asyncio thread")
     asyncio_loop = asyncio.new_event_loop()
     async_thread = threading.Thread(
         target=_start_background_loop, args=(asyncio_loop,), daemon=True
     )
     async_thread.start()
```

### Comparing `dyff-0.9.3/apps/evaluation_client/requirements.txt` & `dyff-0.9.4/apps/evaluation_client/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/fetch_model/Dockerfile` & `dyff-0.9.4/apps/fetch_model/Dockerfile`

 * *Files 10% similar despite different names*

```diff
@@ -28,8 +28,8 @@
   && rm -rf /var/lib/apt/lists/*
 
 WORKDIR /fetch-model/
 
 COPY apps/fetch_model/ ./
 COPY dyff/ ./dyff/
 
-ENTRYPOINT [ "python3", "main.py" ]
+ENTRYPOINT [ "python3", "-m", "fetch_model" ]
```

### Comparing `dyff-0.9.3/apps/fetch_model/main.py` & `dyff-0.9.4/apps/fetch_model/fetch_model/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import absl.app
 import absl.flags
 import ruamel.yaml
 import smart_open
 from absl import logging
 
 from dyff.api import storage, timestamp
-from dyff.models.fetch import fetch
 from dyff.schema.platform import ModelSource
 
+from .fetch import fetch
+
 FLAGS = absl.flags.FLAGS
 
 absl.flags.DEFINE_string(
     "model_yaml", None, "Path to a YAML file containing the Model manifest."
 )
 absl.flags.mark_flag_as_required("model_yaml")
```

### Comparing `dyff-0.9.3/apps/fetch_model/requirements.txt` & `dyff-0.9.4/apps/fetch_model/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/mocks/inferenceservice/requirements.txt` & `dyff-0.9.4/apps/mocks/inferenceservice/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/mocks/inferenceservice/server.py` & `dyff-0.9.4/apps/mocks/inferenceservice/server.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/run_report/Dockerfile` & `dyff-0.9.4/apps/run_report/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/run_report/main.py` & `dyff-0.9.4/apps/run_report/main.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/run_report/requirements.txt` & `dyff-0.9.4/apps/run_report/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/runners/bentoml_service_openllm/requirements.txt` & `dyff-0.9.4/apps/runners/bentoml_service_openllm/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/runners/vllm/Dockerfile` & `dyff-0.9.4/apps/runners/vllm/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/runners/vllm/main.py` & `dyff-0.9.4/apps/runners/vllm/main.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/verify_evaluation_output/Dockerfile` & `dyff-0.9.4/apps/verify_evaluation_output/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/verify_evaluation_output/main.py` & `dyff-0.9.4/apps/verify_evaluation_output/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,24 +36,24 @@
 
 
 class ItemID(NamedTuple):
     replication: str
     item_index: int
 
 
-def verify_output(evaluation, *, repartition: bool = False) -> int:
+def verify_output(evaluation, *, repartition: bool) -> int:
     evaluation_id = evaluation["spec"]["id"]
     dataset = evaluation["spec"]["dataset"]
     replications: int = evaluation["spec"]["replications"]
 
     outputs_dataset = arrow.open_dataset(storage.paths.outputs_raw(evaluation_id))
     feature_schema = outputs_dataset.schema
     num_rows = outputs_dataset.count_rows()
     output_size = storage.storage_size(storage.paths.outputs_raw(evaluation_id))
-    size_MBi = output_size / (1024 * 1024)
+    size_MBi = output_size / (1000 * 1024)
     MBi_per_row = size_MBi / num_rows
     # Target is 100MBi per file
     n = 100.0 / MBi_per_row
     # Nice round number -- smallest power of 2 s.t. n * MBi_per_row >= 100
     rows_per_file = int(math.pow(2, math.ceil(math.log2(n))))
     logging.info(
         f"rows: {num_rows}; size (MBi): {size_MBi}; rows_per_file: {rows_per_file}"
@@ -77,19 +77,27 @@
         ids.replication_id(evaluation_id, i) for i in range(replications)
     ]
     input_items = []
     for index in input_indices:
         for replication in replication_ids:
             input_items.append(ItemID(replication=replication, item_index=index))
 
-    if repartition:
+    partition_keys = evaluation["spec"].get("outputDatasetPartitions")
+    if partition_keys:
+        # If these fields are present, we want to represent them as partitions
+        partition_fields = []
+        for partition_key in partition_keys:
+            field_index = feature_schema.get_field_index(partition_key)
+            if field_index != -1:
+                partition_fields.append(feature_schema.field(field_index))
         partition_schema = (
-            input_dataset.partitioning and input_dataset.partitioning.schema
+            pyarrow.schema(partition_fields) if partition_fields else None
         )
     else:
+        # Else keep the partitioning from the unverified outputs
         partition_schema = (
             outputs_dataset.partitioning and outputs_dataset.partitioning.schema
         )
     logging.info(f"feature_schema:\n{feature_schema}")
     logging.info(f"partition_schema:\n{partition_schema}")
 
     processed: list[ItemID] = []
@@ -145,12 +153,12 @@
     yaml = ruamel.yaml.YAML()
     with open(FLAGS.evaluation_yaml, "r") as fin:
         evaluation = yaml.load(fin)
     yaml_string = YAMLStringIO()
     yaml.dump(evaluation, yaml_string)
     logging.info(f"evaluation_yaml:\n{yaml_string.getvalue()}")
 
-    return verify_output(evaluation)
+    return verify_output(evaluation, repartition=True)
 
 
 if __name__ == "__main__":
     absl.app.run(main)
```

### Comparing `dyff-0.9.3/apps/verify_evaluation_output/requirements.txt` & `dyff-0.9.4/apps/verify_evaluation_output/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/Dockerfile` & `dyff-0.9.4/apps/workflows_informer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/agent/agent.go` & `dyff-0.9.4/apps/workflows_informer/agent/agent.go`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/go.mod` & `dyff-0.9.4/apps/workflows_informer/go.mod`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/go.sum` & `dyff-0.9.4/apps/workflows_informer/go.sum`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/k8s/deployment.yaml` & `dyff-0.9.4/apps/workflows_informer/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/k8s/rbac.yaml` & `dyff-0.9.4/apps/workflows_informer/k8s/rbac.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_informer/main.go` & `dyff-0.9.4/apps/workflows_informer/main.go`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_sink/Dockerfile` & `dyff-0.9.4/apps/workflows_sink/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_sink/k8s/deployment.yaml` & `dyff-0.9.4/apps/workflows_sink/k8s/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/apps/workflows_sink/workflows_sink/main.py` & `dyff-0.9.4/apps/workflows_sink/workflows_sink/main.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/README.md` & `dyff-0.9.4/charts/dyff/README.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/templates/_helpers.tpl` & `dyff-0.9.4/charts/dyff/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/templates/api/api-deployment.yaml` & `dyff-0.9.4/charts/dyff/templates/api/api-deployment.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/templates/api/api-hpa.yaml` & `dyff-0.9.4/charts/dyff/templates/api/api-hpa.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/templates/api/api-ingress.yaml` & `dyff-0.9.4/charts/dyff/templates/api/api-ingress.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/templates/orchestrator/orchestrator-statefulset.yaml` & `dyff-0.9.4/charts/dyff/templates/orchestrator/orchestrator-statefulset.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/charts/dyff/values.yaml` & `dyff-0.9.4/charts/dyff/values.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/admin.md` & `dyff-0.9.4/doc/internal/admin.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/api-server.md` & `dyff-0.9.4/doc/internal/api-server.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/audits.md` & `dyff-0.9.4/doc/internal/audits.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/data-schemas.md` & `dyff-0.9.4/doc/internal/data-schemas.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/evaluations.md` & `dyff-0.9.4/doc/internal/evaluations.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/gcloud-notes.md` & `dyff-0.9.4/doc/internal/gcloud-notes.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/go-operators.md` & `dyff-0.9.4/doc/internal/go-operators.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/kafkaesque.md` & `dyff-0.9.4/doc/internal/kafkaesque.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/models.md` & `dyff-0.9.4/doc/internal/models.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/mongodb.md` & `dyff-0.9.4/doc/internal/mongodb.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/operators.md` & `dyff-0.9.4/doc/internal/operators.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/roadmap.md` & `dyff-0.9.4/doc/internal/roadmap.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/doc/internal/user-facing-api.md` & `dyff-0.9.4/doc/internal/user-facing-api.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docker/Dockerfile-init-workload-identity` & `dyff-0.9.4/docker/Dockerfile-init-workload-identity`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docker/Dockerfile-kafka-cli` & `dyff-0.9.4/docker/Dockerfile-kafka-cli`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/_extensions/pyarrow_schema.py` & `dyff-0.9.4/docs/_extensions/pyarrow_schema.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/api-reference/audit.rst` & `dyff-0.9.4/docs/api-reference/audit.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/api-reference/client.rst` & `dyff-0.9.4/docs/api-reference/client.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/api-reference/models.rst` & `dyff-0.9.4/docs/api-reference/models.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/api-reference/schema.rst` & `dyff-0.9.4/docs/api-reference/schema.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/conf.py` & `dyff-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/deployment/architecture/storage.rst` & `dyff-0.9.4/docs/deployment/architecture/storage.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/deployment/configuration.rst` & `dyff-0.9.4/docs/deployment/configuration.rst`

 * *Files 1% similar despite different names*

```diff
@@ -297,14 +297,23 @@
 
 Type: ``string``
 
 Default: ``us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/bentoml-service-openllm-runner:latest``
 
 Environment variable: ``DYFF_ORCHESTRATOR__IMAGES__BENTOML_SERVICE_OPENLLM``
 
+orchestrator.images.huggingface
+```````````````````````````````
+
+Type: ``string``
+
+Default: ``us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/huggingface-runner:latest``
+
+Environment variable: ``DYFF_ORCHESTRATOR__IMAGES__HUGGINGFACE``
+
 orchestrator.images.mock
 ````````````````````````
 
 Type: ``string``
 
 Default: ``us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/inferenceservice-mock:latest``
```

### Comparing `dyff-0.9.3/docs/deployment/management.rst` & `dyff-0.9.4/docs/deployment/management.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/design.rst` & `dyff-0.9.4/docs/development/design.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/dyff-operator.rst` & `dyff-0.9.4/docs/development/dyff-operator.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/dyff-service-diagram.drawio` & `dyff-0.9.4/docs/development/dyff-service-diagram.drawio`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/dyff-service-diagram.pdf` & `dyff-0.9.4/docs/development/dyff-service-diagram.pdf`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/dyff-service-diagram.svg` & `dyff-0.9.4/docs/development/dyff-service-diagram.svg`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/evaluation.yaml` & `dyff-0.9.4/docs/development/evaluation.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/principles.rst` & `dyff-0.9.4/docs/development/principles.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/development/rbac.rst` & `dyff-0.9.4/docs/development/rbac.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/client/create-evaluation.py` & `dyff-0.9.4/docs/examples/client/create-evaluation.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/client/create-inferenceservice.py` & `dyff-0.9.4/docs/examples/client/create-inferenceservice.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/client/create-inferencesession.py` & `dyff-0.9.4/docs/examples/client/create-inferencesession.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/client/create-upload-dataset.py` & `dyff-0.9.4/docs/examples/client/create-upload-dataset.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/dataset.py` & `dyff-0.9.4/docs/examples/dataset.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/examples/simple-audit.ipynb` & `dyff-0.9.4/docs/examples/simple-audit.ipynb`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/index.rst` & `dyff-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/makefile` & `dyff-0.9.4/docs/makefile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/releases/0.5.0.rst` & `dyff-0.9.4/docs/releases/0.5.0.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/releases/0.6.0.rst` & `dyff-0.9.4/docs/releases/0.6.0.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/requirements.txt` & `dyff-0.9.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/tutorials/creating-a-dataset.rst` & `dyff-0.9.4/docs/tutorials/creating-a-dataset.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/tutorials/creating-an-audit.rst` & `dyff-0.9.4/docs/tutorials/creating-an-audit.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/user-guide/core-resources.rst` & `dyff-0.9.4/docs/user-guide/core-resources.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/user-guide/data-schemas.rst` & `dyff-0.9.4/docs/user-guide/data-schemas.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/user-guide/installation.rst` & `dyff-0.9.4/docs/user-guide/installation.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/docs/user-guide/resource-lifecycle.rst` & `dyff-0.9.4/docs/user-guide/resource-lifecycle.rst`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dotenv/mvp.env` & `dyff-0.9.4/dotenv/mvp.env`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/api.py` & `dyff-0.9.4/dyff/api/api.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/base/auth.py` & `dyff-0.9.4/dyff/api/backend/base/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/base/command.py` & `dyff-0.9.4/dyff/api/backend/base/command.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/base/query.py` & `dyff-0.9.4/dyff/api/backend/base/query.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/base/storage.py` & `dyff-0.9.4/dyff/api/backend/base/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/gcloud/storage.py` & `dyff-0.9.4/dyff/api/backend/gcloud/storage.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/kafka/command.py` & `dyff-0.9.4/dyff/api/backend/kafka/command.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/mock/command.py` & `dyff-0.9.4/dyff/api/backend/mock/command.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/mongodb/auth.py` & `dyff-0.9.4/dyff/api/backend/mongodb/auth.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/backend/mongodb/query.py` & `dyff-0.9.4/dyff/api/backend/mongodb/query.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/clone_audit_procedure.py` & `dyff-0.9.4/dyff/api/bin/clone_audit_procedure.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/fetch_data.py` & `dyff-0.9.4/dyff/api/bin/fetch_data.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/gcloud/build_bentoml_service.py` & `dyff-0.9.4/dyff/api/bin/gcloud/build_bentoml_service.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/gcloud/build_model_container.py` & `dyff-0.9.4/dyff/api/bin/gcloud/build_model_container.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/ingest_dataset.py` & `dyff-0.9.4/dyff/api/bin/ingest_dataset.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/run_audit.py` & `dyff-0.9.4/dyff/api/bin/run_audit.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/bin/run_jupyterbook.py` & `dyff-0.9.4/dyff/api/bin/run_jupyterbook.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/__init__.py` & `dyff-0.9.4/dyff/api/data/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/archives.py` & `dyff-0.9.4/dyff/api/data/archives.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/arrowtypes.py` & `dyff-0.9.4/dyff/api/data/arrowtypes.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/fetch.py` & `dyff-0.9.4/dyff/api/data/fetch.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/huggingface.py` & `dyff-0.9.4/dyff/api/data/huggingface.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/ingest.py` & `dyff-0.9.4/dyff/api/data/ingest.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/sinks.py` & `dyff-0.9.4/dyff/api/data/sinks.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/sources/zenodo.py` & `dyff-0.9.4/dyff/api/data/sources/zenodo.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/data/text.py` & `dyff-0.9.4/dyff/api/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/mgmt/__main__.py` & `dyff-0.9.4/dyff/api/mgmt/__main__.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/mgmt/accounts.py` & `dyff-0.9.4/dyff/api/mgmt/accounts.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/mgmt/tokens.py` & `dyff-0.9.4/dyff/api/mgmt/tokens.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/sanitize.py` & `dyff-0.9.4/dyff/api/sanitize.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/server.py` & `dyff-0.9.4/dyff/api/server.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/server_insecure.py` & `dyff-0.9.4/dyff/api/server_insecure.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 import warnings
 
 import fastapi
 
 from dyff.schema.platform import APIKey
 
-from . import api, tokens
+from . import api, tokens, web
 
 
 def _not_kubernetes() -> None:
     if os.environ.get("KUBERNETES_SERVICE_HOST"):
         raise fastapi.HTTPException(
             fastapi.status.HTTP_503_SERVICE_UNAVAILABLE,
             detail="Test configuration is not to be deployed!",
@@ -37,14 +37,15 @@
 
 
 app = fastapi.FastAPI(
     title="dyff",
 )
 # api.app.dependency_overrides[api.verify_api_token] = _not_kubernetes
 app.mount("/dyff/v0", api.app)
+app.mount("/web", web.app)
 # apps.site.app.dependency_overrides[apps.site.verify_api_token] = _not_kubernetes
 
 
 @app.get(f"/health")
 async def health() -> int:
     """Required health check for GKE Ingress. Should be specified in the
     k8s Deployment as a readinessProbe.
```

### Comparing `dyff-0.9.3/dyff/api/storage/__init__.py` & `dyff-0.9.4/dyff/api/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/storage/paths.py` & `dyff-0.9.4/dyff/api/storage/paths.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/timestamp.py` & `dyff-0.9.4/dyff/api/timestamp.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/api/tokens.py` & `dyff-0.9.4/dyff/api/tokens.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/data/text.py` & `dyff-0.9.4/dyff/audit/data/text.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/metrics/base.py` & `dyff-0.9.4/dyff/audit/metrics/base.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/metrics/text.py` & `dyff-0.9.4/dyff/audit/metrics/text.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/base.py` & `dyff-0.9.4/dyff/audit/scoring/base.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/classification.py` & `dyff-0.9.4/dyff/audit/scoring/classification.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/evaluator_code_syntax_rubrics.py` & `dyff-0.9.4/dyff/audit/scoring/evaluator_code_syntax_rubrics.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/evaluator_misinfo_commonclaims.py` & `dyff-0.9.4/dyff/audit/scoring/evaluator_misinfo_commonclaims.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/evaluator_test_rubric.py` & `dyff-0.9.4/dyff/audit/scoring/evaluator_test_rubric.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/example.py` & `dyff-0.9.4/dyff/audit/scoring/example.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/scoring/text.py` & `dyff-0.9.4/dyff/audit/scoring/text.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/audit/workflows.py` & `dyff-0.9.4/dyff/audit/workflows.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/client/_generated/__init__.py` & `dyff-0.9.4/dyff/client/_generated/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import DyffAPI
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `dyff-0.9.3/dyff/client/_generated/_client.py` & `dyff-0.9.4/dyff/client/_generated/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any
 
 from azure.core import PipelineClient
@@ -62,17 +62,19 @@
                 policies.ContentDecodePolicy(**kwargs),
                 self._config.redirect_policy,
                 self._config.retry_policy,
                 self._config.authentication_policy,
                 self._config.custom_hook_policy,
                 self._config.logging_policy,
                 policies.DistributedTracingPolicy(**kwargs),
-                policies.SensitiveHeaderCleanupPolicy(**kwargs)
-                if self._config.redirect_policy
-                else None,
+                (
+                    policies.SensitiveHeaderCleanupPolicy(**kwargs)
+                    if self._config.redirect_policy
+                    else None
+                ),
                 self._config.http_logging_policy,
             ]
         self._client: PipelineClient = PipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
```

### Comparing `dyff-0.9.3/dyff/client/_generated/_configuration.py` & `dyff-0.9.4/dyff/client/_generated/_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
```

### Comparing `dyff-0.9.3/dyff/client/_generated/_patch.py` & `dyff-0.9.4/dyff/client/_generated/_patch.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 
 
-__all__: list[
-    str
-] = []  # Add all objects you want publicly available to users at this package level
+__all__: list[str] = (
+    []
+)  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

### Comparing `dyff-0.9.3/dyff/client/_generated/_serialization.py` & `dyff-0.9.4/dyff/client/_generated/_serialization.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/client/_generated/_vendor.py` & `dyff-0.9.4/dyff/client/_generated/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/__init__.py` & `dyff-0.9.4/dyff/client/_generated/aio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._client import DyffAPI
 
 try:
     from ._patch import *  # pylint: disable=unused-wildcard-import
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/_client.py` & `dyff-0.9.4/dyff/client/_generated/aio/_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from copy import deepcopy
 from typing import Any, Awaitable
 
 from azure.core import AsyncPipelineClient
@@ -62,17 +62,19 @@
                 policies.ContentDecodePolicy(**kwargs),
                 self._config.redirect_policy,
                 self._config.retry_policy,
                 self._config.authentication_policy,
                 self._config.custom_hook_policy,
                 self._config.logging_policy,
                 policies.DistributedTracingPolicy(**kwargs),
-                policies.SensitiveHeaderCleanupPolicy(**kwargs)
-                if self._config.redirect_policy
-                else None,
+                (
+                    policies.SensitiveHeaderCleanupPolicy(**kwargs)
+                    if self._config.redirect_policy
+                    else None
+                ),
                 self._config.http_logging_policy,
             ]
         self._client: AsyncPipelineClient = AsyncPipelineClient(
             base_url=endpoint, policies=_policies, **kwargs
         )
 
         self._serialize = Serializer()
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/_configuration.py` & `dyff-0.9.4/dyff/client/_generated/aio/_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from typing import Any
 
 from azure.core.pipeline import policies
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/_patch.py` & `dyff-0.9.4/dyff/client/_generated/aio/_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 from typing import List
 
-__all__: List[
-    str
-] = []  # Add all objects you want publicly available to users at this package level
+__all__: List[str] = (
+    []
+)  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/_vendor.py` & `dyff-0.9.4/dyff/client/_generated/aio/_vendor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 
 def raise_if_not_implemented(cls, abstract_methods):
     not_implemented = [
         f for f in abstract_methods if not callable(getattr(cls, f, None))
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/operations/__init__.py` & `dyff-0.9.4/dyff/client/_generated/aio/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/operations/_operations.py` & `dyff-0.9.4/dyff/client/_generated/aio/operations/_operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
@@ -2796,16 +2796,16 @@
                                                   Must be encodable as JSON.
                                             }
                                         ]
                                     }
                                 ],
                                 "runner": {
                                     "kind": "str",  # An enumeration. Required.
-                                      Known values are: "bentoml_service_openllm", "mock",
-                                      "standalone", and "vllm".
+                                      Known values are: "bentoml_service_openllm", "huggingface",
+                                      "mock", "standalone", and "vllm".
                                     "resources": {
                                         "storage": "str",  # Amount of
                                           storage required for packaged model, in k8s Quantity
                                           notation. Required.
                                         "memory": "str"  # Optional. Amount
                                           of memory required to run the model on CPU, in k8s Quantity
                                           notation.
@@ -3133,16 +3133,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -3366,16 +3366,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -3633,16 +3633,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -3927,16 +3927,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -4574,15 +4574,16 @@
                                 ]
                             }
                         ],
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "runner": {
                             "kind": "str",  # An enumeration. Required. Known values are:
-                              "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                              "bentoml_service_openllm", "huggingface", "mock", "standalone", and
+                              "vllm".
                             "resources": {
                                 "storage": "str",  # Amount of storage required for
                                   packaged model, in k8s Quantity notation. Required.
                                 "memory": "str"  # Optional. Amount of memory
                                   required to run the model on CPU, in k8s Quantity notation.
                             },
                             "accelerator": {
@@ -4780,15 +4781,15 @@
                                       Configuration for the schema adapter. Must be encodable as JSON.
                                 }
                             ]
                         }
                     ],
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -4934,15 +4935,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -5123,15 +5124,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -5265,15 +5266,15 @@
                                       Configuration for the schema adapter. Must be encodable as JSON.
                                 }
                             ]
                         }
                     ],
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -5419,15 +5420,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -5669,15 +5670,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6248,16 +6249,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -6567,16 +6568,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -6799,16 +6800,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -7055,16 +7056,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -7339,15 +7340,16 @@
                                           JSON.
                                     }
                                 ]
                             }
                         ],
                         "runner": {
                             "kind": "str",  # An enumeration. Required. Known values are:
-                              "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                              "bentoml_service_openllm", "huggingface", "mock", "standalone", and
+                              "vllm".
                             "resources": {
                                 "storage": "str",  # Amount of storage required for
                                   packaged model, in k8s Quantity notation. Required.
                                 "memory": "str"  # Optional. Amount of memory
                                   required to run the model on CPU, in k8s Quantity notation.
                             },
                             "accelerator": {
```

### Comparing `dyff-0.9.3/dyff/client/_generated/aio/operations/_patch.py` & `dyff-0.9.4/dyff/client/_generated/aio/operations/_patch.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 # ------------------------------------
 """Customize generated code here.
 
 Follow our quickstart for examples: https://aka.ms/azsdk/python/dpcodegen/python/customize
 """
 from typing import List
 
-__all__: List[
-    str
-] = []  # Add all objects you want publicly available to users at this package level
+__all__: List[str] = (
+    []
+)  # Add all objects you want publicly available to users at this package level
 
 
 def patch_sdk():
     """Do not remove from this file.
 
     `patch_sdk` is a last resort escape hatch that allows you to do customizations
     you can't accomplish using the techniques described in
```

### Comparing `dyff-0.9.3/dyff/client/_generated/operations/__init__.py` & `dyff-0.9.4/dyff/client/_generated/operations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 
 from ._operations import (
     AuditproceduresOperations,
     AuditsOperations,
     DatasetsOperations,
```

### Comparing `dyff-0.9.3/dyff/client/_generated/operations/_operations.py` & `dyff-0.9.4/dyff/client/_generated/operations/_operations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # pylint: disable=too-many-lines,too-many-statements
 # coding=utf-8
 # --------------------------------------------------------------------------
-# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.11.1)
+# Code generated by Microsoft (R) AutoRest Code Generator (autorest: 3.9.7, generator: @autorest/python@6.12.3)
 # Changes may cause incorrect behavior and will be lost if the code is regenerated.
 # --------------------------------------------------------------------------
 import sys
 from io import IOBase
 from typing import (
     IO,
     Any,
@@ -3866,16 +3866,16 @@
                                                   Must be encodable as JSON.
                                             }
                                         ]
                                     }
                                 ],
                                 "runner": {
                                     "kind": "str",  # An enumeration. Required.
-                                      Known values are: "bentoml_service_openllm", "mock",
-                                      "standalone", and "vllm".
+                                      Known values are: "bentoml_service_openllm", "huggingface",
+                                      "mock", "standalone", and "vllm".
                                     "resources": {
                                         "storage": "str",  # Amount of
                                           storage required for packaged model, in k8s Quantity
                                           notation. Required.
                                         "memory": "str"  # Optional. Amount
                                           of memory required to run the model on CPU, in k8s Quantity
                                           notation.
@@ -4203,16 +4203,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -4436,16 +4436,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -4703,16 +4703,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -4997,16 +4997,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -5644,15 +5644,16 @@
                                 ]
                             }
                         ],
                         "reason": "str",  # Optional. Reason for current status (assigned by
                           system).
                         "runner": {
                             "kind": "str",  # An enumeration. Required. Known values are:
-                              "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                              "bentoml_service_openllm", "huggingface", "mock", "standalone", and
+                              "vllm".
                             "resources": {
                                 "storage": "str",  # Amount of storage required for
                                   packaged model, in k8s Quantity notation. Required.
                                 "memory": "str"  # Optional. Amount of memory
                                   required to run the model on CPU, in k8s Quantity notation.
                             },
                             "accelerator": {
@@ -5850,15 +5851,15 @@
                                       Configuration for the schema adapter. Must be encodable as JSON.
                                 }
                             ]
                         }
                     ],
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6004,15 +6005,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6193,15 +6194,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6335,15 +6336,15 @@
                                       Configuration for the schema adapter. Must be encodable as JSON.
                                 }
                             ]
                         }
                     ],
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6489,15 +6490,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -6739,15 +6740,15 @@
                                 }
                             ]
                         }
                     ],
                     "reason": "str",  # Optional. Reason for current status (assigned by system).
                     "runner": {
                         "kind": "str",  # An enumeration. Required. Known values are:
-                          "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                          "bentoml_service_openllm", "huggingface", "mock", "standalone", and "vllm".
                         "resources": {
                             "storage": "str",  # Amount of storage required for packaged
                               model, in k8s Quantity notation. Required.
                             "memory": "str"  # Optional. Amount of memory required to run
                               the model on CPU, in k8s Quantity notation.
                         },
                         "accelerator": {
@@ -7318,16 +7319,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -7637,16 +7638,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -7869,16 +7870,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -8125,16 +8126,16 @@
                                               encodable as JSON.
                                         }
                                     ]
                                 }
                             ],
                             "runner": {
                                 "kind": "str",  # An enumeration. Required. Known
-                                  values are: "bentoml_service_openllm", "mock", "standalone", and
-                                  "vllm".
+                                  values are: "bentoml_service_openllm", "huggingface", "mock",
+                                  "standalone", and "vllm".
                                 "resources": {
                                     "storage": "str",  # Amount of storage
                                       required for packaged model, in k8s Quantity notation. Required.
                                     "memory": "str"  # Optional. Amount of memory
                                       required to run the model on CPU, in k8s Quantity notation.
                                 },
                                 "accelerator": {
@@ -8409,15 +8410,16 @@
                                           JSON.
                                     }
                                 ]
                             }
                         ],
                         "runner": {
                             "kind": "str",  # An enumeration. Required. Known values are:
-                              "bentoml_service_openllm", "mock", "standalone", and "vllm".
+                              "bentoml_service_openllm", "huggingface", "mock", "standalone", and
+                              "vllm".
                             "resources": {
                                 "storage": "str",  # Amount of storage required for
                                   packaged model, in k8s Quantity notation. Required.
                                 "memory": "str"  # Optional. Amount of memory
                                   required to run the model on CPU, in k8s Quantity notation.
                             },
                             "accelerator": {
```

### Comparing `dyff-0.9.3/dyff/client/_generated/operations/_patch.py` & `dyff-0.9.4/dyff/client/_generated/operations/_patch.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/client/client.py` & `dyff-0.9.4/dyff/client/client.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/core/config.py` & `dyff-0.9.4/dyff/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,20 +166,29 @@
 class KubernetesConfig(BaseModel):
     workflows_namespace: str = Field(
         default="default",
     )
 
 
 class OrchestratorImageTemplates(BaseModel):
-    bentoml_service_openllm: str = "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/bentoml-service-openllm-runner:latest"
-    mock: str = "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/inferenceservice-mock:latest"
+    bentoml_service_openllm: str = (
+        "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/bentoml-service-openllm-runner:latest"
+    )
+    huggingface: str = (
+        "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/huggingface-runner:latest"
+    )
+    mock: str = (
+        "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/inferenceservice-mock:latest"
+    )
     standalone: str = (
         "us-central1-docker.pkg.dev/dyff-354017/dyff-models/{service.id}:latest"
     )
-    vllm: str = "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/vllm-runner:latest"
+    vllm: str = (
+        "us-central1-docker.pkg.dev/dyff-354017/dyff-system/ul-dsri/dyff/dyff/vllm-runner:latest"
+    )
 
 
 # class ImagePullSecret(BaseModel):
 #     name: str
 
 
 class OrchestratorConfig(BaseModel):
```

### Comparing `dyff-0.9.3/dyff/models/fetch.py` & `dyff-0.9.4/apps/fetch_model/fetch_model/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
-from ..schema.platform import ModelSource, ModelSourceKinds
+from dyff.schema.platform import ModelSource, ModelSourceKinds
 
 
 def fetch(local_path: str, source: ModelSource):
     if source.kind == ModelSourceKinds.GitLFS:
         if source.gitLFS is None:
             raise ValueError("gitLFS not specified")
         from .sources import git_lfs
```

### Comparing `dyff-0.9.3/dyff/models/sources/git_lfs.py` & `dyff-0.9.4/apps/fetch_model/fetch_model/sources/git_lfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
 import subprocess
 
-from ...schema.platform import ModelSourceGitLFS
+from dyff.schema.platform import ModelSourceGitLFS
 
 
 def fetch(local_path: str, spec: ModelSourceGitLFS):
     print(f"cloning: {spec.url}")
     subprocess.run(["git", "clone", spec.url, local_path], check=True)
     # TODO: Only download the "preferred" format of the model weights
     # (HF repos can have multiple copies for different frameworks)
```

### Comparing `dyff-0.9.3/dyff/models/sources/huggingface_hub.py` & `dyff-0.9.4/apps/fetch_model/fetch_model/sources/huggingface_hub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright UL Research Institutes
 # SPDX-License-Identifier: Apache-2.0
 
-from ...schema.platform import ModelSourceHuggingFaceHub
+from dyff.schema.platform import ModelSourceHuggingFaceHub
 
 
 def _impl(local_path: str, spec: ModelSourceHuggingFaceHub):
     import os
 
     import transformers.utils.hub  # type: ignore[import-untyped]
     from huggingface_hub import snapshot_download  # type: ignore[import-untyped]
@@ -18,14 +18,15 @@
     snapshot_download(
         spec.repoID,
         repo_type="model",
         revision=spec.revision,
         cache_dir=local_path,
         allow_patterns=spec.allowPatterns,
         ignore_patterns=spec.ignorePatterns,
+        token=os.environ.get("DYFF_MODELS__HUGGINGFACE_ACCESS_TOKEN"),
     )
 
     print("migrating cache")
     transformers.utils.hub.move_cache(local_path, local_path)
 
 
 def fetch(local_path: str, spec: ModelSourceHuggingFaceHub):
```

### Comparing `dyff-0.9.3/dyff/models/sources/open_llm.py` & `dyff-0.9.4/apps/fetch_model/fetch_model/sources/open_llm.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 import pathlib
 import string
 import subprocess
 
 import ruamel.yaml as yaml
 
-from ...schema.platform import ModelSourceOpenLLM
+from dyff.schema.platform import ModelSourceOpenLLM
 
 
 def fetch(local_path: str, spec: ModelSourceOpenLLM):
     cmd = [
         "openllm",
         "build",
         spec.modelKind,
```

### Comparing `dyff-0.9.3/dyff/orchestrator/Dockerfile` & `dyff-0.9.4/dyff/orchestrator/Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/orchestrator/crd.py` & `dyff-0.9.4/dyff/orchestrator/crd.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,62 +128,70 @@
     if service.runner.kind == InferenceServiceRunnerKind.STANDALONE:
         spec["image"] = config.orchestrator.images.standalone.format(service=service)
     elif service.runner.kind == InferenceServiceRunnerKind.MOCK:
         spec["image"] = config.orchestrator.images.mock
     elif service.runner.kind == InferenceServiceRunnerKind.BENTOML_SERVICE_OPENLLM:
         # TODO: Probably just remove this Kind
         raise NotImplementedError()
-    elif service.runner.kind == InferenceServiceRunnerKind.VLLM:
+    elif service.runner.kind in [
+        InferenceServiceRunnerKind.HUGGINGFACE,
+        InferenceServiceRunnerKind.VLLM,
+    ]:
+        # Runners for HuggingFace models
         if service.model is None:
-            raise ValueError("vLLM runner requires service.model")
+            raise ValueError(f"runner {service.runner.kind}: service.model is required")
         if service.model.artifact.kind != ModelArtifactKind.HuggingFaceCache:
             raise ValueError(
-                f"service.model.artifact.kind must be {ModelArtifactKind.HuggingFaceCache}"
+                f"runner {service.runner.kind}:"
+                f" service.model.artifact.kind must be {ModelArtifactKind.HuggingFaceCache}"
             )
         hf_cache_artifact = service.model.artifact.huggingFaceCache
         assert hf_cache_artifact is not None
 
-        spec["image"] = config.orchestrator.images.vllm
-        spec["args"] = [
-            "--model",
-            f"{model_mount_path}/{hf_cache_artifact.snapshot_path()}",
-            "--download-dir",
-            model_mount_path,
-        ]
+        if service.runner.kind == InferenceServiceRunnerKind.HUGGINGFACE:
+            spec["image"] = config.orchestrator.images.huggingface
+            spec["args"] = [
+                "--model_name",
+                hf_cache_artifact.repoID,
+                "--model_revision",
+                hf_cache_artifact.revision,
+            ]
+        elif service.runner.kind == InferenceServiceRunnerKind.VLLM:
+            spec["image"] = config.orchestrator.images.vllm
+            spec["args"] = [
+                "--model",
+                f"{model_mount_path}/{hf_cache_artifact.snapshot_path()}",
+                "--download-dir",
+                model_mount_path,
+            ]
+        else:
+            raise AssertionError(f"Unexpected runner: {service.runner.kind}")
+
         if service.runner.args:
             spec["args"].extend(service.runner.args)
+        # Some of these are allegedly redundant, but I don't trust HF not
+        # to break things
         spec["env"] = [
             {"name": "HF_DATASETS_OFFLINE", "value": "1"},
             {"name": "HF_HOME", "value": model_mount_path},
             {"name": "HUGGINGFACE_HUB_CACHE", "value": model_mount_path},
             {"name": "TRANSFORMERS_CACHE", "value": model_mount_path},
             {"name": "TRANSFORMERS_OFFLINE", "value": "1"},
+            {"name": "HF_MODULES_CACHE", "value": "/tmp/hf_modules"},
+        ]
+        spec["dependencies"] = [
+            {
+                "kind": "ReadOnlyVolume",
+                "readOnlyVolume": {
+                    "name": "model",
+                    "claimName": f"model-{service.model.id}-rox",
+                    "mountPath": model_mount_path,
+                },
+            }
         ]
-        if service.model is not None:
-            spec["dependencies"] = [
-                {
-                    "kind": "ReadOnlyVolume",
-                    "readOnlyVolume": {
-                        "name": "model",
-                        "claimName": f"model-{service.model.id}-rox",
-                        "mountPath": model_mount_path,
-                    },
-                }
-            ]
-        else:
-            spec["dependencies"] = [
-                {
-                    "kind": "EphemeralVolume",
-                    "ephemeralVolume": {
-                        "name": "model",
-                        "mountPath": model_mount_path,
-                        "storage": service.runner.resources.storage,
-                    },
-                }
-            ]
     else:
         raise NotImplementedError(f"service.runner.kind {service.runner.kind}")
 
     session_resources = {
         # defaults
         "requests": {
             "memory": "4Gi",
```

### Comparing `dyff-0.9.3/dyff/orchestrator/k8s/conditions.py` & `dyff-0.9.4/dyff/orchestrator/k8s/conditions.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/orchestrator/k8s/resources.py` & `dyff-0.9.4/dyff/orchestrator/k8s/resources.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/orchestrator/main.py` & `dyff-0.9.4/dyff/orchestrator/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
     def create_k8s_workflow(self, entity: DyffEntityType) -> Optional[YAMLObject]:
         try:
             manifest = crd.manifest(entity)
             if manifest is not None:
                 return self._admit_entity(entity, manifest)
             else:
-                logging.info(f"Nothing to do for {entity.kind} {entity.id}")
+                logging.debug(f"Nothing to do for {entity.kind} {entity.id}")
                 if isinstance(entity, Dataset):
                     # No status change: user needs to upload data to and then
                     # manually indicate Ready
                     return None
                 else:
                     return {"status": EntityStatus.ready, "reason": None}
         except Exception:
@@ -563,17 +563,17 @@
                     self.delete_k8s_workflow(entity)
                 except kubernetes.client.exceptions.ApiException as ex:
                     # NotFound is OK because we might have a duplicate message
                     # or a user might delete the entity after the k8s resource
                     # has been GC'd.
                     if ex.status != 404:
                         raise
-            changed_dependents: List[
-                DyffEntityType
-            ] = self.dependency_graph.on_workflow_termination(self.db, entity)
+            changed_dependents: List[DyffEntityType] = (
+                self.dependency_graph.on_workflow_termination(self.db, entity)
+            )
             for e in changed_dependents:
                 self.produce_event(e.id, {"status": e.status, "reason": e.reason})
                 write_batch.put_entity(e.id, e)
             write_batch.put_dependency_graph(self.dependency_graph)
 
         # Store state change in local DB
         write_batch.put_entity(entity.id, entity)
```

### Comparing `dyff-0.9.3/dyff/schema/__init__.py` & `dyff-0.9.4/dyff/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/copydoc.py` & `dyff-0.9.4/dyff/schema/copydoc.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/ids.py` & `dyff-0.9.4/dyff/schema/ids.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/quantity.py` & `dyff-0.9.4/dyff/schema/quantity.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/adapters.py` & `dyff-0.9.4/dyff/schema/v0/r1/adapters.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/base.py` & `dyff-0.9.4/dyff/schema/v0/r1/base.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/dataset/__init__.py` & `dyff-0.9.4/dyff/schema/v0/r1/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/dataset/arrow.py` & `dyff-0.9.4/dyff/schema/v0/r1/dataset/arrow.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/dataset/binary.py` & `dyff-0.9.4/dyff/schema/v0/r1/dataset/binary.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/dataset/text.py` & `dyff-0.9.4/dyff/schema/v0/r1/dataset/text.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/io/vllm.py` & `dyff-0.9.4/dyff/schema/v0/r1/io/vllm.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/platform.py` & `dyff-0.9.4/dyff/schema/v0/r1/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -853,14 +853,15 @@
 class InferenceServiceBuilder(DyffSchemaBaseModel):
     kind: str
     args: Optional[list[str]] = None
 
 
 class InferenceServiceRunnerKind(str, Enum):
     BENTOML_SERVICE_OPENLLM = "bentoml_service_openllm"
+    HUGGINGFACE = "huggingface"
     MOCK = "mock"
     STANDALONE = "standalone"
     VLLM = "vllm"
 
 
 class InferenceServiceRunner(DyffSchemaBaseModel):
     kind: InferenceServiceRunnerKind
```

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/requests.py` & `dyff-0.9.4/dyff/schema/v0/r1/requests.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff/schema/v0/r1/test.py` & `dyff-0.9.4/dyff/schema/v0/r1/test.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/dyff.egg-info/PKG-INFO` & `dyff-0.9.4/dyff.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dyff
-Version: 0.9.3
+Version: 0.9.4
 Summary: The Python client library for the Dyff AI auditing platform.
 Project-URL: Home, https://dyff.io
 Project-URL: Docs, https://docs.dyff.io
 Project-URL: Code, https://gitlab.com/dyff/dyff
 Project-URL: Issues, https://gitlab.com/dyff/dyff/-/issues
 Keywords: ai,audit,safety,evaluation
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dyff-0.9.3/dyff.egg-info/SOURCES.txt` & `dyff-0.9.4/dyff.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 .helmignore
 .licenserc.yaml
 .pre-commit-config.yaml
 .prettierignore
 .python-version
 CODE_OF_CONDUCT.md
 Dockerfile
+Dockerfile-api-server-insecure
 LICENSE
 NOTICE
 README.client.md
 README.md
 gcloud-build.yaml
 makefile
 package-lock.json
@@ -33,19 +34,24 @@
 apps/evaluation_client/Dockerfile
 apps/evaluation_client/__init__.py
 apps/evaluation_client/gcloud-build.yaml
 apps/evaluation_client/main.py
 apps/evaluation_client/requirements.in
 apps/evaluation_client/requirements.txt
 apps/fetch_model/Dockerfile
-apps/fetch_model/__init__.py
 apps/fetch_model/gcloud-build.yaml
-apps/fetch_model/main.py
 apps/fetch_model/requirements.in
 apps/fetch_model/requirements.txt
+apps/fetch_model/fetch_model/__init__.py
+apps/fetch_model/fetch_model/__main__.py
+apps/fetch_model/fetch_model/fetch.py
+apps/fetch_model/fetch_model/sources/__init__.py
+apps/fetch_model/fetch_model/sources/git_lfs.py
+apps/fetch_model/fetch_model/sources/huggingface_hub.py
+apps/fetch_model/fetch_model/sources/open_llm.py
 apps/mocks/__init__.py
 apps/mocks/inferenceservice/Dockerfile
 apps/mocks/inferenceservice/__init__.py
 apps/mocks/inferenceservice/gcloud-build.yaml
 apps/mocks/inferenceservice/requirements.in
 apps/mocks/inferenceservice/requirements.txt
 apps/mocks/inferenceservice/server.py
@@ -57,14 +63,19 @@
 apps/run_report/requirements.txt
 apps/runners/__init__.py
 apps/runners/bentoml_service_openllm/Dockerfile
 apps/runners/bentoml_service_openllm/__init__.py
 apps/runners/bentoml_service_openllm/gcloud-build.yaml
 apps/runners/bentoml_service_openllm/requirements.in
 apps/runners/bentoml_service_openllm/requirements.txt
+apps/runners/huggingface/Dockerfile
+apps/runners/huggingface/__init__.py
+apps/runners/huggingface/gcloud-build.yaml
+apps/runners/huggingface/main.py
+apps/runners/huggingface/requirements.txt
 apps/runners/vllm/Dockerfile
 apps/runners/vllm/__init__.py
 apps/runners/vllm/gcloud-build.yaml
 apps/runners/vllm/main.py
 apps/runners/vllm/requirements.txt
 apps/verify_evaluation_output/Dockerfile
 apps/verify_evaluation_output/__init__.py
@@ -195,14 +206,15 @@
 dyff/api/exceptions.py
 dyff/api/sanitize.py
 dyff/api/server.py
 dyff/api/server_insecure.py
 dyff/api/timestamp.py
 dyff/api/tokens.py
 dyff/api/typing.py
+dyff/api/web.py
 dyff/api/backend/__init__.py
 dyff/api/backend/base/__init__.py
 dyff/api/backend/base/auth.py
 dyff/api/backend/base/command.py
 dyff/api/backend/base/query.py
 dyff/api/backend/base/storage.py
 dyff/api/backend/gcloud/__init__.py
@@ -246,14 +258,15 @@
 dyff/audit/metrics/text.py
 dyff/audit/schemas/__init__.py
 dyff/audit/scoring/__init__.py
 dyff/audit/scoring/base.py
 dyff/audit/scoring/classification.py
 dyff/audit/scoring/evaluator_code_syntax_rubrics.py
 dyff/audit/scoring/evaluator_misinfo_commonclaims.py
+dyff/audit/scoring/evaluator_personas.py
 dyff/audit/scoring/evaluator_test_rubric.py
 dyff/audit/scoring/example.py
 dyff/audit/scoring/text.py
 dyff/client/__init__.py
 dyff/client/client.py
 dyff/client/_generated/__init__.py
 dyff/client/_generated/_client.py
@@ -272,29 +285,14 @@
 dyff/client/_generated/aio/operations/_patch.py
 dyff/client/_generated/operations/__init__.py
 dyff/client/_generated/operations/_operations.py
 dyff/client/_generated/operations/_patch.py
 dyff/core/__init__.py
 dyff/core/config.py
 dyff/core/dynamic_import.py
-dyff/models/__init__.py
-dyff/models/api.py
-dyff/models/fetch.py
-dyff/models/bentoml/__init__.py
-dyff/models/bentoml/service.py-template
-dyff/models/bentoml/template_openllm_service.py
-dyff/models/frameworks/__init__.py
-dyff/models/frameworks/transformers.py
-dyff/models/outputs/__init__.py
-dyff/models/outputs/classification.py
-dyff/models/outputs/text.py
-dyff/models/sources/__init__.py
-dyff/models/sources/git_lfs.py
-dyff/models/sources/huggingface_hub.py
-dyff/models/sources/open_llm.py
 dyff/orchestrator/Dockerfile
 dyff/orchestrator/__init__.py
 dyff/orchestrator/__main__.py
 dyff/orchestrator/crd.py
 dyff/orchestrator/gcloud-build.yaml
 dyff/orchestrator/main.py
 dyff/orchestrator/k8s/__init__.py
```

### Comparing `dyff-0.9.3/gcloud/datastore/index.yaml` & `dyff-0.9.4/gcloud/datastore/index.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/gcloud/k8s/run-fetch-data.yaml` & `dyff-0.9.4/gcloud/k8s/run-fetch-data.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/gcloud/k8s/run-ingest-dataset.yaml` & `dyff-0.9.4/gcloud/k8s/run-ingest-dataset.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/gcloud/k8s/run-model-test.yaml` & `dyff-0.9.4/gcloud/k8s/run-model-test.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/ingest/imagenet-c.yaml` & `dyff-0.9.4/ingest/imagenet-c.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/ingest/mnist-c.yaml` & `dyff-0.9.4/ingest/mnist-c.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/ingest/test-imagenet-c.yaml` & `dyff-0.9.4/ingest/test-imagenet-c.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/api-server-ingress.yaml` & `dyff-0.9.4/k8s/deploy/api-server-ingress.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/api-server.yaml` & `dyff-0.9.4/k8s/deploy/api-server.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/kafka/kafka.yaml` & `dyff-0.9.4/k8s/deploy/kafka/kafka.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/kafka/topics/dyff-workflows.yaml` & `dyff-0.9.4/k8s/deploy/kafka/topics/dyff-workflows.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/kafka/topics/test-workflows.yaml` & `dyff-0.9.4/k8s/deploy/kafka/topics/test-workflows.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/orchestrator.yaml` & `dyff-0.9.4/k8s/deploy/orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/deploy/test/api-server-mock.yaml` & `dyff-0.9.4/k8s/deploy/test/api-server-mock.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/network/audit.yaml` & `dyff-0.9.4/k8s/network/audit.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/rbac/api-server.yaml` & `dyff-0.9.4/k8s/rbac/api-server.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/rbac/mongodb/mongodb-admin.yaml` & `dyff-0.9.4/k8s/rbac/mongodb/mongodb-admin.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/k8s/rbac/orchestrator.yaml` & `dyff-0.9.4/k8s/rbac/orchestrator.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/makefile` & `dyff-0.9.4/makefile`

 * *Files 11% similar despite different names*

```diff
@@ -105,7 +105,15 @@
 .PHONY: orchestrator-run
 orchestrator-run:
 	$(DOCKER) run --rm -it -t $(ORCHESTRATOR_IMAGE) .
 
 .PHONY: config-listing
 config-listing:
 	PYTHONPATH=$(shell pwd) $(PYTHON) ./scripts/generate-config-listing.py > docs/deployment/configuration.rst
+
+.PHONY: local-server-insecure-build
+local-server-insecure-build:
+	$(DOCKER) build -f Dockerfile-api-server-insecure -t dyff/api-server-insecure:local .
+
+.PHONE: local-server-insecure-run
+local-server-insecure-run:
+	$(DOCKER) run -p 8000:8000 dyff/api-server-insecure:local
```

### Comparing `dyff-0.9.3/mongodb/deploy/backup/restore.yaml` & `dyff-0.9.4/mongodb/deploy/backup/restore.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/bundle.yaml` & `dyff-0.9.4/mongodb/deploy/bundle.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/cr-minimal.yaml` & `dyff-0.9.4/mongodb/deploy/cr-minimal.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/cr.yaml` & `dyff-0.9.4/mongodb/deploy/cr.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/crd.yaml` & `dyff-0.9.4/mongodb/deploy/crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/percona-server-mongodb-operator.v1.4.0.clusterserviceversion.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/percona-server-mongodb-operator.v1.4.0.clusterserviceversion.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.4.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/percona-server-mongodb-operator.v1.5.0.clusterserviceversion.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/percona-server-mongodb-operator.v1.5.0.clusterserviceversion.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/config.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.5.0/tests/scorecard/config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/percona-server-mongodb-operator.v1.6.0.clusterserviceversion.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/percona-server-mongodb-operator.v1.6.0.clusterserviceversion.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/config.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.6.0/tests/scorecard/config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/percona-server-mongodb-operator.v1.7.0.clusterserviceversion.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/percona-server-mongodb-operator.v1.7.0.clusterserviceversion.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbbackups.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbrestores.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/manifests/perconaservermongodbs.psmdb.percona.com.crd.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/config.yaml` & `dyff-0.9.4/mongodb/deploy/csv/redhat/1.7.0/tests/scorecard/config.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/README.md` & `dyff-0.9.4/mongodb/deploy/csv/redhat/README.md`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.4.0.Dockerfile` & `dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.4.0.Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.5.0.Dockerfile` & `dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.5.0.Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.6.0.Dockerfile` & `dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.6.0.Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/csv/redhat/bundle-1.7.0.Dockerfile` & `dyff-0.9.4/mongodb/deploy/csv/redhat/bundle-1.7.0.Dockerfile`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/cw-bundle.yaml` & `dyff-0.9.4/mongodb/deploy/cw-bundle.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/cw-operator.yaml` & `dyff-0.9.4/mongodb/deploy/cw-operator.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/cw-rbac.yaml` & `dyff-0.9.4/mongodb/deploy/cw-rbac.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/operator.yaml` & `dyff-0.9.4/mongodb/deploy/operator.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/rbac.yaml` & `dyff-0.9.4/mongodb/deploy/rbac.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/secrets.yaml` & `dyff-0.9.4/mongodb/deploy/secrets.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/deploy/ssl-secrets.yaml` & `dyff-0.9.4/mongodb/deploy/ssl-secrets.yaml`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/mongodb/fetch-deploy-files-from-upstream.sh` & `dyff-0.9.4/mongodb/fetch-deploy-files-from-upstream.sh`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/openapi/dyff.json` & `dyff-0.9.4/openapi/dyff.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999918619791667%*

 * *Differences: {"'components'": "{'schemas': {'InferenceServiceRunnerKind': {'enum': {insert: [(1, "*

 * *                 "'huggingface')]}}}}"}*

```diff
@@ -1000,14 +1000,15 @@
                 "title": "InferenceServiceRunner",
                 "type": "object"
             },
             "InferenceServiceRunnerKind": {
                 "description": "An enumeration.",
                 "enum": [
                     "bentoml_service_openllm",
+                    "huggingface",
                     "mock",
                     "standalone",
                     "vllm"
                 ],
                 "title": "InferenceServiceRunnerKind",
                 "type": "string"
             },
```

### Comparing `dyff-0.9.3/pyproject.toml` & `dyff-0.9.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 ]
 include_external_packages = true
 
 [[tool.importlinter.contracts]]
 name = "enforce layered architecture"
 type = "layers"
 layers = [
-    "dyff.api | dyff.audit | dyff.models",
+    "dyff.api | dyff.audit",
     "dyff.client",
     "dyff.core | dyff.schema",
 ]
 
 [[tool.importlinter.contracts]]
 name = "dyff.client can't depend on dyff.core module"
 type = "forbidden"
@@ -97,29 +97,27 @@
 name = "restrict direct use of google"
 type = "forbidden"
 source_modules = [
     # "dyff.api",
     "dyff.audit",
     "dyff.client",
     "dyff.core",
-    "dyff.models",
 ]
 forbidden_modules = [
     "google",
 ]
 
 [[tool.importlinter.contracts]]
 name = "restrict direct use of pandas"
 type = "forbidden"
 source_modules = [
     "dyff.api",
     # "dyff.audit",
     # "dyff.client",
     "dyff.core",
-    "dyff.models",
 ]
 forbidden_modules = ["pandas"]
 
 [[tool.importlinter.contracts]]
 name = "avoid introducing new dependencies"
 type = "forbidden"
 source_modules = [
@@ -128,27 +126,30 @@
 ]
 forbidden_modules = [
     "matplotlib",
     "seaborn",
     "torch",
     "tensorflow",
 ]
+ignore_imports = [
+    "apps.runners.** -> torch"
+]
 
 [[tool.importlinter.contracts]]
 name = "dyff does not need these dependencies"
 type = "forbidden"
 source_modules = [
     "dyff",
 ]
 forbidden_modules = [
     "psutil",
 ]
 
 [[tool.importlinter.contracts]]
-name = "other packages do not need dyff.models dependencies"
+name = "other packages do not need bentoml"
 type = "forbidden"
 source_modules = [
     "dyff.api",
     "dyff.audit",
     "dyff.client",
     "dyff.core",
     "dyff.orchestrator",
@@ -183,42 +184,38 @@
 name = "avoid introducing new smart_open dependencies"
 type = "forbidden"
 source_modules = ["dyff", "apps"]
 forbidden_modules = ["smart_open"]
 ignore_imports = [
     "dyff.api.api -> smart_open",
     "dyff.api.data.ingest -> smart_open",
-    "dyff.models.api -> smart_open",
-    "apps.fetch_model.main -> smart_open",
 ]
 
 [[tool.importlinter.contracts]]
 name = "other packages do not need dyff.orchestrator dependencies (API too)"
 type = "forbidden"
 source_modules = [
     "dyff.api",
     "dyff.audit",
     "dyff.client",
     "dyff.core",
-    "dyff.models",
 ]
 forbidden_modules = [
     "networkx",
     "rocksdict",
 ]
 
 [[tool.importlinter.contracts]]
 name = "other packages do not need dyff.client dependencies"
 type = "forbidden"
 source_modules = [
     "apps",
     "dyff.api",
     # "dyff.audit",
     "dyff.core",
-    "dyff.models",
     "dyff.orchestrator",
 ]
 forbidden_modules = [
     "azure",
     "isodate",
 ]
 
@@ -234,15 +231,14 @@
 [[tool.importlinter.contracts]]
 name = "dyff.orchestrator does not depend on storage services"
 type = "forbidden"
 source_modules = [
     # "dyff.api",
     "dyff.audit",
     "dyff.core",
-    # "dyff.models",
     "dyff.orchestrator",
     "dyff.schema",
 ]
 forbidden_modules = [
     "gcsfs",
     "google",
     "numpy",
@@ -267,15 +263,14 @@
 name = "dyff.client depends on nothing except dyff.schema"
 type = "forbidden"
 source_modules = ["dyff.client"]
 forbidden_modules = [
     "dyff.api",
     "dyff.audit",
     "dyff.core",
-    "dyff.models",
     "dyff.orchestrator",
     "apps",
 ]
 ignore_imports = [
     "dyff.api.backend.kafka.command -> confluent_kafka",
     "dyff.orchestrator.main -> confluent_kafka",
     "apps.workflows_sink.workflows_sink.main -> confluent_kafka",
@@ -289,16 +284,10 @@
     # "apps.fetch_model",
     "apps.mocks.inferenceservice",
     "apps.runners.bentoml_service_openllm",
     # "apps.workflows_sink",
 ]
 forbidden_modules = ["dyff"]
 
-# [[tool.importlinter.contracts]]
-# name = "nothing depends on dyff.models.api"
-# type = "forbidden"
-# source_modules = ["apps.fetch_model"]
-# forbidden_modules = ["dyff"]
-
 [tool.isort]
 known_first_party = ["alignmentlabs", "dyff"]
 profile = "black"
```

### Comparing `dyff-0.9.3/requirements-orchestrator.txt` & `dyff-0.9.4/requirements-orchestrator.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,68 +1,68 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --no-emit-index-url --strip-extras requirements-orchestrator.in
 #
-absl-py==2.0.0
+absl-py==2.1.0
     # via -r requirements-orchestrator.in
 cachetools==5.3.2
     # via google-auth
-certifi==2023.7.22
+certifi==2023.11.17
     # via
     #   kubernetes
     #   requests
 charset-normalizer==3.3.2
     # via requests
 confluent-kafka==2.3.0
     # via -r requirements-orchestrator.in
-google-auth==2.23.4
+google-auth==2.27.0
     # via kubernetes
-idna==3.4
+idna==3.6
     # via requests
-kubernetes==28.1.0
+kubernetes==29.0.0
     # via -r requirements-orchestrator.in
 networkx==3.2.1
     # via -r requirements-orchestrator.in
-numpy==1.26.2
+numpy==1.26.3
     # via pyarrow
 oauthlib==3.2.2
     # via
     #   kubernetes
     #   requests-oauthlib
-pyarrow==14.0.1
+pyarrow==15.0.0
     # via -r requirements-orchestrator.in
-pyasn1==0.5.0
+pyasn1==0.5.1
     # via
     #   pyasn1-modules
     #   rsa
 pyasn1-modules==0.3.0
     # via google-auth
-pydantic==1.10.13
+pydantic==1.10.14
     # via -r requirements-orchestrator.in
 python-dateutil==2.8.2
     # via kubernetes
 pyyaml==6.0.1
     # via kubernetes
 requests==2.31.0
     # via
     #   kubernetes
     #   requests-oauthlib
 requests-oauthlib==1.3.1
     # via kubernetes
-rocksdict==0.3.17
+rocksdict==0.3.20
     # via -r requirements-orchestrator.in
 rsa==4.9
     # via google-auth
 six==1.16.0
     # via
     #   kubernetes
     #   python-dateutil
-typing-extensions==4.8.0
+typing-extensions==4.9.0
     # via pydantic
-urllib3==1.26.18
+urllib3==2.1.0
     # via
     #   kubernetes
     #   requests
-websocket-client==1.6.4
+websocket-client==1.7.0
     # via kubernetes
```

### Comparing `dyff-0.9.3/requirements.in` & `dyff-0.9.4/requirements.in`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/requirements.txt` & `dyff-0.9.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/create-gcs-bucket.py` & `dyff-0.9.4/scripts/create-gcs-bucket.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/fix-openapi.py` & `dyff-0.9.4/scripts/fix-openapi.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/generate-config-listing.py` & `dyff-0.9.4/scripts/generate-config-listing.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/generate-openapi-definitions.py` & `dyff-0.9.4/scripts/generate-openapi-definitions.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/inferenceservices/databricks--dolly-v2-3b--default.py` & `dyff-0.9.4/scripts/inferenceservices/databricks--dolly-v2-3b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/inferenceservices/tiiuae--falcon-7b--default.py` & `dyff-0.9.4/scripts/inferenceservices/tiiuae--falcon-7b--default.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/k8s-secret-data.py` & `dyff-0.9.4/scripts/k8s-secret-data.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/models/databricks--dolly-v2-3b.py` & `dyff-0.9.4/scripts/models/databricks--dolly-v2-3b.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/models/tiiuae--falcon-7b.py` & `dyff-0.9.4/scripts/models/tiiuae--falcon-7b.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/scripts/rotate-api-key-signing-secret.py` & `dyff-0.9.4/scripts/rotate-api-key-signing-secret.py`

 * *Files identical despite different names*

### Comparing `dyff-0.9.3/skaffold.yaml` & `dyff-0.9.4/skaffold.yaml`

 * *Files identical despite different names*

