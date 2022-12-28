# Component
**A component is a software object that is an architectural and portable set of replaceable and reusable functions and is intended to interact with other components. It is a configuration unit with a contractually defined interface. The component has three different views: an object-oriented view, a traditional view, and a process-related view.
The component has many properties, including:**
-	Reusability: components are designed to be reused in different situations in different applications
-	Components can be freely replaced by others
-	It is not context-specific as the components are designed to work in different environments and contexts
-	Extensible 
-	Encapsulated 
-	Independent standalone components are designed to have minimal dependencies on other components.
Advantages of using component-based architecture:
-	Component-based architecture reduces development and maintenance costs.
-	It is reusable which means that it can be used for reusable components to spread the cost of development and maintenance across many applications.
-	Increases the reliability of the entire system by reusing.
-	It is easy to maintain and update the implementation without affecting the rest of the system.
-	Modifies complexity using the component container and its services.
-	If new compatible versions are available, it is easy to replace existing versions without any impact on other components.

# Props
**Props are a special keyword in React, which stands for properties and is used to pass data from one component to another. But here is that the data with props is passed in a one-way flow. (one parent-to-child method) Moreover, props data is read-only, which means that data from parents should not be changed by child components.**
props used in React:
-	First, define an attribute and its value (data)
-	Then pass it to the child component(s) using props
-	Finally, view the props data
Props are arguments passed to components and prop is an object.

# Things I want to know more about
***I need to know how works it and research more about it***

# State and Props
## React lifecycle
**1- Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? ***When you follow the drawing, we notice that it is the render that occurs first in the mounting and updating phases, but in the mounting phase, the constructor is created first***.**

**2- What is the very first thing to happen in the lifecycle of React? ***The static getDerivedStateFromProps is the first React lifecycle method***.**

3- **Things that happen in react in order:**
- constructor
- render
- React Updates
- componentWillUnmount

**What does componentDidMount do? ***Here we use componentDidMount() to call the YouTube API and get videos when components are rendered***.**

## React State Vs Props
**1- What types of things can you pass in the props? ***props enable you to pass values from one component to another under the component tree***.**

**2- What is the big difference between props and state? ***The state is internal controlled by the component itself while props are external and controlled by whatever makes the component***.**

**3- When do we re-render our application? ***When the state changes in the parent component, the two Tile components will re-render, even though the second component does not receive any props***.**

**4- What are some examples of things that we could store in state? ***string , number or any complex object***.**

## Things I want to know more about