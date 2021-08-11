[Home](README.md)

# Readings: Introduction to React and Components
###### Component Based Architecture
---------------
  1. What is a component?  
     A component is a modular, portable, replaceable, and reusable set of well-defined functionality that encapsulates its implementation and exporting it as a higher-level interface.<sup>1</sup> 

     In the case of React, a component is a reusable chunk of code that will be rendered on the webpage.

  2. What are the charactistics of a component?
     The characteristics of components are the following: <sup>1<sup>
     * Reusability
     * Replacable
     * Not context specific
     * Extensible
     * Encapsulated
     * Independent 

  3. What are the advantages of using component based architecture?
      The advantages are the following: <sup>1<sup>
      * Ease of deployment
      * Reduced Cost
      * Ease of development
      * Reusable
      * Modification of technical complexity
      * Reliability
      * System maintenance and evolution
      * Independent
      

###### What is Props and how to use it in React?
---------------
  1. What is props short for?
    - Props is short for properties. 

  2. How are props used in React? 
    - They are used 
     "for passing data from one component to another"<sup>2</sup>

  3. What is the flow of props?
    - They flow in one direction. That is, they flow from a component **down** towards subcomponents in a component hiearchy. A component's data, or state, can flow from itself to a subcomponent and that subcomponent can access that data though the props object argument (fnc component) or this.props (class component). 

## Things I want to know more about
---------------
* More on when class components should be used vs fnc components and vice-versa
* Why exactly React isn't a framework aside from not being robust enough.
* Differences between objected-oriented, conventional, and process-related views for components, via examples.
* Component level design
* Props are how the state is passed down to children components. Since props are read-only, what are some good ways to pass the state/data up to parent components? (without Redux)


###### Works Cited
<sup>1</sup> tutorialspoint, _Component-Based Architecture_, 2021, https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm

<sup>2</sup> Eygi, Cem _What is “Props” and how to use it in React?_, ITNEXT, Medium, 7 Oct 2019, https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0#:~:text=%E2%80%9CProps%E2%80%9D%20is%20a%20special%20keyword,way%20from%20parent%20to%20child
