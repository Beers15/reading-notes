[Home](README.md)
 
# Readings: Redux - Asynchronous Actions
 
## Review, Research, and Discussion
 
---------------
Answers taken from resources supplied in prompt

1) How granular should your reducers be?

  * They should be granular as reasonably possible. Reducers are supposed to be implemented as pure functions. Have each reducer perform precise actions will help them predictably return a new state.

2) Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched

  * This is a good thing. State values often depends on other state values. With that, a single action will often modify multiple pieces of state and require many events to be performed. Only having to dispatch a single action to do all this allows you to control the behavior of your application more easily.

3) Name a strategy for preventing the above

  * To prevent this you can vary your actions names so that they only trigger multiple reducers when desired? You could also write unit tests to ensure that only the reducers that you want to fire for a specific action are doing so.

### Vocabulary terms

store

  * 'The single source of truth' in Redux. In an ideal Redux + React app, all state is contained in a single object inside of this object. All actions on that state are dispatched to reducers that are part of the store.

combined reducers

  * With Redux you can combine all reducers into a single entity and pass that to a store upon its initialization. With that, an action that is dispatched to that store will be able to be handled by any of the reducers that are combined and put into the store.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * rules of reducers in Redux
    * actions and action creators
    * attaching action creators and state to the props of a component

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Redux middleware, Redux Thunk
    * Async actions in Redux
    * Handling state management with Redux in large scale apps
 
3) What are you most excited about trying to implement or see how it works?
 
    * Implementing an applications that handles asynchronous actions within Redux using middleware

--------------

### Resources

https://redux.js.org/tutorials/fundamentals/part-6-async-logic

https://github.com/reduxjs/redux-thunk

https://www.digitalocean.com/community/tutorials/redux-redux-thunk

https://redux.js.org/faq/actions#should-i-dispatch-multiple-actions-in-a-row-from-one-action-creator