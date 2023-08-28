# Context API - Behaviors

## Scaling Up with Reducer and Context

### 1.How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose.)

In a small example like this, this works well, but if you have tens or hundreds of components in the middle, passing down all state and functions can be quite frustrating!

This is why, as an alternative to passing them through props, you might want to put both the tasks state and the dispatch function into context. This way, any component below TaskApp in the tree can read the tasks and dispatch actions without the repetitive “prop drilling”.

Here is how you can combine a reducer with context:

1. Create the context.

2. Put state and dispatch into context.

3. Use context anywhere in the tree.

The useReducer Hook returns the current tasks and the dispatch function that lets you update them:

const [tasks, dispatch] = useReducer(tasksReducer, initialTasks);

To pass them down the tree, you will create two separate contexts:

TasksContext provides the current list of tasks.
TasksDispatchContext provides the function that lets components dispatch actions.

Export them from a separate file so that you can later import them from other files:

Now you can import both contexts in your TaskApp component. Take the tasks and dispatch returned by useReducer() and provide them to the entire tree

Now you don’t need to pass the list of tasks or the event handlers down the tree:

Instead, any component that needs the task list can read it from the TaskContext:

To update the task list, any component can read the dispatch function from context and call it:

The state still “lives” in the top-level TaskApp component, managed with useReducer. But its tasks and dispatch are now available to every component below in the tree by importing and using these contexts.