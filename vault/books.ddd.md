---
id: 38da90b2-6b96-4da7-be74-80a4c127daf2
title: Domain Driven Design - Eric Evans
desc: ''
updated: 1622799177546
created: 1618319123664
---

## Part 1 - Putting the Domain model to Work

* Tackling complexity requires 
  * Common language and vocabulary
  * Skill sharing
  * A close relationship and constant communication between domain experts, usually business people, and technical experts
* The Domain Model is the *Obiquitous Language* that helps to put together experts and technical jargons
* The Domain Model can be expressed with code and diagrams
  * Diagrams *are not* the model, they are a representation
  * The code is the absolute truth because it implements the model and every detail of it
  * Well implemented and clear code can also act as a good representation
  * Code doesn't hide details for which can be necessary to have an additional diagram
  * Any additional diagram must be maintained and updated with changes in the code, reason for which is good to use them as a less detailed representation of the model
* Is important to share the language of the Domain Model inside the whole organization in order to reduce the explaination time and have consistency
* These concept can be applied also to microservices but the need of a non-code documentation is higher, nonetheless, the code will still document the details of the implementation of the single components of the model

### Chapter 3 - Binding Model and implementation

* Tightly relating the code to an underlying model gives the code meaning and makes the model relevant
* Model-Driven design discards the dichotomy of analysis model and design for a single model that serves both purposes
  * Support to an *Obiquitous Language*
  * Code as an expression of the model
  * OOP as modeling paradigm
  * Same applies to *modelers* and *implementers*
* Letting the bones show means to expose a model to users rather than hiding it
  * Let the User model and the design/implementation model to be close
  * Internet Explorer favs stored as files but not explicitly showed as so to the user

## Part 2 - The Building blocks of a Model-Driven design



