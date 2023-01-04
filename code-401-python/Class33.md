# Next- Forms and Conditional Rendering 

## Extracting a Custom Hook
A **custom Hook** is a JavaScript function whose name starts with ”use” and that may call other Hooks. For example, useFriendStatus below is our first custom Hook:
        import { useState, useEffect } from 'react';

        function useFriendStatus(friendID) {
        const [isOnline, setIsOnline] = useState(null);

        useEffect(() => {
            function handleStatusChange(status) {
            setIsOnline(status.isOnline);
            }

            ChatAPI.subscribeToFriendStatus(friendID, handleStatusChange);
            return () => {
            ChatAPI.unsubscribeFromFriendStatus(friendID, handleStatusChange);
            };
        });

        return isOnline;
        }

There’s nothing new inside of it — the logic is copied from the components above. Just like in a component, make sure to only call other Hooks unconditionally at the top level of your custom Hook.

Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return. In other words, it’s just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

* The purpose of our useFriendStatus Hook is to subscribe us to a friend’s status. This is why it takes friendID as an argument, and returns whether this friend is online:

        function useFriendStatus(friendID) {
        const [isOnline, setIsOnline] = useState(null);

        // ...

        return isOnline;
        }

## Lifting State Up
In React, sharing state is accomplished by moving it up to the closest common ancestor of the components that need it. This is called “lifting state up”. We will remove the local state from the TemperatureInput and move it into the Calculator instead.



# MEMOIZATION
## WHAT IS MEMOIZATION?
**Memoization** is an optimization technique that allows an increase in the performance of a program by storing the results of some expensive function so that we don’t need to call that function when the same inputs are given.


## HOW TO IMPLEMENT MEMOIZATION IN REACT
React has the features PureComponent and memo hook which allow us to implement memoization in React.
PureComponent allows us to perform optimization. It depends on the shouldComponentUpdate() lifecycle method but it can only be used with the class component.
React also gives us a memo() hook to apply memoization for functional components.
If we need a function component that gives the same result for the same props and we don’t want to re-render it, we can use memoization to skip the re-render of the component by storing and reusing the last rendered result.