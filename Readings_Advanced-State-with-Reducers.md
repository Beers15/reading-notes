[Home](README.md)
 
# Readings: Component Lifecycle / useEffect() Hook
 
## Review, Research, and Discussion
 
---------------

1) How can we ensure that an effect hook runs only once?

  * The optional 2nd array argument for this hook is an array that contains the dependencies for the hook. State-like variables passed into this array trigger the hook to re-run when they are updated. By supplying an empty argument it will only a single time.

2) Can useState() update more than one state variable at the same time?

  * No, but it can be called multiple times to update more than one state variable.

3) Is useState() synchronous?

  * No, it is asynchronous for performance reasons. Behind the scenes React actually sends proposed changes to a queue when using useState. The state object is not modified directly by this method.

### Vocabulary terms

State Hook

  * A state hook lets functional component use state (and other) features that are typically reserved for class components.

Component Lifecycle

  * The 3 mains stages of a component's life starting with its rendering to the DOM, and ending with it being removed from the DOM. 3 main stages: Mounting, Updating, Un-mounting. React has a sequence of built in methods that get called at each stage that can be used to perform actions at a certain point in the component's life.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * Component lifecycle
    
    * state hooks
    
    * state management in React

2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Actions and Reducers with regards to Redux
 
    * using the useReducer hook, and how its an alternative to Redux

    * reducer functions
 
3) What are you most excited about trying to implement or see how it works?
 
    * Writing test using the React-Testing-Library, and making React apps with Redux

--------------

### Resources

https://linguinecode.com/post/why-react-setstate-usestate-does-not-update-immediately

https://www.w3schools.com/react/react_lifecycle.asp

https://reactjs.org/docs/hooks-reference.html#usereducer

https://blog.logrocket.com/guide-to-react-usereducer-hook/