[Home](README.md)
 
# Readings: Context API - Behaviors
 
## Review, Research, and Discussion
 
---------------
All answers taken from resources supplied in prompt

1) When you have multiple contexts, what component type should you use (class/function) and why?

  * I believe it would be better to use a functional component. Class components use 'static contextType = ContextThatIsToBeUse' to consume a context's state. As far as I know, this only allows one to be consumed at a time. Functional components use the useContext hooks to do this. This hook can be used multiple times with any number of contexts.

2) What are some good use cases for using the Context API for global state?

  * Any scenario that could benefit from global state. (E.g. theme data, configuration data, auth, user preferences, etc.)

3) How can you best test context?

  * This can be done by using the Jest-based React testing library to write multiple tests that check the UI. Modifying the context values and asserting that the desired result is actually happening is a pretty good way to do this.

### Vocabulary terms

context

  * Context is a newer React feature that allows us to pass state to components on a global scale in a way that does not require explicitly passing values down through a component tree. It uses a context provider that wraps a component to serve state to any component in that tree that consumes it.

useContext()

  * This hook allows a function component to hook into the React Context API. By grabbing a piece of context with this hook, a functional component can consume its global state.

static context

  * I'm unsure on this one. In a class component, 'static contextType = ContextThatIsToBeUse' is how it consumes the state that a provider that is somewhere higher up in the component tree provides.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * useContext Hook
    * React Context API
    * global state management

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Other types of providers in React that have components that consume them.
    * Other use cases for Global state with or without React's Context
    * custom hooks
 
3) What are you most excited about trying to implement or see how it works?
 
    * Building an app that manages global state with Redux instead of React's Context API

--------------

### Resources

https://reactjs.org/docs/context.html

https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b

https://github.com/diegohaz/awesome-react-context