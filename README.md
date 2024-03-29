# Is one Kubernetes Cluster enough?

A single Kubernetes cluster provides an extremely flexible platform to design
any complex distributed system. This also includes statefull workloads such as
databases.

![cluster-Architecture](./_media/k8s-architecture.png)

For many scenarios a single cluster is enough.

- scaleability achieved by increasing number of nodes from a node pool
  > Kubernetes 1.24
  > [supports](https://kubernetes.io/docs/setup/best-practices/cluster-large/#:~:text=Kubernetes%20v1.24%20supports%20clusters%20with%20up%20to%205000%20nodes)
  > clusters up to **5000** nodes
- workload isolation using namespaces

When are multiple clusters needed.

- there are already existing clusters that need to talk to each other
- strict security and workload isolation rules
- cost factors

## Multi-Cluster Architecture

## Connectivity Levels

## List of Projects

[Good comparison](https://www.cncf.io/blog/2021/04/12/simplifying-multi-clusters-in-kubernetes/)

- [Submariner](https://submariner.io/)
- [Skupper](https://github.com/skupperproject/skupper)
- [KubeCarrier](https://docs.kubermatic.com/kubecarrier/v0.3/)
- [Linkerd](https://linkerd.io/2.11/features/multicluster/)
- [Cilium Cluster Mesh](https://docs.cilium.io/en/stable/gettingstarted/clustermesh/clustermesh/#gs-clustermesh)
- [Multi-Cluster Service APIs](https://github.com/kubernetes-sigs/mcs-api)
- [Consul Connect](https://www.consul.io/docs/connect)
- [Liqo](https://github.com/liqotech/liqo)
- [Yggdrasil](https://github.com/uswitch/yggdrasil)
- [KEP-1645](https://github.com/kubernetes/enhancements/tree/master/keps/sig-multicluster/1645-multi-cluster-services-api)

### Table with levels

## Demo with Cilium cluster mesh
