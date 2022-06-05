# Kubectl Plugins


## kubectl-clean

A `kubectl` plugin that cleans all the terminated pods in your cluster.

### Quick Start

#### From Source

```bash
git clone git@github.com:shardulsrivastava/kubectl-plugin.git
cd kubectl-plugin/plugins/kubectl-clean
mv kubectl-clean /usr/local/bin
kubectl clean --help
```

### Usage

To delete all the terminated pods in a namespace in a cluster: 
```bash
kubectl clean <NAMESPACE>
```

To delete the terminated pods from all the namespaces in a cluster:

```bash
kubectl clean all
```

## kubectl-find-deprecated-clusters

A `kubectl` plugin that checks for GKE clusters using deprecated versions of Kubernetes inside a GCP folder.

### Quick Start

#### From Source

```bash
git clone git@github.com:shardulsrivastava/kubectl-plugin.git
cd kubectl-plugin/plugins/find-deprecated-clusters
mv kubectl-find-deprecated-clusters /usr/local/bin
kubectl find-deprecated-clusters --help
```

### Usage

To check for all the clusters running kubernetes version lower than `1.20` inside folder Id `xyz` : 
```bash
kubectl find-deprecated-clusters <GCP Folder Id> <GKE Minimum Version(optional)> 
```

To delete the terminated pods from all the namespaces in a cluster:

```bash
kubectl find-deprecated-clusters 907623304376 1.21
```