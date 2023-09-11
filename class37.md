# Redux - Combined Reducers

## Multiple Reducers Example

### 1.Why create multiple reducers?

in order to manage multiple states in a large scale project

### 2.How would you combine multiple reducers?

by using combineReducers() function

### 3.How will you manage state as an immutable object? why?

using a new object and using a spread operator to handle the state variable, because if we cange the property directly it will affect the original state instead of replacing it with a new state object.

## Redux Docs: Using Combined Reducers

### 1.combineReducers is a utility function to simplify the most common use case when writing ___ _____ .

Redux reducers

### 2.Explain how combineReducers assembles the new state tree.

combineReducers will call each slice reducer with its current slice of state and the current action, giving the slice reducer a chance to respond and update its slice of state if needed. So, in that sense, using combineReducers does "call all reducers", or at least all of the slice reducers it is wrapping.

### 3.How would you define initial state in an app using combineReducers?

There are two main ways to initialize state for your application. The createStore method can accept an optional preloadedState value as its second argument. Reducers can also specify an initial value by looking for an incoming state argument that is undefined, and returning the value they'd like to use as a default. This can either be done with an explicit check inside the reducer, or by using the ES6 default argument value syntax: function myReducer(state = someDefaultValue, action)

## Redux Docs: Combined Reducer Syntax

### 1.Why will you want to split your reducing functions as your app becomes more complex?

As your app grows more complex, you'll want to split your reducing function into separate functions, each managing independent parts of the state.

### 2.The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.

combineReducers / createStore

### 3.What is a popular convention when naming reducers?

A popular convention is to name reducers after the state slices they manage, so you can use ES6 property shorthand notation: combineReducers({ counter, todos }). This is equivalent to writing combineReducers({ counter: counter, todos: todos }).