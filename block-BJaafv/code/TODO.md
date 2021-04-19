1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
first function return some values from the function whereas second function does not.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

First function will return either a string type or number type, depend on the parameter you are passing. But second function will always return undefined.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

The function will be terminate normally but only two parameters will execute third will be ignored. SO, the output will be 36.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

Yes you can store the function in a variable name beacuse function can be also treated as a expression.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name){
  return `Hello Arya`;
}
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
The output will be "Hello, John" because userName is an outer variable but can be accessed inside a funcion.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // 'john'

showMessage(); // "Hello, John"

alert(userName); // `john`
```

8. What is a Anonymous Function give example of three functions.

A function without name is called anonymous function. Anonymous function are stored in a variable and always gets invoked with the variable name.

var sum = function(numA, numB){
  return a+b;
}
var div = function(numA, numB){
  console.log(numA/numB);
}

var mul = function(numA, numB){
  console.log(numA*numB);
}

9. Can function declaration be a Anonymous Function? Explain

Nope, beacuse function declaration always has a name and function with name can not be a anonymous function.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```
setElement, getInfo,  removeItem, updateValue, createTable