# Week 3

Started the week with learning about building basic web applications

Debugging - fixed a bug which was preventing puma from running with Sinatra using Shotgun. Submitted a pull request with the gem's repo.

## Practicals completed
- Sinatra pills
- Servers 1
- Clients 1
- HTTP Servers
- Birthday greeter app

## Key Skills learned
- Setting up a web app with Sinatra
- Setting up testing infrastructure for web apps using capybara and rspec
- Using webdriver with capybara
- MVC: organising code into model-view-controller structure
- HTML: building web pages using html
- CSS: applying styling to web pages
- erb: combining HTML and CSS with ruby code using erb
- Sinatra project structure: learning the more complicated setup required for getting sinatra web apps up and running, as well as important naming and project folder structure conventions
- storing class instance within class instance variables to allow the object to be visible across the entire scope of an app
- using layouts to wrap erb templates and link css stylesheets

## Mini project

 Flying solo - built a [birthday greeter](github.com/AJ8GH/birthday-app) app, applying many of the techniques and skills picked up in this week's workshops, challenges and learning materials. Whilst the finished product doesn't look terrifically complicated, it was deceptively tricky and was great practice in applying the OOD principles I've learned in weeks 1 & 2 and combining those with MVC principles in week 3. Plus some good HTML and CSS practice!

## Pairing challenge

### [Battle](https://github.com/AJ8GH/battle)

Applying our learnings in our weekly pairing challenge - working together to learn how servers work, the different kinds of HTTP requests. How we can apply this knowledge with our Ruby programming skills to build simple web-apps

## Weekend Challenge

### [Rock Paper Scissors](https://github.com/AJ8GH/rps-challenge)

The weekend challenge for our 3rd week is as always a follow on from the week's learning topics and goals. It's an independent project which we work through without peer or coach help. My approach here is to apply some of the advanced topics from the battle app project early on - such as using class instance variables to store the instance of a class - and avoid the use of evil $global variables altogether.

#### goals:
- apply strict use of MVC structure, keeping SRP, encapsulation and cohesion high
- keep controllers and views as skinny as possible, extracting all logic to the model
- use layouts to wrap my erb templates and apply styling for a sexy interface

## HTTP Skills workshop

### HTTP Request sequence diagram

```flow
# parties

alias u = "User"
alias c = "Client/Browser"
alias s = "Server"

# going to web page

user->client: "Type in http://makers-cats.herokuapp.com/"
client->server: "HTTP GET / request"
server->client: "200 OK, here's the html"
client->user: "Renders the HTML (shows page to the user)"

# typo

u->c: "Type in http://makers-rats.herokuapp.com/"
c->s: "HTTP GET / request"
s-->c: "404 page not found - alternative HTML page"
c->s: "HTTP GET / request http://alternative-HTML-page"
s-->c: "200 OK alternative HTML page"
c-->u: "HTML rendered"

# image

u->c: "click cat-pic link"
c->s: "HTTP GET / request"
s-->c: "200 OK - HTML with cat img relative url"
c-->u: "HTML rendered"
c->s: "HTTP GET / cat-img-rel-url"
s-->c: "200 OK cat pic"
c-->u: "cat pic rendered into HTML"

# form

u->c: "click cat-pic link"
c->s: "HTTP GET / request"
s-->c: "200 OK - HTML form"
u->c: "enter email and click submit"
c->s: "HTTP POST / send form data"
s-->c: "200 OK Thanks! HTML"
c-->u: "HTML rendered"
```
