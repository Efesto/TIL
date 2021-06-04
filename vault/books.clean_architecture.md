---
id: 89abee74-1611-4cc7-8ade-0ba99ec53a73
title: Clean Architecture - Robert C. Martin
desc: ''
updated: 1622802148137
created: 1622797002140
---
![](/brain/assets/images/2021-06-04-11-24-44.png)

### CHP 22 - The clean architecture
* **The dependency Rule**: source code dependencies must point only inward, toward higher-level policies 
* Clean architecture is:
  * Indipendent of frameworks
  * Testable
  * Indipendent of the UI
  * Indipendent of the database
  * Indipendent of any external agency

### CHP 25 - Layers and Boundaries

* Architectural layers and boundaries exists also in the simplest program
* The components for implementing the language interpretation in an adventure game may lie in the `language layer`

### CHP 27 - Services: great and small

* System architecture is a set of boundaries that separate high-level policies from low-level details and follow Dependency Rule. AKA: decoupling fallacy
* Separating behaviours in services means implementing expensive function calls
* Services can be decoupled by code and resources but might be coupled by shared data
* History shown that large enterprise systems can be built by monoliths and by service-based systems as well, scalability is not exclusive to the last
* The taxi distribution system and the kitty problem shows how not even microservices are immune to big changes for implementing new behaviours, SOLID helps in this by driving us to implement the service change withing the service itself

