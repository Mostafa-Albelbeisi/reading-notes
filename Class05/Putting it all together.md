# Thinking in React

**1-What is the single responsibility principle and how does it apply to components?** A module should be responsible to one, and only one, actor.

**2- What does it mean to build a ‘static’ version of your application?** I have a library of reusable components that display the data model.

**3- Once you have a static application, what do you need to add?** And add interaction

**4- What are the three questions you can ask to determine if something is state?** 
- Is it passed in from a parent via props?
- Does it remain unchanged over time?
- Can you compute it based on any other state or props in your component?

**5- How can you identify where state needs to live?**
- Identify every component that renders something based on that state.
- Find a common owner component.
- If you can’t find a component where it makes sense to own the state.

# Order Functions
**1-What is a “higher-order function”?**  a function that takes a function as an argument, or returns a function

**2- Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?** It compares the other number if it is greater than it or not.

**3- Explain how either map or reduce operates, with regards to higher-order functions.** Map operates on a list of values in order to produce a new list of values, by applying the same computation to each value. Reduce operates on a list of values to collapse or combine those values into a single value (or some number of values), again by applying the same computation to each value.