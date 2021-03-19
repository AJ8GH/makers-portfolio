# Review process / developer process

## general notes

- TDD
  - Incremental steps, always pass the test in the simplest way possible
  - don't write redundant tests - remove them if they are redundant
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
- code .
- set up testing framework

## Information gathering

- Take down the specification
- Ask for examples of input and output
- Ask about different types of input - edge cases
- record edge cases and note each type of edge / corner case to test

## Planning

- make input / output table
- plan the steps needed in terms of test input (baby steps)
- write a user story for first part of the spec (or more if possible)
- NO object / message table or class model diagram at this stage - that is part of the red stage in the TDD process
- git commit

## Manually feature test

  - open irb
  - simulate the input of the user
  - experiment with different options for user interface if necessary
  - make a note of the user flow to implement

## TDD

- Red
  - find simplest input / output to test
  - write unit test for this
  - run test
  - read error message and do the simplest thing to change the error message (e.g. make a class, define a function)
  - continue the process until the error is a failure
  - implement simplest code possible to pass the test - normally hard coding the desired value
