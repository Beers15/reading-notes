[Home](README.md)
 
# Readings: Redux Additional Topics
 
## Review, Research, and Discussion
 
---------------
Some answers taken from the resources below

1) What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

  * One effective way to do this is to use a lifecycle method or hook equivalent in your main container component (like App.js). Upon initial render, that method can retrieve data using an action and dispatch it to the redux store.

2) When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

  * You would export the reducer function, as you normally would. The related action creator would dispatch the created action and all reducers in the store would be able to pick up on that dispatch.

### Vocabulary terms

Middleware

  * Middleware is code that runs between to actions. In terms of Redux, middleware runs after an action is dispatched and before said actions reaches the reducer.

Thunk

  * This is a library that provides Redux middleware. This middleware allows async action creators to be used. In other words async code can interact with the Redux store.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?

    * Redux Thunk
    * Reducers and actions
    * Handling asynchronously in Redux

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Using Redux Toolkit
    * How to use the Alternative State managers provided in the resources below
    * Effectively using other Redux middleware other than Thunk
 
3) What are you most excited about trying to implement or see how it works?
 
    * React apps using state manager alternatives to Redux

--------------

### Resources
https://github.com/reduxjs/redux-thunk

https://mobx.js.org/getting-started.html

https://hookstate.js.org/

https://redux-toolkit.js.org/tutorials/overview