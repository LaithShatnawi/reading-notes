# Application State with Redux

## Dan Abramov Redux Tutorials

### 1.What is the first principle of Redux?

everything that changes in your application, including the data and the UI state, is contained in a single object, we call the state or the state tree.

### 2.what is a store and what do we use our reducers for within that store?

This store binds together the three principles of Redux. It holds the current application's state object. It lets you dispatch actions. When you create it, you need to specify the reducer that tells how state is updated with actions.

### 3.Name three Redux store methods given to us by createStore and describe their use.

The first method of this store is called get state. It retrieves the current state of the Redux store. If we were on this, we're going to see zero because this is the initial state of our application.

The second and the most commonly used store method is called dispatch. It lets you dispatch actions to change the state of your application. If we log this store state after dispatch, we're going to see that it has changed.

The third is subscribe, it's lets you register a callback that the Redux store will call any time an action has been dispatched, so that you can update the UI of your application. It will reflect the current application state.

### 4.Explain to a non-technical recruiter what combineReducers() does and why it is useful.

combineReducers() is like a helpful organizer that takes care of combining all the smaller pieces of your application's state management into a neat and manageable package. It's a key tool in making sure your Redux-powered application stays organized and maintainable.