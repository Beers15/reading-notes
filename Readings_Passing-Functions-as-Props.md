[Home](README.md)

# Readings: Passing Functions as Props
###### React Docs - lists and keys
---------------

  1. What does .map() return?
     A new array that is equal in size to the array that called the map method.

  2. If I want to loop through an array and display each value in JSX, how do I do that in React?
      * Call map on the array and pass as an argument a callback function that has at least 1 argument.
      * In the body of that function return a jsx component using the argument as desired within the jsx. 
      * Assign that return value of the map method to a variable.
      * Render the variable that contains the result, or render another jsx element that contains the result.

      Example<sup>1<sup>

      const numbers = [1, 2, 3, 4, 5];

      const listItems = numbers.map((number) => <li>{number}</li>);

      ReactDOM.render(<ul>{listItems}</ul>, document.getElementById('root'));
    
  3. Each list item needs a unique *key*.

  4. What is the purpose of a key?

    React needs these to help uniquely indentify when an element is changed, added, or removed from an array of elements within a component. _"Keys should be given to the elements inside the array to give the elements a stable identity."_<sup>1<sup> Avoiding using array indexes as keys when possible since elements may rearrange in the array throughout the execution of your program.

###### What is the spread operator?
---------------
  1. List 4 things that the spread operator can do.


  2. Give an example of using the spread operator to combine two arrays.


  3. Give an example of using the spread operator to add a new item to an array.


  4. Give an example of using the spread operator to combine two objects into one.


---------------
    
## Things I want to know more about
---------------
* How exactly do keys help React indentify items that have changed, been added, or removed?

###### Works Cited
<sup>1</sup> Lists and Keys, React, https://reactjs.org/docs/lists-and-keys.html
<sup>2</sup> Griffith, Steve 