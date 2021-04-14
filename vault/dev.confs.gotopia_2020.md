---
id: 4ddc16fc-0bf8-42ee-b292-5214cee9ab0c
title: GOTOpia 2020
desc: ''
updated: 1618325367737
created: 1618319229170
---

## War is Peace, Freedom is Slavery, Ignorance is Strength, Scrum is Agile - Allen Hollub
![](/brain/assets/images/confs.gotopia_2020.1.png)
* What is Agile and what is not
* Is
  * Continuous communication
  * fast feedback REALLY fast
    * by pushing Value to the users and receiving feedback
    * Being able to change fast
  * focus on people
  * Self-organizing teams
    * Which do their own hiring
    * Which change their own processes
      * An organization where everyone works in the same way is a red flag for agility
    * A small team number, between 3 and 6, allows an effective communication
      * In a communication graph, the less edges, the better
    * Inter team communication happens organizally without any overhead push
* Scrum is a wrapper for Agile, is not Agile
  * It doesn't make sense without XP, XP without Scrum works just fine
* You cannot move an agile process that worked in a place to another and expect success
* Plans fail, always, because we are learning
* Technical excellence allows fast changes

## Prioritizing Technical Debt as if Time and Money Matters - Adam Tornhill
* Prioritizing Technical debt requires determining business impact
* Identifiyng critical points for tech debt requires identifying hotspots
  * Code complexity combined with frequency of change
  * Eventual loss of knowledge by identifying codebase with bus number 1
* The perception of tech debt includes social factors
  * A code might be perceived as messy if a team is not familiar with it
* Tools/techniques
  * Codescene.io
  * Adam Tornhill repository
  * X-Ray code insight
  * Check his books
    * Analyzing code as a crime scene
* Lehman's laws of software dev

## Three Practices for Effective DevOps Adoption - Eoin Woods
* __Devops__ as a conseguency of Agility movement
  * The point of following Devops is speed and control for achieving Continuous Delivery
* > Cross-functional teams, delivering and operating software as a visible, measurable flow of value in a continuous and sutainable way
  * Continuous Delivery
  * C.A.L.M.S.
* Devops needs a regular, sustainable and predicatble flow of valuable changes
* __Agile Working__
  * Requires empowered, informed, decisive POs
  * Empowered cross-functional team
  * High quality backlog
  * Consistent and sufficient code quality
* __Pipeline__ - Stability, Confidence, consistency and repeatability
  * Single automated path from commit to deploy
  * As a collaboration point
  * As a visible visualization of path to production
* __Enabler Team__
  * Build useful shared devop tools
  * Develop culture by example
  * Bring and transfer technical knowledge
    * EG: building the first pipeline
  *  ![some enabler team models](/brain/assets/images/confs.gotopia_2020.2.png)
  * Enabler team typical dissolve
* 4 eyes principle requires active partecipation of unlocking managers
  * Part of the culture
  * Part of the sustainability - eventually
  * Reduce the friction

## Dave Thomas
* Mentorship is a way to teach and to learn
* An organization where is too risky to let a Junior to put code in production has some problem
* We as Scientists are experimenting and errors are part of that

## Take Aways
* have a look at gRPC
* [Netflix full cycle development for team organization](https://netflixtechblog.com/full-cycle-developers-at-netflix-a08c31f83249)
* Event storming as a project kick off process could be worthy to give a read
* Event sourcing, implementations, problems and solutions
* Software development metrics - Time in process, percentages (as a meaning for estimation), identify the real goal, consider, fixed cost time (like commuting)
* Normal distribution for estimation doesn't make sense, what makes sense is average time of things in processing time
* Enabler team is a really cool concept for pushing devops

