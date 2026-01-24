# flux2-kustomize-helm-example

[![test](https://github.com/omar-ashraf1488/meal-kit-MDP-k8s/workflows/test/badge.svg)](https://github.com/omar-ashraf1488/meal-kit-MDP-k8s/actions)
[![e2e](https://github.com/omar-ashraf1488/meal-kit-MDP-k8s/workflows/e2e/badge.svg)](https://github.com/omar-ashraf1488/meal-kit-MDP-k8s/actions)

## Testing

Any change to the Kubernetes manifests or to the repository structure should be validated in CI before
a pull requests is merged into the main branch and synced on the cluster.

This repository contains the following GitHub CI workflows:

* the [test](./.github/workflows/test.yaml) workflow validates the Kubernetes manifests and Kustomize overlays with [kubeconform](https://github.com/yannh/kubeconform)
* the [e2e](./.github/workflows/e2e.yaml) workflow starts a Kubernetes cluster in CI and tests the staging setup by running Flux in Kubernetes Kind
