---
id: c0a783b2-0c1c-4f26-a908-327c442548c6
title: On distributed Elixir/Erlang and Kubernetes
desc: ''
updated: 1622210259090
created: 1622210180765
---

https://dashbit.co/blog/kubernetes-and-the-erlang-vm-orchestration-on-the-large-and-the-small

* Erlang offers fault tollerance at application level: if your connection to db sporadically fails but your health check doesn't
  * K8S provides fault tollerance at node level, Erlang at application/software level
* Does make sense Erlang's internode communication capacity when K8S allows us to use protocols as gRPC and service discovery?
  * Service discovery works amazing together with node communication in Erlang
  * Erlang offers a native approach cutting serialization/deserialization for communicating between instances of the same application
* Erlang's hot code swapping
  * Hot code swapping was fitting Ericsson's needs where there isn't ever a good moment to restart
  * K8S changes rolling out is good enough for most of the cases
* Config providers are cool and fits well with K8S https://hexdocs.pm/elixir/Config.Provider.html
* Big pods are good because Erlang VM is good in sharing resources between 
