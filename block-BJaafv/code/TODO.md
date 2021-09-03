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
//Difference between first and second function is the output basically first will return the sum as output but second function is printing the sum into the console so we can not assign the value to variable because we are not getting as output from second function.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

//first case: a+b , sum of both input
//Second case: undefined,
3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
//It will ignore the thired parameter because it is having two parameter as input.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
//Yes we can store the function in variable named add because function is treated as object which gives some values so values can be stored that is basically called function expression so we can store the function in var.
exp:
```js
const add = function sum(a,b){
  return a+b;
}
```js

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.
```js
function sayHello(name){
  return `Hello ${name}`;
}


```js
6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
///'Hello,John'
username is globale variable so we will have access inside the function and in message we are storing the string after concatination so when we are calling the function we will have output as 'Hello,John'

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // it will alert the user with following pop up : 'John'

showMessage(); // 'Hello,John'

alert(userName); // it will alert the user with following pop up : 'John'

```

8. What is a Anonymous Function give example of three functions.
Anonymous function is function which does have its name in syntax or function declartion that is called anonymous.
Exp:
1: 
```js
const add = function(a,b){
  return a+b;
}
const sub = function(a,b){
  return a-b;
}
const mul = function(a,b){
  return a*b;
}
 ```



9. Can function declaration be a Anonymous Function? Explain

Yes function declaration can be anonymous , because in above examples we are doing same that is actually function declaration of anonymous.
10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

1: while we are defining somthing the function name should be like what is doing so someone can make sense by its name only if possible.
2: name should not start from capital letter.
3: if it is having more than one word try make second word's first letter in capital letter.
4: name should not be starting with numbers.
Examples:

```js
function convertToString(){}
function getNumber(){}
function calAge(){}
function findName(){}
function calSalary(){}

```
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
