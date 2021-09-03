1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let sum=0;
for(let i=1;i<=10;i++){
 sum= +promt(`Please enter the number`);
}
let avg=sum/10;
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
///'hi'
///'hi'
///'hi'

```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max=10){
  let sum=0;
  for(let i=1;i<=max;i++)
  {
    if(i%2==0){
      sum+=i;
    }
  }
  return sum;
}



```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js

function getOddSum(max=10){
  let sum=0;
  for(let i=1;i<=max;i++)
  {
    if(i%2!==0){
      sum+=i;
    }
  }
  return sum;
}



```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

```js

function getProductOfDigits(num){
  let product=1;
  
  let temp=num;
  if(num>0){
  for(let i=1;i<=100;i++)
  { 
    product=product* num%10;
    num=num/10;
    
  }
  return product;
  }
  else{
    return `not a valid input`;
  }


}



```
- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // 'Bigger than 5'
check(1); // 'Smaller than 5'
check(5); // 5

///in each case it is having return keyword which will make our program to terminate and return the value.
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya'
getOutput('John'); // 'You are john'
getOutput(); // 'Who are you'

//
///in each case it is having return keyword which will make our program to terminate and return the value.
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // 'You are arya' and 'Who are you' will be returned
getOutput('John'); // 'You are John' and 'Who are you' will be returned
getOutput(); // Who are you here we are having console.log which will print the message in screen and also having one return so it give output 'who are you'.
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

Yes a function can have multiple return statement.
```js
function findTime(operation){

  if(operation==='wake up'){
    return '5A.M';
  }else if(operation==='dress up'){
    return '8A.M.';
  }else if(operation==='lunch'){
    return '12P.M.';
  }else if(operation==='snacks'){
    return '5P.M.';
  }else if(operation==='dinner'){
    return '9P.M.';
  }else if(operation==='sleep'){
    return '11P.M.';
  }
  else{
    return 'enter a valid operation';
  }
  
}
//here i have used multiple conditions and multiple return statement because user have to enter onw operation 
// so that has to return signle output for a particular input so we need to use multiple return.





```
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
Both are for looping purpose it is used where we want to repeat something there we can use loops
main difference between for and while is while has only one input condtion but for 'for' we have three input conditions .both has one breaking condtions.
exp:
```js
for(i=0;i<=10;i++)
{
  ///some code
}
// here i=0 is first input conditon which is start of the loop so it is initilization of that,after that we have breaking condtions where we have to stop if this is true then loop will keep executing,third we have increment by this we are incresing the value of i so our loop is looping for next itiration.
while(i<10)
{
  //some code
}
// here we have one input condition by which we will enter inside the loop so untill or unless this is true this loop will keep executing for that we must have one breaking condtion at end of the loop.