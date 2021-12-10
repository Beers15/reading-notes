[Home](README.md)
 
# Readings: API Integration
 
## Review, Research, and Discussion
 
---------------
Answers taken from the resources below

1) Why choose Redux instead of the Context API for global state?

  * Context API re-renders all the components it provides to while Redux only does so for the components that actually updated. Redux also allows you to deal with state related logic away from the components that use it. There are also powerful dev tools for Redux. 

2) What is the purpose of a reducer?

  * Reducers can be used to better manage how state is changed.

3) What does an action contain?

  * An action is a js object that contains an action and a payload.

4) Why do we need to copy the state in a reducer?

  * State is supposed to be immutable and unchanged. Reducers are meant to return a new state object every time an action is dispatched to them.

### Vocabulary terms

immutable state

  * Whether its vanilla React or Redux state should not be directly modified and should be left alone. 'Immutable state' is a term used to refer to this. Modifications to state should return an entirely new state to replace the old one since directly changing state can result in unwanted behaviors.

time travel in redux

  * Using various tools, you can load up a previous version of the Redux store and view the app without reloading an application. Or in other words, you can rewind and view the application as it was with a previous version of the redux store's state.

action creator

  * This is a function who's sole purpose is to prepare needed to prepare an action object and return it. This returned object will be dispatched to a reducer.

reducer

  * This is a pure function used in React and Redux. It takes an action and performs a task based of the action's type. It uses the action's payload to modify a previous state by return a new state.

dispatch

  * This is a method provided by redux that sends an action to the redux store. Reducers can then handle that action appropriately. The useReducer hook also can have a dispatch method defined that does something similar for its own state.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?

    * Redux
    * Combining reducers
    * Actions and action creators

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Redux dev tools
    * Combining reducers
    * Use cases for Redux vs Context API
 
3) What are you most excited about trying to implement or see how it works?
 
    * Creating large scale React apps where Redux's configuration complexity ends up being well worth it

--------------

### Resources

https://www.codehousegroup.com/insight-and-inspiration/tech-stream/using-redux-and-context-api

https://medium.com/the-web-tub/time-travel-in-react-redux-apps-using-the-redux-devtools-5e94eba5e7c0

https://www.youtube.com/watch?v=gBER4Or86hE

https://redux.js.org/usage/structuring-reducers/using-combinereducers/

https://redux.js.org/api/combinereducers/