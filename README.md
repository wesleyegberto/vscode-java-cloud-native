# VSCode Java Cloud Native

[![](https://vsmarketplacebadge.apphb.com/version/wesleyegberto.vscode-java-cloud-native.svg)](https://marketplace.visualstudio.com/items?itemName=wesleyegberto.vscode-java-cloud-native)
[![](https://vsmarketplacebadge.apphb.com/installs-short/wesleyegberto.vscode-java-cloud-native.svg)](https://marketplace.visualstudio.com/items?itemName=wesleyegberto.vscode-java-cloud-native)

Extension to help write Java application in Cloud Native fashion.

Currently the options for JVM in the Dockerfile is focused for Spring Boot applications.

Features:

* snippets for Dockerfile
* snippets for Kubernetes objects
* snippets for Github Action

## Dockerfile

| Prefix | Description |
| --- | --- |
| `java-openj9-optimized-runtime` | Snippet for Dockerfile using Open J9 11 as runtime |
| `java-openj9-optimized-multistage` | Snippet for Dockerfile with multistage build using Maven and Open J9 11 as runtime |
| `java-openj9-optimized-multistage-unziped` | Snippet for Dockerfile with multistage build using Maven and Open J9 11 as runtime, the Uberjar file is unziped for runtime |

## Kubernetes

| Prefix | Description |
| --- | --- |
| `k8s-namespace` | Kubernetes namespace |
| `k8s-deployment` | Kubernetes deployment |
| `k8s-secret-opaque` | Kubernetes secret using Base64 encoded data |
| `k8s-secret-plain` | Kubernetes secret using plain text data |
| `k8s-env-from-secret` | Container environment var from Kubernetes Secret |
| `k8s-env-from-configmap` | Container environment var from Kubernetes ConfigMap |
| `k8s-configmap-file` | Configmap that contains a file |
| `k8s-configmap` | ConfigMap with a Key/Value pair |
| `k8s-configmap-kv-file` | ConfigMap with a Key/Value pair and file |
| `k8s-file-from-secret` | Mount a file from a Kubernetes Secret |
| `k8s-svc` | Kubernentes service v1 |
| `k8s-svc-intern` | Kubernentes service with internal LB |
| `k8s-hpa` | Kubernentes horizontal pod autoscaler |
| `k8s-ing-svc` | Kubernentes ingress direct to a service |
| `k8s-ing-fanout` | Kubernentes ingress fanout |
| `k8s-ing-named-based` | Kubernetes ingress named based |

## Github Action

| Prefix | Description |
| --- | --- |
| `gh-action-java-ci` | Github Action CI for Java (build, test, upload test and coverage report) |
