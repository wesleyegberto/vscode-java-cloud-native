# VSCode Java Cloud Native

[![github-license-badge]][github-license]
[![github-badge]][github]

Extension to help write Java application in Cloud Native fashion.

Currently the options for JVM in the Dockerfile is focused for Spring Boot applications.

Features:

* snippets for Dockerfile
* snippets for Kubernetes objects
* snippets for Github Action

## Docker Images

[Maven JDK](https://hub.docker.com/_/maven):

- `maven:3.6-jdk-11`
- `maven:3.8-openjdk-11`
- `maven:3.8-openjdk-17`

Java images:

- JDK 11:
  - OpenJDK: `openjdk:11`
  - Open J9: `adoptopenjdk/openjdk11-openj9:alpine-slim`
- JDK 11:
  - OpenJDK: `openjdk:17-alpine`
  - Open J9: `ibm-semeru-runtimes:open-17-jdk`

## Snippets

### Dockerfile

| Prefix | Description |
| --- | --- |
| `java-openj9-optimized-runtime` | Snippet for Dockerfile using Open J9 11 as runtime |
| `java-openj9-optimized-multistage` | Snippet for Dockerfile with multistage build using Maven and Open J9 11 as runtime |
| `java-openj9-optimized-multistage-unziped` | Snippet for Dockerfile with multistage build using Maven and Open J9 11 as runtime, the Uberjar file is unziped for runtime |

### Kubernetes

| Prefix | Description |
| --- | --- |
| `k8s-namespace` | Kubernetes namespace |
| `k8s-deployment` | Kubernetes deployment |
| `k8s-rollingupdate` | Kubernetes deployment rollout strategy |
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

### Github Action

| Prefix | Description |
| --- | --- |
| `gh-action-java-ci` | Github Action CI for Java (build, test, upload test and coverage report) |

## References

- [Microsoft's Containerize Java Applications](https://docs.microsoft.com/en-us/azure/developer/java/containers/overview)

[github-license]: https://github.com/wesleyegberto/vscode-java-cloud-native/blob/master/LICENSE
[github-license-badge]: https://img.shields.io/github/license/wesleyegberto/vscode-java-cloud-native.svg?style=flat "License"
[github]: https://github.com/wesleyegberto/vscode-java-cloud-native/actions?query=branch%3Amaster
[github-badge]: https://github.com/wesleyegberto/vscode-java-cloud-native/actions/workflows/ci.yml/badge.svg?branch=master
[github-history-badge]: https://buildstats.info/github/chart/wesleyegberto/vscode-java-cloud-native?includeBuildsFromPullRequest=false "GitHub Actions History"
