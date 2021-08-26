[Home](README.md)

# Readings: In memory storage

### Understanding the JavaScript Call Stack
---------------

Referenced the source below for answers<sup>1<sup>

1. What is a ‘call’?

  A call is a function invocation.

2. How many ‘calls’ can happen at once?

  As functions are called they are added to the call stack. As they complete they are removed from it. 

3. What does LIFO mean?

  Last In First Out.

4. Draw an example of a call stack and the functions that would to be invoked to generate that call stack.

|1-----|    |1(pop)|   |------|   |------|  

|2-----|    |2-----|   |2(pop)|   |------|   

|3-----|    |3-----|   |3-----|   |3(pop)|

////////    ////////   ////////   //////// 


three calls 2 calls 1, then they finish in revesrse order and pop of the call stack.

function numeroOne(){
  //do something
}

function numeroTwo(){
  numeroOne();
}

function numeroThree(){
  numeroTwo();
}

numeroThree();


5. What causes a Stack Overflow?

  This happens when recursive calls to a function execute continuously without a proper breaking point. The avaiable stack memory fills up and this results in a Stack Overflow.


### JavaScript error messages
---------------

Referenced the source below for answers<sup>2<sup>

1. What is a ‘refrence error’?

  They error occurs if you refer to a variable that is yet to be declared.

2. What is a ‘syntax error’?

  JS code that is not parsable (due to improper syntax) falls under this error type.

3. What is a ‘range error’?

  When there is an attempt to insert a value at a non-existant index within an array this error occurs. 

4. What is a ‘type error’?

  This error happens when arguments to functions are used that are an incompatiable type to what is exected, and when accessing a property of something that is undefined. 

5. What is a breakpoint?

  A conditional stopping point that can be added into your code. Using and IDE you can navigate between breakpoints. They are used to see what the state of you code is up until that point.

6. What does the word ‘debugger’ do in your code?

  Adds a breakpoint into your code.


## Things I want to know more about
---------------
* When handling error in JS, how do you effectively check for errors of different types in the same code block.
* How the Event Loop and Task Queue work


###### Works Cited

<sup>1</sup> Freeborn, Chris, _The JavaScript Call Stack - What It Is and Why It's Necessary_, freeCodeCamp, Jan 11 2018, https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/

<sup>2</sup> Spinola, Diogo, _JavaScript error messages && debugging_, Medium, Jul 17 2017, https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c