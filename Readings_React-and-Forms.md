[Home](README.md)

# Readings: React and Forms

### React Docs - Forms
---------------

Referenced the source below for answers<sup>1<sup>

1. What is a ‘Controlled Component’?

  A controlled component is a form element where the data is controlled by React, as the component's state. This makes "the React state the source of truth".<sup>1<sup>

2. Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.

  We should store the value of a form as soon as a user enters them. This is done so that React can immediately update its state as. I would assume this is also done so that React can quickly re-render the appropriate content, resulting in a highly responsive application.


3. How do we target what the user is entering if we have an event handler on an input field?

  We do this by passing an event parameter to the method that an event handle attribute was passed (for example, onChange={handleChange} ). We then can reference what the user is entering with 'e.target.value'

  handleChange(e) {
    this.setState({myStateField: e.target.value});
  }



### The Conditional (Ternary) Operator Explained
---------------

1. Why would we use a ternary operator?

    It allows if else logic to be condensed into a single line expression (although it can be multiple lines). This is useful when embedding js expressions in React components or using arrow functions.

2. Rewrite the following statement using a ternary statement:

    if(x===y){
    console.log(true);
    } else {
    console.log(false);
    }

  **x === y ? console.log(true) : console.log(false)**



## Things I want to know more about
---------------
* In the React documentation reading on forms, why do we need to bind this for event handler methods in a class component (inside the constructor)?
  
  For example: 
  this.handleChange = this.handleChange.bind(this);
  this.handleSubmit = this.handleSubmit.bind(this);

###### Works Cited
<sup>1</sup> _Forms_, React, https://reactjs.org/docs/forms.html Accessed 16 Aug 2021.
