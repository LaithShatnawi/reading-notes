# Redux - Asynchronous Actions

## async actions

### 1.Why use Redux middleware?

By itself, a Redux store doesn't know anything about async logic. It only knows how to synchronously dispatch actions, update the state by calling the root reducer function, and notify the UI that something has changed. Any asynchronicity has to happen outside the store.

### 2.Consider the Redux Async Data Flow Diagram. Describe the flow in your own words.

It starts by the clieant making an event, in which the event handler dispatches an action, that specific action is then received in the midleware and an api request is made, and wait until the response is there then dispatch an action for the reducer to change the state and send it back to the user.

### 3.How are we accommodating async in our Redux app?

Writing async logic as thunk functions allows us to reuse that logic without knowing what Redux store we're using ahead of time.

## thunk middleware

### 1.Why would you need redux-thunk middleware?

For Redux specifically, "thunks" are a pattern of writing functions with logic inside that can interact with a Redux store's dispatch and getState methods.

Using thunks requires the redux-thunk middleware to be added to the Redux store as part of its configuration.

Thunks are a standard approach for writing async logic in Redux apps, and are commonly used for data fetching. However, they can be used for a variety of tasks, and can contain both synchronous and asynchronous logic.

### 2.Redux Thunk middleware allows you to write action creators that return a ____ instead of an action.

function

### 3.Describe how any return value from the inner thunk function will be made available.

Any return value from the inner function will be available as the return value of dispatch itself. This is convenient for orchestrating an asynchronous control flow with thunk action creators dispatching each other and returning Promises to wait for each other’s completion: