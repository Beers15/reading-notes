[Home](README.md)

# Readings: Passing Functions as Props
###### React Docs - lists and keys
---------------
  Referenced the source below for answers<sup>1<sup>

  1. What does .map() return?

     A new array that is equal in size to the array that called the map method.

  2. If I want to loop through an array and display each value in JSX, how do I do that in React?

      * Call map on the array and pass a callback function as an argument.
      * In the body of that function return a jsx component using the argument passed to the callback, which refers to the current element, as desired. 
      * Assign that return value of the map method to a variable to obtain the resultant array. 
      * Render this variable, or render another jsx element that contains it within it to display the result.

      Example<sup>1<sup>

      const numbers = [1, 2, 3, 4, 5];

      const listItems = numbers.map((number)=> \<li>{number}\</li>);

      ReactDOM.render(\<ul>{listItems}\</ul>, document.getElementById('root'));
    
  3. Each list item needs a unique *key*.

  4. What is the purpose of a key?

    React needs these to help uniquely indentify when an element is changed, added, or removed from an array of elements within a component. _"Keys should be given to the elements inside the array to give the elements a stable identity."_<sup>1<sup> Avoiding using array indexes as keys when possible since elements may rearrange in the array throughout the execution of your program.

###### What is the spread operator?
---------------
  Referenced the source below for answers<sup>2<sup>

  1. List 4 things that the spread operator can do.
     Copy an array, concatenate or combine arrays, add to state in React, combine objects

  2. Give an example of using the spread operator to combine two arrays.
     const arr1 = [1,2,3];  
     const arr2 = [4,5,6];
     const arr3 = [...arr1, ...arr2];

  3. Give an example of using the spread operator to add a new item to an array.
     const arr1 = [1,2,3];  
     const arr2 = [...arr1, 4, 5, 6];

  4. Give an example of using the spread operator to combine two objects into one.
     const obj1 = {foo: 123};
     const obj2 = {bar: "abc"};
     const obj3 = {...obj1, ...obj2}


###### How to Pass Functions Between Components
---------------
  Referenced the source below for answers<sup>3<sup>

  1. In the video, what is the first step that the developer does to pass functions between components?
     The developer creates a function that modifies the state of a component inside the same component. This function will later be passed as a prop to a child component.
     
  2. In your own words, what does the increment function do?
     This function iterates through the people object, which is part of the App component's state. It returns each object inside the people object, only making a modification to the count property of a particular object in people if it matches the name argument that was passed into the increment function. 


  3. How can you pass a method from a parent component into a child component?
     You can pass the function to a component as a prop in the same manner as a prop of any other data type.
  
  4. How does the child component invoke a method that was passed to it from a parent component?
     First, a function is created in the child component which invokes this.props.someParentFunction (or props.someParentFunction if it's a function component). Inside the body of the child component an event handler is set. When this is triggered, it calls the child component's function, which then calls the prop function that was given to it from the parent.
 
## Things I want to know more about
---------------
  * How exactly do keys help React indentify items that have changed, been added, or removed?
  * Refering to the video below, is it necessary to create an extra function to use as an event handler as described in question #4, or can a prop function be set directly as an event handler? 

  For example, in a child component, is \<MyElement onClick={this.props.someParentFunction} /> allowed directly or does there have to be an extra function like in the video \<MyElement onClick={this.someFncThatCallsParentFunction} />?

###### Works Cited
<sup>1</sup> Lists and Keys, React, https://reactjs.org/docs/lists-and-keys.html

<sup>2</sup> Austin, Derek, _How to Use the Spread Operator (…) in JavaScript_, Coding at Dawn, Medium, Oct 4 2019, https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab

<sup>3</sup> Griffith, Steve. "React - How to Pass Functions between Components - Episode 22" YouTube, uploaded by Prof3ssorSt3v3, Oct 22 2018, https://www.youtube.com/watch?v=c05OL7XbwXU