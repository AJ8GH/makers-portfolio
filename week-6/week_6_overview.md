## Week 6

By the end of the week all developers can:

* Test drive a simple front-end web app with Javascript
* Follow an effective process for learning a new language

### Challenges

* [Afternoons - Thermostat](https://github.com/makersacademy/course/blob/master/thermostat_es6/README.md)
* [End of unit - Bowling continuation in JS](https://github.com/makersacademy/bowling-challenge)

### Practicals

* [Learning a new language by translation](https://hackmd.io/kMNgXiPHQf2Q_P9A-tnS9A)
* [Explore asynchronicity in Javascript](https://github.com/makersacademy/skills-workshops/blob/master/javascript_fundamentals/async_JS.md)
* [Closures](https://hackmd.io/cIFsMAqISHqVHN_-p9hY0Q)

### Resources

* [Count app](https://github.com/maryrosecook/count):
A tiny JavaScript/Sinatra app that mimics the architecture of the Thermostat app. A useful guide for developers to use for concepts and idioms.
* [Technical Learning Resources](https://airtable.com/shrbaXgV5mQnsvuGe/tblokmw6yNUO75ge6?blocks=hide)

### Skills workshops

* [Encapsulation with the constructor & prototype pattern](https://github.com/makersacademy/skills-workshops/tree/master/javascript_fundamentals/encapsulation_with_constructor_and_prototype_pattern)
* [Following the flow and getting visibility](https://github.com/makersacademy/skills-workshops/tree/master/javascript_fundamentals/following_the_flow_and_getting_visibility_in_javascript_es6)
* [Following the Ajax request/response cycle](https://github.com/makersacademy/skills-workshops/tree/master/javascript_fundamentals/following_ajax_request_response_cycle)
* [Callbacks and following the flow of control](https://github.com/makersacademy/skills-workshops/tree/master/javascript_fundamentals/callbacks_following_the_flow_of_control)


# Welcome to JavaScript

## What is JavaScript?

JavaScript is a fully-featured programming language.  It runs in the web browser.  It lets you write web apps that can update the page without a page refresh.

It's a great second language to learn, as it introduces many new language concepts not found in Ruby. It will also let you reinforce concepts you've already learned.

## Goals for the week

Ask yourself the same two questions:

* Are you having fun?

* Are you a better developer than you were yesterday?

By the end of the week, the goal is to be able to answer "yes" to the week's primary question:

* **Can you learn a new language and its patterns?**

By the end of the week all developers can:

* Test drive a simple front-end web app with Javascript
* Follow an effective process for learning a new language

### Check your understanding

To guide your learning, aim to be able to answer "yes" to the questions below.

Return to these questions each day to check your understanding.

#### JavaScript

* Can you read and write JavaScript syntax?

* Can you understand the rules that govern the behaviour of the `this` keyword?

* Can you follow the flow of an Ajax request and response?

* Can you follow the flow of control through code that uses callbacks?

#### Transferring your existing skills

* Can you encapsulate behaviour in JavaScript?

* Can you get visibility effectively in JavaScript?

* Can you TDD in JavaScript?

* Can you follow the flow of control over the whole web app cycle? e.g. the interface of a thermostat is displayed in HTML/CSS, the "increase temperature" button is clicked, a JavaScript click event fires, JavaScript code runs to handle the event, an Ajax request is made, a Sinatra controller POST action handler is run, a Thermostat Ruby model is updated, the new temperature is saved to a Postgres database, the new temperature is returned as JSON by the Ruby controller, JavaScript code runs to update the temperature in the web page.

## The Count projects

The [Count](https://github.com/maryrosecook/count) project is a tiny, model full stack web app.  It exemplifies:

* Making Ajax requests.
* Testing frontend code.
* Separating frontend concerns into model, view and controller.

Here's the simple [Count project rewritten in ES6](https://github.com/dearshrewdwit/count). It exemplifies:
* Making Ajax requests using fetch.
* Separating frontend concerns using a component approach
* Testing frontend code.
* Testing controller responses.

It's very worthwhile spending time investigating and playing with the code in these projects to understand how they work.

## Challenges

### Rewrite fizz buzz and the airport challenge

You'll revisit some familiar exercises to map the knowledge you learnt in the first four weeks to JavaScript: the FizzBuzz kata, followed by translating the Airport challenge.
