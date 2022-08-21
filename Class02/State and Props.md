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