registry
========

## Pre-Requisites
1. Make sure helm version **3** is installed.
```bash
$ helm version --short
v3.5.0+g32c2223
```

## Setup
1. To use the above helm chart make sure you have created your secrets as defined in `registry/values.yaml` under the heading `secrets`
2. Also make sure `helm` is installed.
3. Install the release using helm
```bash
$ helm install registry registry
```

## Development
1. In order to lint the charts once you are done with your development
```bash
$ helm lint registry
```
2. In order to make sure that templates are rendered withour any issue
```bash
$ helm template registry
```

## TODO
1. Use `redis` as cache in config
2. Provide healthchecks for backends
3. Use redis pool for registry
4. Fix registry test cases
