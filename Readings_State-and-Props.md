[Home](README.md)

# Readings: State and Props
###### React lifecycle
---------------

  1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? Answers taken from source below<sup>1</sup>

     Render occurs first. 
  2. What is the very first thing to happen in the lifecycle of React?

     The very first thing that happens is *Mounting*. In this phase a component is created and inserted into the DOM.

  3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates
     The correct order is constructor -> render -> ComponentDidMount -> ComponentDidUpdate
  4. What does componentDidMount do?

     This is a method that is invoked when the component is rendered into the DOM for the first time, which is almost at the start of the component lifecycle.  

    
## Things I want to know more about
---------------
* When to use various lifecycle methods via examples. 
* What is meant in the article below about setting up subscriptions in componentDidMount.

###### Works Cited
<sup>1</sup> Blankenship, Joshua _React: Component Lifecycle Events_, Medium Jul 8 2021, https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093
