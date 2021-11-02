[Home](README.md)
 
# Readings: Socket.io
 
## Review, Research, and Discussion
 
---------------
All answers taken from resources supplied in prompt

1) What is the benefit of transforming data into packets?

    It allows data to be broken up and sent in pieces while still maintaining data integrity and information about the sender and receiver. 

2) UDP is often refereed to as a connection-less protocol. Why is this?

    This type of protocol requires no connection to be established before data can be transferred. There is no acknowledgement to the sender that data was received. 

3) Can a socket server application have multiple socket connections?

    Yes

4) Can a socket connection application be connected to multiple socket servers?

    Yes

5) Can an application be both a socket server and a socket connection?

    Yes

### Vocabulary terms


Observer Pattern <sup>1</sup>

  * This is a design pattern that consists of a subject and its observers. The subject will notify its observers as needed. The observers are capable of receiving such notifications.

Listener

  * A function that is set up to listen for a specific event and fires off an event handler when that event occurs

Event Handler

  * A function that is executed in response to a specific event being fired within its scope

Event Driven Programming 

  * A programming paradigm where the execution of a program is based off of events and handlers that respond to those events

Event Loop <sup>3</sup>

  * Checks if the call stack is empty. If it's empty the loop grabs something off the event queue and pushes it on the stack to get executed.

Event Queue <sup>3</sup>

  * In JS, this is the queue where asynchronous code is pushed to by Web APIs that work in conjunction with the a runtime environment. 

Call Stack <sup>3</sup>

  * The JS interpreter is single threaded and pushes function calls to the call stack which is contained in the JS runtime environment.

Emit/Raise/Trigger

  * Emit fires off a custom event. Raise and trigger are likely other words for doing so when using libraries outside Node.js.

Subscribe

  * Event driven applications can have clients subscribe to a publisher. In other words, clients can listen for a subject to fire off an event and in doing so they are subscribing to that subject (aka publisher).

database

  * A data structure that stores information in some organized manner

### Preview

1) Which 3 things had you heard about previously and now have better clarity on?
  
    Event driven programming, Socket.io, and the event loop + call stack + event queue, etc


2) Which 3 things are you hoping to learn more about in the upcoming lecture/demo?

    OSI and its layers
 
    Building more apps with Socket.io

    Implementing the observer pattern
 
3) What are you most excited about trying to implement or see how it works?
 
    Implementing complex real time applications using WebSocket architecture
 
#### Works Cited
 
<sup>1</sup> Magionami, Alessandro, _Node Observer Pattern _, DEV, Jan 20 2020, https://dev.to/alemagio/node-observer-pattern-27oj

<sup>2</sup> EK, Chris, _JavaScript's Call Stack, Callback Queue, and Event Loop_, Cek.io, Dec 3 2015, https://cek.io/blog/2015/12/03/event-loop/