---
id: c0916890-936f-4f17-9c85-1960d763f744
title: Kubernetes
desc: ''
updated: 1622210592760
created: 1622209333900
---

> Kubernetes, also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications.

https://kubernetes.io/

### Glossary
* [Node](https://kubernetes.io/docs/concepts/architecture/nodes/) - VM or physical machine
  * runs Kubelet
* Cluster - Combination of nodes with a control plane
* [Deployment](https://kubernetes.io/docs/concepts/workloads/controllers/deployment/) - Description of the cluster changes from the actual state to the desired
* Kubelet - Agent for managing the node
* [Pod](https://kubernetes.io/docs/concepts/workloads/pods/) - Basic execution unit of a Kubernetes App  
  * One container per pod is the most common k8s use case
  * Is part of a workload
  * Can be one or more application containers
  * Containers in a pod share storage and network resources
  * Ephemeral
* Service - Logical set of pods
  * Pods in a service communicate together
* ConfigMaps - maps of configuration for the applications
  * Can be exposed as file, as env variable and so on
* [Workload](https://kubernetes.io/docs/concepts/workloads/) - An application running on Kubernetes

### Tools
https://github.com/Shopify/krane


[[dev.tech.languages.elixir_erlang.kubernetes]]






