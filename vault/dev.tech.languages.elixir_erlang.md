---
id: 4a393d90-2cfb-48d0-ac13-b4b4eb62b134
title: Elixir & Erlang
desc: ''
updated: 1622210158344
created: 1618384711136
---

- The world of Elixir Http Clients is complex and Tesla is a good all around choice
- [Keathley about Finch and Http clients](https://elixirforum.com/t/mint-vs-finch-vs-gun-vs-tesla-vs-httpoison-etc/38588/11)
- [Slab and building a real time collaboration tool](https://elixir-lang.org/blog/2020/11/17/real-time-collaboration-with-elixir-at-slab/)
- [Custom ExUnit assertions](https://www.crustofcode.com/custom-assertions-with-exunit/)
- [Some neat NIF example](https://dev.to/rodrigocaldeira/elixir-and-nif-a-study-case-2npp)

### Secure coding guidelines
https://erlef.github.io/security-wg/secure_coding_and_deployment_hardening/
https://github.com/nccgroup/sobelow


### Embracing errors in Erlang
https://www.youtube.com/watch?v=TTM_b7EJg5E&list=WL

* Fault tollerance and scaling is impossible on a single computer
  * Hardware faults
* Find methods to prove software is correct at compile time
* Assume that shit happens at runtime so something needs to be done then
  * Software is implicitly incorrect
* Proving self-consistency doesn't help
  * Types system proves that the system is consistent in itself
  * Large assemblies of small things cannot be proved correct
* Adopting message passing, rejecting shared memory
* Don't try to fix an error, don't ignore it; Crash and assume somebody else will fix the problem
* When a sequential program crashes, nothing remains
  * Crashing is generally not embraced becauses
* With a concurrent/parallel language
  * Easier error recovery
  * Programming on one local system as on multiple systems
* Error Kernel -> The part that is correct involving an error


