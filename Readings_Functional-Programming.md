[Home](README.md)

# Readings: NODE.js

### Functional Programming Concepts
---------------

Referenced the source below for answers<sup>1<sup>

1. What is functional programming?

   It is a programming paradigm where programs are composed of functions. In this paradigm mutable data and change state is avoided.

2. What is a pure function and how do we know if something is a pure function?

   A function is considered pure if it *always* returns the same result when provided the same arguments and it doesn't have any 'side effects'. Side effects here means the functions requires something outside of its provided arguments and contents to execute.  

3. What are the benefits of a pure function?
   Testing code is easier since code that follows this paradigm is generally free of side effects.
   

4. What is immutability?

   Data is immutable if its state can't be changed after creation. Create a new object with the needed values if change is needed.

5. What is Referential transparency?

   "pure functions + immutable data = referential transparency"<sup>1</sup>


### Node JS Tutorial for Beginners #6 - Modules and require()
---------------

Referenced the source below for answers<sup>2<sup>

1. What is a module?

   A javascript file that contains seperated, related logic.

2. What does the word ‘require’ do?

   This keyword allows you to put other modules into your program for use.


3. How do we bring another module into the file the we are working in?

  The require fnc allows you to do this. Supply the installed package or the path to a local modules as an argument.


4. What do we have to do to make a module available?

   In the file that is to be made into a module, assign whatever needs to be exported to the module.exports object. Then install it from npm or prepend the appropriate path to where it is within our project's code.


## Things I want to know more about
---------------
* Aside from often being easier to test and read, what are some benefits of functional programming?


###### Works Cited

<sup>1</sup> TK, _Concepts of Functional Programming in Javascript_, Medium, Nov 25 2018, https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa

<sup>2</sup> "Node JS Tutorial for Beginners #6 - Modules and require()" YouTube, uploaded by The Net Ninja, May 27 2016, https://www.youtube.com/watch?v=xHLd36QoS4k