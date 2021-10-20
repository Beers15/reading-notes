[Home](README.md)

# Readings: Node Ecosystem, TDD, CI/CD

### Review, Research, and Discussion
---------------
1. Describe (in plain English) what Array.map() does<sup>1</sup>

    When used on an array this method calls the passed in callback function one time for each element in the array. The element itself is used as the argument to the callback. Basically, the returned value from each call builds a new array from all the elements of the original and this array is what's returned.

2. Describe (in plain English) what Array.reduce() does<sup>1</sup>

    When used on an array this method calls the passed in callback function one time for each element in the array. The accumulated result and the current value are used as the arguments to the callback. The return value from each iteration of the callback being called represents the accumulated value. At the end of this, the array should be boiled down into a single value. (e. g. getting the sum from an array of ints)

3. Provide code snippets showing how to use superagent() to fetch data from a URL and log the result 

  * With normal Promise:
```
super.get(`https://someCityAPI/${cityName}`)
  .then(res => console.log(data.body.lat, data.body.long))
  .catch(err => console.log(err));
```

  * With Async Await:
```
try {
  const data = await superagent.get(`https://someCityAPi/${cityName}`);
  console.log(data.body.lat, data.body.long);
} catch(err) {
  console.log(err);
}
```

4. Explain promises as though you were mentoring a Code 301 level student

    A promise is an object that represents the eventual resolution or rejection of some asynchronous operation and therefore is very commonly used with them in js as an alternative to callback function. This object has 3 states, pending, fufilled, and rejected. Code can be written to handle either a fufilled or rejected state once the operation is no longer represented as 'pending' by the promise object by using async/await syntax or promise instance methods. <sup>2</sup>

5. Are all callback functions considered to be Asynchronous? Why or Why Not?

    They are not asynchronous themselves, but are used for asynchronous behaviors. To elaborate, when a higher order function is passed a callback function, it can call the callback as needed after it completes some task. Outside that higher order function, execution can continue onwards before the callback that was passed is triggered.

## Things I want to know more about
---------------
* I would like to learn more about how to use static promise methods and some of their applications.

###### Works Cited 
---------------
<sup>1</sup> MDN Web Docs, _Array_, https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

<sup>2</sup> MDN Web Docs, _Promise_, https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise
