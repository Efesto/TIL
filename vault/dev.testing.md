---
id: b3366033-0a7d-4804-b6b4-c3bba134eff8
title: Testing
desc: ''
updated: 1619015517024
created: 1619013941733
---

[When TDD is Difficult - Try this!](https://www.youtube.com/watch?v=ESHn53myB88)


### Acceptance testing
- Requires simulating a user behaviour
- Black box testing on a version of the system as much as possible close to production
- Slow, but effective

### Unit testing
- Works better by replacing the edges of our system, like file system, db, and so on with fakes
- Introducing abstractions helps us to adopt TDD by allowing the test to be focused on the logic rather than edges interactions
- Abstracting edges helps with separation of concerns, repleceability and test execution speed

### My favourite
- Top-down or outside-in TDD with inner loops of unit testing for tackling complexities
- Prevents over-engineering because you can stop once the test is clear and good enough
- Starts with the user case
- Leaves space for refactoring
- Satisfying, because it starts with some red test and ends with a suite of greens

### TO CHECK
- Defensive programming towards dependencies techniques
- Contract enforcing in order to effectively avoid E2E testing