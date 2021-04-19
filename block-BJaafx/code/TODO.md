1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
function averageOfNumber(){
  var sum =0;
  for(let i = 0; i < 10; i++){
    var num =prompt("enter numbers");
    sum += num;
  }
  return sum/10;
}
averageOfNumber();
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
output - println is a syntax error here but if we replace println with console.log output will be 'hi''hi''hi'.

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js 
function getEvenSum(max=10){
  var sum =0;
   for(let i=1; i<=max; i++){
     if(i%2 === 0){
       sum += i;
     }
   }
   return sum;
}
```
4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js 
function getEvenSum(max=10){
  var sum =0;
   for(let i=1; i<=max; i++){
     if(i%2 !== 0){
       sum += i;
     }
   }
   return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js 

function getProductOfDigits(num){

  if(num<0){
    return `not a valid input`;
  }else{
    var productOfNum = 1, remainder =0 ;
    while(num != 0){
      remainder = num % 10
      productOfNum = productOfNum * remainder;
      num = num-remainder; 
      num = num / 10;
    }
    return productOfNum;
  }
}
```

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

check(10); // Bigger than 5
check(1); // Smaller than 5
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // You are arya
getOutput('John'); // You are john
getOutput(); // who are you
```
third output will be `who are you` because we are passing a empty string. So fisrt two condition inside `if` blocks won't match and third statement don't have any certain condition, it will return the value anyway.


8. Can a function have multiple return statement? Give one example if possible and explain the reason.

 -Yes we can have any number of return statement inside a function.
 example:
 ```js
 function getLastName(name) {
  if (name === 'Gordon') return 'Ramsay';
  if (name === 'Arya') return 'Stark';
  return 'enter valid input';
 }
```
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

We use `while` loop when number of iteration is unknown but `for` loop is used when number of iteration is known. Inside `while` paranthesis we can define only condition, the initialization have to be defined oustide the while statement whereas inside `for` statement we can define initialization, condition and increment in the paranthesis. 

example:
```js
while(num != 0){
  remainder = num % 10
  sumOfNum = sumOfNum * remainder;
  num = num-remainder; 
  num = num / 10;
}
return sumOfNum;
```
This program is for adding digits of a number and no. of iteration is unknown. So `while` loop is being used.

```js
for(int i=0; i<=100;){
  sumOfHundred += i;
}
return sumOfHundred;
```
This program is for adding 0 to 100. Since, here we knew the number of iteration we will use for loop.