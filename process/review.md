# Review process / developer process

## general notes
- TDD
  - Incremental steps, always pass the test in the simplest way possible
  - don't write redundant tests - remove them if they are redundant
  - Red
    - find simplest input / output to test
    - write unit test for this
    - run test
    - read error message and do the simplest thing to change the error message (e.g. make a class, define a function)
    - continue the process until the error is a failure
    - implement simplest code possible to pass the test - normally hard coding the desired value
- frequent commits:
  - After every green test
  - After every refactor
  - good commit message starting with capital letter
  - commit message should summarise what was implemented or what the added code does. does not need to mention the test it passed

## Set up
- mkdir new-project-directory
- cd new-project-directory
- touch README.md
- git init
- git add .
- git commit -m 'First commit'
- set up testing framework

## Understand

### Information gathering
- Take down the specification in the README
- Ask for examples of input and output
- Ask about different types of input - edge cases
- record edge cases and note each type of edge / corner case to test
- Ask if we might receive invalid inputs

### Planning
- make input / output table
- plan the steps needed in terms of test input (smallest steps possible)
- Maybe translate the requirements into user stories if appropriate
- NO object / message table or class model diagram at this stage - that is part of the red stage in the TDD process
- Commit the planning notes

### Manually feature test
- open irb
- simulate the input of the user
- experiment with different options for user interface if necessary
- make a note of the user flow to implement

## Solve
- Tell interviewer / reviewer that you will take a few minutes to think about your approach to the problem and that you will get back to them once you've done this.
- Have a piece of paper handy to sketch
- brainstorm and list algorithms and data structures, and pattern match these to the problem
- work backwards - start with the expected output and work backwards from there
- break problem down into small steps
- start with the big picture and do an end to end breakdown, don't focus too much on the individual small details at least at first or worry if there are steps which are not clear on how to solve

## Communicate
- Once you have a high-level solution, start communicating it to interviewer
- show you can communicate high-level technical concepts
- explain in a few sentences what your approach is, reference the type of data structures, algorithms, constructs or methods you are using
- goal here is to validate your approach before you start writing code. Find out if some part of your approach is undesirable or unnecessary for them
- Clarify when you deviate from an approach you would take in production, e.g. "in production I would encapsulate this in a class, here I just plan to use an array instead."
- Use this step to manage risk. You have a high level approach but may not fully understand how to do some steps yet
- Heierarchy (do each one only if necessary to fully breakdown and understand problem):
  - first high-level verbal run through
  - then walk through a small example, write down your state, then update your state as you walk through your example
  - then write down the steps in pseudocode
- if you pause or change approach or think - explain why, thought process
- if the code gives the wrong output, tell them that you notice this and why you think this is. show that you understand error messages. show your debugging and problem solving process at this point. Don't read out entire error message - just point out the specific problem and the line it's coming from. figure out the problem in your code if you can or if not, explain the steps you are taking to get there.
- if things get messy or you get stuck, talk to the interviewer rather than waste time
- don't narrate your thoughts due to nerves! express your nerves productively

## Implementation
- Dependent on having a good solution in mind!
- Be comfortable in your programming language and the tools available to you
- Write your code incrementally - run tests, run the code, use print to inspect state. Test assumptions as you go
- Write small methods
- Allows you to test smaller chunks of code - both better code quality and also less confusing for you.
- magic methods - if you can abstract something you don't know into a method and carry on, this is better. Get a whole structure, even if one part of it isn't implemented fully.
- Don't narrate thoughts outloud when you code.
