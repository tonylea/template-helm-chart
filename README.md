# App Name Helm Chart

![Downloads](https://img.shields.io/github/downloads/tonylea/helm-chart-app-name/total)

[One line: what the chart deploys, linked to the project, and the image it uses, linked to the image's source, with why that image (its official image, or the one the project's docs recommend).]

[What makes the chart opinionated, and how it runs: replicas, the update strategy and why, and where App Name keeps its data.]

## Values

[A table of every value in `values.yaml` and its default. A value with no default says what it needs, such as "none; required" or "none; the chart creates a claim".]

| Value | Default |
| --- | --- |

## Fixed settings

[The settings the chart sets for App Name that can't be changed in its web UI, each with why. Leave this section out if there are none.]

## Requirements

[What has to exist before an install: databases, Secrets and their keys, storage classes, and the Gateway API's `HTTPRoute` CRD when `httpRoute.enabled` is set.]

## Usage

```sh
helm repo add app-name https://tonylea.github.io/helm-chart-app-name
helm install app-name app-name/app-name --values my-values.yaml
```

[An example `my-values.yaml` that sets the required values.]

## Development

Pull requests run:

- `helm lint --strict`, and the rendered chart checked by kubeconform against Kubernetes 1.37.
- helm-unittest's tests in `tests/`.
- [An install with chart-testing in a kind cluster, and what it installs against from `ci/kind`, if anything.]

Commits follow Conventional Commits.
Releases are versioned and tagged automatically from `main`, and published to the Helm repository on this repo's GitHub Pages.
