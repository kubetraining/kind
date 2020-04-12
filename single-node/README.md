


```bash
Usage:
  kind create cluster [flags]

Flags:
      --config string       path to a kind config file
  -h, --help                help for cluster
      --image string        node docker image to use for booting the cluster
      --kubeconfig string   sets kubeconfig path instead of $KUBECONFIG or $HOME/.kube/config
      --name string         cluster context name (default "kind")
      --retain              retain nodes for debugging when cluster creation fails
      --wait duration       wait for control plane node to be ready (default 0s)

Global Flags:
      --loglevel string   DEPRECATED: see -v instead
  -q, --quiet             silence all stderr output
  -v, --verbosity int32   info log verbosity

```

Creating Clusters with Single Node (AIO - all in once)

```bash
# K8s Cluster (name : mycluster)
kind create cluster --name mycluster

# K8s api 1.18
kind create cluster --image kindest/node:v1.18.0

# K8s api 1.17
kind create cluster --image kindest/node:v1.17.0

```