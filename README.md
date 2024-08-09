# Homework 12

## What is FLUX?

FLUX is a unidirectional data flow pattern used to help manage state within React especially as the application scales. There are four parts to FLUX: dispatcher, stores, actions, and views. The view creates an action (ex. button click) which creates the data associated and is sent to the dispatcher which dispatches the result of the action to the associated store which in turns updates the state associated and sends an update to the view.

## What is Redux? How do you use it with React components?

Redux is a JavaScript library also used to help manage state within React. Using Redux with React is started by creating a Redux store and providing it to React through passing the store as a prop in Provider. Slices and slice reducers can be made with slice reducers can be added to the store to handle updates to certain states. Finally, using React Redux hooks, useSelector and useDispatch, data can be read from the state and actions can be dispatched.

## What is a reducer?

Reducers are functions that create a new state by taking the current state and an action as arguments.

## How do you choose between ContextAPI and Redux for global state management?

ContextAPI are used for applications with basic state management while Redux is better for applications that are more complex as using ContextAPI with complicated states makes it hard to follow changes to the state.

## What is redux thunk and why do you want to use it?

Redux thunk are a pattern in Redux that utilise dispatch and getState to interact with the store. They are mainly used to write async functions and are helpful in moving logic out of components and the UI layer. Thunks also have no restrictions on side effects unlike reducers.
