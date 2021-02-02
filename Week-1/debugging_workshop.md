# Debugging 1

## skills-workshops/test_driven_development/debugging_1

### Covered:

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
