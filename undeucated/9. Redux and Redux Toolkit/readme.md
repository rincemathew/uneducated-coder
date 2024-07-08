# Redux

### What is Redux?
Redux is a state management library for JavaScript applications, commonly used with React but also usable with other JavaScript frameworks or vanilla JavaScript. It provides a predictable state container to help manage the state of your application in a more structured and maintainable way.

OR

Redux is a powerful tool for managing state in JavaScript applications. It provides a structured and predictable way to manage state, improving maintainability, debugging capabilities, and ease of testing. While it introduces some boilerplate, the benefits it brings to large and complex applications often outweigh the initial setup cost.

Key Concepts of Redux
1. Store: The central repository for all state in a Redux application. The store holds the entire state tree of the application. There is only one store in a Redux application.

2. Actions: Plain JavaScript objects that represent an intention to change the state. Each action has a type property that indicates the type of action being performed, and it can have additional properties to provide context or data for the state change.

3. Reducers: Pure functions that take the current state and an action as arguments and return a new state. Reducers specify how the application's state changes in response to actions sent to the store.

4. Dispatch: A function used to send actions to the store. The store's reducer processes the action and updates the state accordingly.

5. Selectors: Functions that extract and derive specific pieces of data from the state.

### Why Use Redux?
Predictability of State: Since the state is always managed in a consistent way, it becomes predictable. Every state change follows strict rules defined by reducers, making the application's state transitions easy to follow and debug.

Centralized State Management: Redux centralizes the application's state, making it easier to understand, manage, and debug. All state changes are recorded in one place, reducing the complexity of state management.

Time-Travel Debugging: Tools like Redux DevTools allow developers to step back and forth through state changes, providing powerful debugging capabilities.

Ease of Testing: Reducers are pure functions, which means they are easy to test. You simply provide the current state and an action, and check the new state returned by the reducer.

Improved Code Maintainability: By organizing state management logic in actions, reducers, and the store, the codebase becomes more modular and easier to maintain. Changes to the state management logic are localized and easier to reason about.

State Sharing Across Components: Redux makes it straightforward to share state across different parts of the application, avoiding prop drilling (passing data through multiple layers of components) and making the code cleaner.

### Plain Javascript Example..

``` html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Redux</title>
</head>
<body>
    <button id="increment">Increment</button>
    <label id="value">--</label>
    <button id="decrement">Decrement</button>
</body>
<script src="index.js" type="module"></script>
</html>
```

``` javascript
import {createStore} from 'https://cdn.skypack.dev/redux@5.0.1';

const initialState = {
    value: 0
}

//function reducer
function appReducer(prevState = initialState, action) {
    switch(action.type) {
        case 'increment':
            return {
                ...prevState,
                value: prevState.value + 1
            };
        case 'decrement':
            return {
                ...prevState,
                value: prevState.value - 1
            };
        default:
            return prevState;
    }
}

//creating a store
const store = createStore(appReducer);

const state = store.getState();

//subscribe
store.subscribe(()=>{
    document.getElementById('value').innerText = store.getState().value;
});

document.getElementById('value').innerText = state.value;

document.getElementById('increment').onclick = ()=>{
    //dispatching actions
    store.dispatch({
        type:'increment',
    });
}

document.getElementById('decrement').onclick = ()=>{
    //dispatching actions
    store.dispatch({
        type:'decrement'
    });
}

```


This can update state asynchronously using “Think”
Mutable sate update using “immer”



How to install?
Install ‘redux’ and ‘react-redux’
Create a store.

Reducers actions dispatch

store - state getState()
dispatch() - change state
subscripton - when state changes subscription calls
Reducer function