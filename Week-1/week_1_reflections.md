# Week 1

## Goals
- [x] Master TDD using RSpec
- [x] become confident in mocks: using different kinds of stubs and doubles, when to use them and why
- [x] understand best practices for when and how to use subject, let, before and after effectively
- [x] utilise the above methods to write, robust and DRY tests
- [x] Become proficient and comfortable in pair programming
- [x] Learn how to use Github collaboration effectively
- [x] Decide on which driver navigator style works for me
- [x] be confident in achieving the maximum possible in the given time in any pairing session

## Skills learned and applied

- Encapsulation
- SRP
- TDD
- Mocking with doubles and stubs in `rspec`
- Domain Modelling
- BDD
- Sequence Diagrams
- Using modules to mixin common functionality to multiple classes
- Memoization

## Challenges

#### [AIRPORT CHALLENGE](https://github.com/AJ8GH/airport_challenge)

Our first weekend challenge! Built a program for air traffic control, complete with safety guards and its own weather system.

#### [BORIS BIKES](https://github.com/AJ8GH/boris-bikes)

The Pair programming challenge for the week was focused on building a system for docking, releasing, tracking and maintaining the network of so called Boris Bikes across London.

## Debugging Workshop

### Topics covered:

- Explored different ways to debug code.
- Learned the 'tighten-the-loop' process
- Worked through fixing some bugs in classes within
- [Resource page](https://github.com/AJ8GH/skills-workshops/tree/master/test_driven_development/debugging_1)

### Key Take-Aways

- Error messages give a lot of helpful info - reading through carefully is the best place to start
- Stack-trace - read through from bottom to top, the bottom line is the first piece of relevant code run. The top line is where the code eventually breaks. Each specifies the file path and the line of code.
- Sometimes the bug will be somewhere else, e.g. in a Gem your app is using! Follow the stack-trace, wherever it takes you.
- Debugging process:
  - Tighten the loop (find the exact line the bug is coming from)
  - Get visibility (use p to inspect everything to help you home in on the exact line)
  - Once you know the one thing that is wrong, out of place, misspelled, or not giving you what you expect, try to fix it.

_"Wisest are they who try only one thing to fix the problem. Faffing about trying whatever occurs to you next is a recipe for development hell."_
