[Home](README.md)
 
# Readings: Context API
 
## Review, Research, and Discussion
 
---------------
All answers taken from resources supplied in prompt

1) Describe use cases useState() vs useReducer()

  * The useReducer hook is more useful in situations where state has a complicated shape, i.e. state that has many sub-values that requires different types of operations to be performed on it. If a state update depends on the previous state, this hook is the better choice as well. The useState hook is still a viable option in many cases since state can often not be complex.

2) Why do custom hooks need the use prefix?

  * I believe this isn't required. React documentation recommends the prefix to help you tell 'at a glance' that the function is meant to be used as a hook.

3) What do custom hooks usually do?

  * They let you hook into React features from a functional component in a way that makes your code more modular. They let you reuse stateful logic.

4) Using any list of custom hooks, research and name one that you think will be useful in your applications

  * useForm: This is a custom hook that I used in my todo app that help me manage a form by extracting logic.

5) Describe how a hook that fetches API data might work

  * A hook that does this (such as a useEffect hook with some dependencies passed in) may perform a fetch call to an API every time that it is triggered.

### Vocabulary terms

reducer

  * A pure function that takes in an action and the previous state and returns a new state after modifying it.


### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    * Custom hooks
    * reducers
    * actions


2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * How to effectively use reducers 
    * How to write custom hooks
    * Redux
 
3) What are you most excited about trying to implement or see how it works?
 
    * Building an app that manages complex state use reducers via the useReducer hook or Redux

--------------

### Resources

https://dev.to/spukas/3-reasons-to-usereducer-over-usestate-43ad

https://reactjs.org/docs/hooks-custom.html

https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b

https://github.com/diegohaz/awesome-react-context

https://reactjs.org/docs/context.html