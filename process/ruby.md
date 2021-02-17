# Developer Process - Ruby

## Ruby project setup

1. `mkdir <new-project-directory>`
2. `cd <new-project-directory>`
3. `mkdir lib`
4. `touch README.md`
4. `rspec --init`
5. `bundle init`
6. setup Gemfile:
  - `gem 'rspec'`
  - `gem 'rubocop'`
  - `gem 'simplecov'`
  - `gem 'simplecov-console'`
  - `ruby '3.0.0'`
7. `bundle install`
8. `git init`
9. create new github repo of same name
10. `git remote add origin <github-repo-ssh-address>`
11. `git add .`
12. `git commit -m 'first commit'`
13. `git push -u origin main`
