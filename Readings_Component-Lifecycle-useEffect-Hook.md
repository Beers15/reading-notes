[Home](README.md)
 
# Readings: Component Lifecycle / useEffect() Hook
 
## Review, Research, and Discussion
 
---------------
All answers taken from resources supplied in prompt

1) Why do we not need more .html pages in a multi-page React app?

  * React can render a single component into the DOM using the ReactDOM.render method. By convention, this is all inserted into a single div with the id of 'root' which is contained in a html file named 'index.html'.

2) If we wanted a component to show up on every page, where would we put it and why? 

  * Inside a <Route />: The <BrowserRouter /> component defines link components that change the url when they are interacted with. The  <Route /> component actually renders the page with children component provided when the path supplied to its 'path' attribute is visited. <Route path="/"><YourComponent /></Route> would render a component on every page, since every path has a "/" at the beginning (using exact path="/" would avoid this behavior).

### Vocabulary terms

State Hook

  * A state hook lets functional component use state (and other) features that are typically reserved for class components.

Mounting and Un-Mounting

  * Mounting is when a component is inserted into the DOM in React. Un-mounting is simply when it's removed from the DOM.

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    *  State hooks, mounting and un-mounting, routing in React


2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    * Routing in React
 
    * Performing lifecycle actions with state hooks in functional components

    * How React works behind the scenes, e.g. how it uses a virtual dom to sync with the actual DOM for more responsive re-renders, etc.
 
3) What are you most excited about trying to implement or see how it works?
 
    * Creating highly responsive front-ends with React

--------------

### Resources

https://reactjs.org/docs/hooks-effect.html

https://v5.reactrouter.com/web/example

https://reactjs.org/docs/hooks-state.html