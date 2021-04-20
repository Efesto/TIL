---
id: 4a393d90-2cfb-48d0-ac13-b4b4eb62b134
title: Elixir
desc: ''
updated: 1618917109555
created: 1618384711136
---

- The world of Elixir Http Clients is complex and Tesla is a good all around choice
- [Keathley about Finch and Http clients](https://elixirforum.com/t/mint-vs-finch-vs-gun-vs-tesla-vs-httpoison-etc/38588/11)
- [Slab and building a real time collaboration tool](https://elixir-lang.org/blog/2020/11/17/real-time-collaboration-with-elixir-at-slab/)

### Secure coding guidelines
https://erlef.github.io/security-wg/secure_coding_and_deployment_hardening/
https://github.com/nccgroup/sobelow

### On the topic of distributed Elixir/Erlang and K8S

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