# Developer Process

## Environment Setup (Ruby)
1. mkdir <new-project-directory>
2. cd <new-project-directory>
3. mkdir lib
4. touch README.md
4. rspec --init
5. bundle init
6. setup Gemfile:
  - gem 'rspec'
  - gem 'rubocop'
  - gem 'simplecov'
  - gem 'simplecov-console'
  - ruby '3.0.0'
7. bundle install
8. git init
9. create new github repo of same name
10. git remote add origin <github-repo-ssh-address>
11. git add .
12. git commit -m 'first commit'
13. git push -u origin main

## Domain modelling

1. Read through client specification in full
2. break down into user stories (if not already done)
3. keep the user stories in user_stories.md or in README.md
3. choose the first user story to work on - normally the simplest and work through the user stories one at a time
4. create table of objects (nouns) and messages (verbs) for the first user story
5. draw sequence diagram to represent the flow of data and messages between the objects and the user
7. save the sequence diagram code in sequence_diagrams.md, user_stories.md or notes.md

## Code

## Problem Solving
1. write the problem out in pseudocode
2. break large steps down into smaller ones
3.
