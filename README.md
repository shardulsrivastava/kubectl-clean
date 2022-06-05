# Kubectl Plugins


## kubectl-clean

A `kubect` plugin that cleans all the terminated pods in your cluster.

### Quick Start

#### From Source

```bash
git clone git@github.com:shardulsrivastava/kubectl-clean.git
cd kubectl-clean
mv kubectl-clean/kubectl-clean /usr/local/bin
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