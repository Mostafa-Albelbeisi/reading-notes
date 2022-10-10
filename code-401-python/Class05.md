# Intro to OOP

## Classes and Objects:
**Opbject-orinted programming(oop):** is a methodology or paradigm to design a program using classes and object.

## Classes and Objects:
- **Classes:** A classes is a template, prototype, blueprint for objects, and an object is an instance of class.
- **Objects:** An instance is an executable copy of class. Another name for instance is object.


## Thinking Recursively:
A **recursive** function is a function defined in terms of itself via self-referential expressions. This means that the function will continue to call itself and repeat its behavior until some condition is met to return a result.

## Pytest Fixtures and Coverage
**Pytest fixtures** are functions that can be used to manage our apps states and dependencies. Most importantly, they can provide data for testing and a wide range of value types when explicitly called by our testing software. You can use the mock data that fixtures create across multiple tests.

**Coverage.py** is a tool for measuring code coverage of Python programs. It monitors your program, noting which parts of the code have been executed, then analyzes the source to identify code that could have been executed but was not. Coverage measurement is typically used to gauge the effectiveness of tests.
- To install the coverage tools python `-m pip install pytest-cov`
- To run the coverage command: pytest `--cov blackjack --cov-report html`