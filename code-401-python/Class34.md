# Context API

## What is global state with React?

In React, originally, the state is held and modified within the same React component. In most applications, different components may need to access and update the same state. This is achieved by introducing the global states in your app. The main purpose of the global state is to share a state among multiple components.
### There are three ways this communication can happen:

* With a child component
* With a parent component
* With a sibling component



## When to Use Context
**Context** is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. **Context** is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult.

## Context API
**Context API** is a built-in React tool that does not influence the final bundle size, and is integrated by design.

### To use the Context API, you have to:
1. Create the Context

`const Context = createContext(MockData);`

2. Create a Provider for the Context

        const Parent = () => {
            return (
                <Context.Provider value={initialValue}>
                    <Children/>
                </Context.Provider>
            )
        }

3. Consume the data in the Context

        const Child = () => {
            const contextData = useContext(Context);
            // use the data
            // ...
        }

## Redux
**Redux** is an Open Source Library which provides a central store, and actions to modify the store. It can be used with any project using JavaScript or TypeScript, but since we are comparing it to Context API, so we will stick to React-based Applications.

### To use Redux you need to:

1. Create a Reducer

        import { createSlice } from "@reduxjs/toolkit";

        export const slice = createSlice({
            name: "slice-name",
            initialState: {
                // ...
            },
            reducers: {
                func01: (state) => {
                    // ...
                },
            }
        });

        export const { func01 } = slice.actions;
        export default slice.reducer;

2. Configure the Store

        import { configureStore } from "@reduxjs/toolkit";
        import reducer from "./reducer";

        export default configureStore({
            reducer: {
                reducer: reducer
            }
        });

3. Make the Store available for data consumption

        import React from 'react';
        import ReactDOM from 'react-dom';
        import { Provider } from 'react-redux';
        import App from './App.jsx'
        import store from './store';

        ReactDOM.render(
            <Provider store={store}>
                <App />
            </Provider>,
            document.getElementById("root")
        );

4. Use State or Dispatch Actions

        import { useSelector, useDispatch } from 'react-redux';
        import { func01 } from './redux/reducer';

        const Component = () => {
            const reducerState = useSelector((state) => state.reducer);
            const dispatch = useDispatch();
            const doSomething = () = > dispatch(func01)  
            return (
                <>
                    {/* ... */}
                </>
            );
        }
        export default Component;

| Context API   |    Redux      |
| ------------- | ------------- |
| Built-in tool that ships with React	                                                  | Additional installation Required, driving up the final bundle size                    |
| Requires minimal Setup                                                                  | Requires extensive setup to integrate it with a React Application                     |
| Specifically designed for static data, that is not often refreshed or updated	          | Works like a charm with both static and dynamic data                                  |
| Adding new contexts requires creation from scratch	                                  | Easily extendible due to the ease of adding new data/actions after the initial setup  |
| Debugging can be hard in highly nested React Component Structure even with Dev Tool	  | Incredibly powerful Redux Dev Tools to ease debugging                                 |
| UI logic and State Management Logic are in the same component	                          | Better code organization with separate UI logic and State Management Logic            |
