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

## kubectl-gke-outdated

A `kubectl` plugin that checks for GKE clusters using outdated versions of Kubernetes inside a GCP folder.

### Quick Start

#### From Source

```bash
git clone git@github.com:shardulsrivastava/kubectl-plugin.git
cd kubectl-plugin/plugins/gke-outdated
mv kubectl-gke_outdated print-table /usr/local/bin
kubectl gke-outdated --help
```

### Usage

To check all the GKE clusters running outdated kubernetes version inside folder Id `xyz` : 
```bash
kubectl gke-outdated <GCP Folder Id> <GKE Minimum Version(optional)> 
```

To check all the GKE clusters inside folder id `907623304376` running kubernetes version lower than `1.22` :

```bash
kubectl gke-outdated 907623304376 1.22
```