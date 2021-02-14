# Week 2

## Goals
- [ ] Understand and apply dependency injection and be able to explain it to others in my cohort
- [ ] Be comfortable test driving more complex projects using OOD principles and techniques
- [ ] Learn the basics of sinatra, html, css
- [ ] Understand and apply forwarding and polymorphism and be able to explain them to others
- [ ] be able to use Twilio to send text messages using Ruby

## Skills learned and applied

- Dependency injection
- All skills from week 1
- Code quality:
  - Mutation testing - ensuring test are actually testing desired behaviour
  - Readability & transparency
  - Complexity reduction
  - Applying metrics tools - linting, complexity, code smells
- Domain modelling
- Sequence diagramming
- Twilio Gem - SMS Messaging

## Practicals completed

- Dependency injection - worked through 3 exercises, refactoring multiple classes through dependency injection to be testable in isolation: [dependency injection](https://github.com/AJ8GH/object-oriented-design/tree/main/dependency-injection)
- Building rspec - created a working version of Rspec from scratch using Ruby: [homemade rspec](https://github.com/AJ8GH/homemade-rspec)
- Testing relationships - exercise in testing class interation, through desired and expected behaviours [testing relationships](https://github.com/AJ8GH/object-oriented-design/tree/main/testing-relationships-between-classes)
- Testing behaviour not state - learnt to test for desired behaviour, over state and implementation: [testing behaviour](https://github.com/AJ8GH/object-oriented-design/tree/main/testing-behaviour-not-state/tic-tac-toe)
- Polymorphism & Duck typing
- Encapsulation

## still to cover:

- Refactoring

## Challenges

### [OYSTERCARD](https://github.com/AJ8GH/oystercard)

Pairing challenge number 2! Our previous client TFL were clearly impressed with our Boris Bikes system. They've now asked to us to design the system for London's Oystercard. This week pairing feels easier and smoother, our coding and communication skills seem to be improving. Techniques applied in the challenge are again focused on TDD and OOD principles, as well as realising a client spec using BDD - domain modelling user stories.   

### [TAKEAWAY](https://github.com/AJ8GH/takeaway-challenge)

The weekend challenge for the week


## Skills Workshops / exercises

### Domain Modelling Workshop

One of the most valuable tools picked up this week has actually been domain modelling using sequence diagrams. It's added a lot more structure to my planning and design process and has really helped crystalise my thoughts before diving into coding and writing tests.

Key take aways:

- Don't get too caught up in building perfect domain model, or designing perfect structure
- It will change, classes and messages can be added or removed later on
- Time has already been saved - quicker and cheaper to change diagrams than code

## [diagram.codes](https://playground.diagram.codes/d/sequence)

### Syntax

- `->` message
- `-->` return value of message
- `alias bank="Bank"` assign variable name bank with value of Bank class
- `user->bank: "deposit(amount)"` user send deposit message to bank with argument `amount`
- `bank->bank: update_balance(amount)` internal procedure / method call

### Bank Account Example

```flow
alias user="User"
alias bank="BankAccount "
alias transaction="Transaction"

user->bank: "opens a bank account: BankAccount.new"

user->bank: "makes a deposit: bank_account.deposit(50)"
  bank->bank: "@balance += amount"

  bank->transaction: "transaction.new(deposit)"
  transaction-->bank: "new instance of trasaction"
  bank->bank: "@transactions << transaction"

user->bank: "makes a withdrawal; bank_account.withdraw(30)"
  bank->bank: "@balance -= amount"

user->bank: "requests to view balance: print_statement()"
  bank-->user: "displays balance: String"
```

### Notebook Exercise

```flow
alias user="User"
alias notebook="NoteBook"
alias note="Note"

user->notebook: "NoteBook.new"
notebook-->user: "notebook instance"

user->notebook: "add_note(info: 'info', tag: 'tag')"
notebook->note: "Note.new(info)"
note-->notebook: "new Note instance"
notebook->notebook: "@notes << note"

user->notebook: "search(tag)"
notebook->notebook: "find_notes(tag)"
notebook-->user: "desired notes"
```
