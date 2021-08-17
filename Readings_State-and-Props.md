[Home](README.md)

# Readings: State and Props
###### React lifecycle
---------------

  1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? Answers taken from source below<sup>1</sup>

     Render occurs first. 
  2. What is the very first thing to happen in the lifecycle of React?

     The very first thing that happens is *Mounting*. In this phase a component is created and inserted into the DOM.

  3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates. 
  
    The correct order is constructor -> render -> React updates -> ComponentDidMount -> ComponentWillUnmount
    
  4. What does componentDidMount do?

     This is a method that is invoked when the component is rendered into the DOM for the first time, which is almost at the start of the component lifecycle.  


###### React State Vs Props
---------------
    Answers taken fom source below <sup>2</sup>
    1. What types of things can you pass in the props?
       Values that can be used for initialization or values used for the rendering of a component are often passed to props. This similar to how the arguments of a function are used.
    
    2. What is the big difference between props and state?
       Props are passed down into a component. State is handled within a component itself.
    
    3. When do we re-render our application?
       When the state of a component is changed, it re-renders.

    4. What are some examples of things that we could store in state?
       Use state to store anything that will cause the component to re-render based of actions a user of the app takes. All data that needs to be handled inside a component itself, should be state. This could be form data, a counter, etc.

    
## Things I want to know more about
---------------
* When to use various lifecycle methods via examples. 
* What is meant in the article below about setting up subscriptions in componentDidMount.

###### Works Cited
<sup>1</sup> Blankenship, Joshua _React: Component Lifecycle Events_, Medium Jul 8 2021, https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093
<sup>2</sup> Web Dev Simplified. “React State Vs Props.” YouTube, uploaded by Big Think, Aug 27 2019, https://www.youtube.com/watch?v=IYvD9oBCuJI.