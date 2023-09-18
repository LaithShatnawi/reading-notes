# Additional Topics

## Redux Toolkit (RTK)

### 1.What concerns are addressed by Redux Toolkit?

It was originally created to help address three common concerns about Redux:

"Configuring a Redux store is too complicated"

"I have to add a lot of packages to get Redux to do anything useful"

"Redux requires too much boilerplate code"

### 2.What does configureStore() do?

wraps createStore to provide simplified configuration options and good defaults. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

### 3.How would I use createSlice()?

A function that accepts an initial state, an object of reducer functions, and a "slice name", and automatically generates action creators and action types that correspond to the reducers and state.

## MobX

### 1.What is Mobx?

MobX is a simple, scalable and battle tested state management solution. This tutorial will teach you all the important concepts of MobX in ten minutes. MobX is a standalone library, but most people are using it with React and this tutorial focuses on that combination.

### 2.How does MobX make it “impossible” to produce an inconsistent state?

Finally there are actions. Actions are all the things that alter the state. MobX will make sure that all changes to the application state caused by your actions are automatically processed by all derivations and reactions. Synchronously and glitch-free.

### 3.How would we build a reactive user interface?

Luckily that is exactly what MobX can do for us. Automatically execute code that solely depends on state. So that our report function updates automatically, just like a chart in a spreadsheet. To achieve that, the TodoStore has to become observable so that MobX can track all the changes that are being made. Let's alter the class just enough to achieve that.

Also, the completedTodosCount property could be derived automatically from the todo list. By using the observable and computed annotations we can introduce observable properties on an object. In the example below we use makeObservable to show the annotations explicitly, but we could have used makeAutoObservable(this) instead to simplify this process.

## Tutorial

### 1.What take-away(s) did this tutorial provide?

The Redux Toolkit Quick Start tutorial briefly shows how to add and use Redux Toolkit in a React application.

The Redux Essentials tutorial teaches you "how to use Redux the right way", using Redux Toolkit as the standard approach for writing Redux logic.

It shows how to build a "real world"-style example application, and teaches Redux concepts along the way.