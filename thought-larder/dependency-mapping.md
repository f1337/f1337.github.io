# Project Dependency Mapping

This is a stub, re-capping a process I recently used to map a complex process at the VA. I borrowed this tool from Michael Keeling, when we worked together at LendingHome. It's similar to the [Event Storming](https://en.wikipedia.org/wiki/Event_storming) method, from DDD. This write-up is incomplete, but hopefully there is enough here to prompt questions. Enjoy, and as always, YMMV!

## Process

- On the far right of the visible area of the board, we made a tall (full-screen height at the start) box labeled _DONE_.
- Beginning with _DONE_, we asked “What needs to happen for the work to be considered _DONE?”_, then we created blue stickies for each _independent_ deliverable, arranging them vertically to the left of _DONE_ (more on this later; don’t worry about perfection).
- For each blue sticky, we then worked our way right to left (backwards), asking “What needs to happen for us to be able to work on that?”. We identified dependencies for each, and dependencies for the dependencies, until the answer was “nothing, we can start now”.

## Method

- Use rows for work _threads_ or _streams_ or whatever you call _sets of interdependent work that are themselves independent of other sets of work_.
- Use columns for iterations: _sprints_ if that’s the term you use.
- Use blue notes for independent deliverables for a particular work stream.
- Use purple to denote the expected, roughly predictable dependencies.
- Use pink notes for risks.
- Use yellow notes for time-boxed activities.

INSERT DRAWING THAT MAKES THE ABOVE MAKE SENSE
<!--stackedit_data:
eyJoaXN0b3J5IjpbMTEzMDQ4MjkzNF19
-->