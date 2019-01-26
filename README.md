# The Stumptown Labs Library for Kubernetes

Applications, provided by [Stumptown Labs](https://stumptownlabs.com), ready to launch on Kubernetes using [Kubernetes Helm](https://github.com/helm/helm).

## TL;DR

```bash
$ helm repo add stumptownlabs https://stumptownlabs.github.io/charts
$ helm search stumptown
```

## Upstreamed charts (contributed to [helm/charts](https://github.com/helm/charts))

- [Dokuwiki](https://github.com/helm/charts/tree/master/stable/dokuwiki)


## Stumptown Labs charts

- [DKAN](https://github.com/stumptownlabs/charts/tree/master/stumptownlabs/dkan)
- [Geomesa-Cassandra](https://github.com/stumptownlabs/charts/tree/master/stumptownlabs/geomesa-cassandra)


## Before you begin

### Setup a Kubernetes Cluster

The quickest way to setup a Kubernetes cluster is with [Azure Kubernetes Service](https://azure.microsoft.com/en-us/services/kubernetes-service/), [AWS Elastic Container Service](https://aws.amazon.com/eks/) or [Google Kubernetes Engine](https://cloud.google.com/kubernetes-engine/) using their respective quick-start guides. For setting up Kubernetes on other cloud platforms or bare-metal servers refer to the Kubernetes [getting started guide](http://kubernetes.io/docs/getting-started-guides/).

### Install Helm

Helm is a tool for managing Kubernetes charts. Charts are packages of pre-configured Kubernetes resources.

To install Helm, refer to the [Helm install guide](https://github.com/helm/helm#install) and ensure that the `helm` binary is in the `PATH` of your shell.

### Add Repo

The stable charts are contributed to the upstream [helm/charts](https://github.com/helm/charts) repository. The following command allows you to download and install all the charts from this repository, both the bitnami and the upstreamed ones.

```bash
$ helm repo add stumptownlabs https://stumptownlabs.github.io/charts
```

### Using Helm

Once you have installed the Helm client and initialized the Tiller server, you can deploy a Stumptown Labs Helm Chart into a Kubernetes cluster.

Please refer to the [Quick Start guide](https://github.com/helm/helm/blob/master/docs/quickstart.md) if you wish to get running in just a few commands, otherwise the [Using Helm Guide](https://github.com/helm/helm/blob/master/docs/using_helm.md) provides detailed instructions on how to use the Helm client to manage packages on your Kubernetes cluster.

Useful Helm Client Commands:
* View available charts: `helm search`
* Install a chart: `helm install stable/<package-name>`
* Upgrade your application: `helm upgrade`

# License

Copyright (c) 2019 Stumptown Labs

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.