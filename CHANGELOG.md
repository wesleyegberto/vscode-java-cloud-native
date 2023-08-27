# Change Log

All notable changes to the "vscode-java-cloud-native" extension will be documented in this file.

Check [Keep a Changelog](http://keepachangelog.com/) for recommendations on how to structure this file.

## [0.0.6] - 2023-08-26

- Fixed:
  - Snippet without escape `$`

## [0.0.5] - 2022-06-15

- Changed:
  - removed `replica: 1` from deployment snippet to keep only rollout strategy
- Added:
  - added snippet for rolling update

## [0.0.4] - 2022-04-20

- Changed:
  - Snippet to create Secret using opaque to `k8s-secret-opaque`
  - Snippet to use environment variables from Secret
- Added:
  - Snippet to create Secret using plain string

## [0.0.3] - 2022-04-07

- Fixed:
  - Snippet to set environment variable from ConfigMap key

## [0.0.2] - 2022-03-12

- Added:
  - Snippets for Kubernentes service with internal LB
- Fixed:
  - Image with unzipped Jar still using to Jar file

## [0.0.1] - 2021-06-05

- Initial release