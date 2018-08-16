## Table of Contents

1. [HTML Questions](/questions/html-questions.md)
1. [CSS Questions](/questions/css-questions.md)
1. [JavaScript Questions](/questions/javascript-questions.md)
1. [React Questions](/questions/javascript-questions.md)
1. [MongoDB Questions](/questions/javascript-questions.md)
1. [MySQL Questions](/questions/javascript-questions.md)


***
## HTML Questions



***
## CSS Questions



***
## Javascript Questions

### What is a Higher-order function?


### What is a Callback function?
A Callback function is any function that is passed as an argument and subsequently called by the function that receives it.

Consider the following example in which the setTimeout method is used to simulate a code delay.  

```
function first(){
  // Simulate a code delay
  setTimeout( function(){
    console.log(1);
  }, 500 );
}
function second(){
  console.log(2);
}
first();
second();
```

Notice how Javascript didn't wait for a response from the 'first' function before moving on to execute 'second'.  For this reason, our console logged the following output.

```
// 2
// 1
```

To fix this issue, we can use a callback function.  Callbacks are a way to make sure certain code doesn’t execute until other code has finished execution:

function first(){
  // Simulate a code delay
  setTimeout( function(){
    console.log(1);
  }, 500 );
}

function doHomework(subject, callback) {
  // Simulate a code delay
  setTimeout( function(subject,){
      alert('I am starting my ${subject} homework!')
  callback();
  }, 1500);
}

doHomework('math', function() {
  alert('I just finished my ${subject} homework!')
});










***
## React Questions



***
## MongoDB Questions



***
## MySQL






### Sources
* https://medium.com/@bretdoucette/part-4-what-is-event-delegation-in-javascript-f5c8c0de2983
* https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events
* https://www.sitepoint.com/higher-order-functions-javascript/
netspi