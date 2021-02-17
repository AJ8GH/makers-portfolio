# Sinatra Project Setup

1. create project folder:
  - `mkdir <project-name>`
2. create Gemfile:
  - `bundle init`
3. add gems to gemfile:
  - `capybara`, `rspec`, `sinatra`
4. install gems:
  - `bundle`
5. create testing suite:
  - `rspec --init`
  - `mkdir spec/features`
6. require libraries and app in spec_helper
  - `require 'capybara'`
  - `require 'capybara/rspec'`
  - `require 'rspec'`
  - `require './..app'`
7. create views:
  - `mkdir views`
  - `touch views/index.erb`
8. create controller file:
  - `touch app.rb`
9. set up app.rb file
  - `require 'sintatra'`
  - define app class which inherets from `Sinatra::Base`
  - `enable :sessions`
  - `set :sessions_secret`
10. create models folder:
  - mkdir `lib`
11. create config.ru file:
  - `touch config.ru`
12. set up config:
  - `require './app'`
  - `run <AppClassName>`
