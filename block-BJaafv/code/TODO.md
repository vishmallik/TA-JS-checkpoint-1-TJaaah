1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
} //

// second
function sum(a, b) {
  console.log(a + b);
} //the first function will return the sum of a+b and display the value in console and the second function will log the value the value a+b in console but will return undefined as value.
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   //value of first will be a+b
   //value of second will undefined

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   //output will be 36 and third argument will be ignored.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   //yes, we can store the `sum` function in `add` variable

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function  sayHello(name){
  return `Hello ${name};
}
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage(); //'Hello, John
```

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // 'John'

showMessage(); // 'Hello, John'

alert(userName); // 'John'
```

8. What is a Anonymous Function give example of three functions.
   Anonymous function is a function which doesnt have a function name associated with it.

```js
sum = function (a, b) {
  return a + b;
};
```

```js
diff = function (a, b) {
  return a - b;
};
```

```js
mul = function (a, b) {
  return a * b;
};
```

9. Can function declaration be a Anonymous Function? Explain

   Anonymous is a function which doesnt have function name and function declaration have function name in its syntax, so, function declaration cannot be a Anonymous function.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

a. getSum
b. calcSquare
c. checkIfPrime
d. checkIfLarger
e. addString
