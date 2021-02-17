# Week 3

Started the week with learning about building basic web applications

Debugging - fixed a bug which was preventing puma from running with Sinatra using Shotgun. Submitted a pull request with the gem's repo.

## Practicals completed
- Sinatra pills
- Servers 1
- Clients 1
- HTTP Servers

## Key Skills learned
- Setting up a web app with Sinatra
- Setting up testing infrastructure for web apps using capybara and rspec
- Using webdriver with capybara
- MVC: organising code into model-view-controller structure
- HTML: building web pages using html
- CSS: applying styling to web pages
- erb: combining HTML and CSS with ruby code using erb

## Pairing challenge

### [Battle](https://github.com/AJ8GH/battle)

## Weekend Challenge

### [Rock Paper Scissors](https://github.com/AJ8GH/rps-challenge)

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
