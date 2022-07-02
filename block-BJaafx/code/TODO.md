1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
let total = 0;
for (let i = 1; i <= 10; i++) {
  let value = +prompt(`Enter value ${i}:`);
  total = total + value;
}
console.log(total / 10);
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println("hi");
  i++;
} //uncaught referenceerror: println is not defined, there is no function as println in javascript
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10) {
  var i = 0;
  var sum = 0;
  while (i <= max) {
    if (i % 2 === 0) {
      sum = sum + i;
    }
    i++;
  }
  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10) {
  var i = 0;
  var sum = 0;
  while (i <= max) {
    if (i % 2 === 1) {
      sum = sum + i;
    }
    i++;
  }
  return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num) {
  let product = 1;

  while (num != 0) {
    product = product * (num % 10);
    num = Math.floor(num / 10);
  }
  return product;
}
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // "Bigger than 5"
check(1); // "Smaller than 5"
check(5); //5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // "You are arya" since argument Arya matches with first condition so first command will get executed.
getOutput("John"); // "You are john" since argument John matches with second condition so second command will get executed.
getOutput(); // "Who are you" since there is no default parameter set so undefined will be default value and it doesnt match with any condition so last return will get executed.
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // "Who are you" since there is no return command in conditional statements, so "You are arya" will be logged into console but the output of the function will be "Who are you?".
getOutput("John"); //"Who are you" since there is no return command in conditional statements, so "You are john" will be logged into console but the output of the function will be "Who are you?".
getOutput(); // "Who are you" since there is no default parameter set so undefined will be default value and it doesnt match with any condition so last return will get executed.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
   Yes a function can have multiple return statement. conditionals statements can have multiple return statement for each condition. Also we can use multiple return statement in a function but only the first one will be executed and others will get ignored.
   eg:

```js
function getSum(a, b) {
  if (a % 2 == 0 && b % 2 == 0) {
    return a + b;
  } else {
    return a - b;
  }
}
```

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
    for loop is used when we already know all three things initialisation, condition and increment/decrement and how many times the iteration will run but when we know only about the condition and dont know how many times the iteration will run we should use while loop as it only requires the condition for which the loop remains true.
    eg :

```js
for (let i = 0; i < 7; i++) {
  console.log("Hello World");
}
```

```js
let x = 0;
let y = 0;

while (x < 4) {
  x++;
  y += x;
}
```
