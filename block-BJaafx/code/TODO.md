1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let average = 0; 
for(let i = 1; i <= 10; i++) {
average = +prompt(`Enter number for average ${average}`);
}
console.log(average / 10);
```
2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
} //Uncaught ReferenceError: println is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10) {
  let sumEven = 0;
  for(let i = 1; i <= max; i++) {
    if(sumEven % 2 === 0) {
      sumEven += i;
    }
  }
  return sumEven;
}
getEvenSum(10);
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max = 10) {
  let sumOdd = 0;
  for(let i = 1; i <= max; i++){
    if(sumOdd % 2 !== 0) {
      sumOdd += i;
    }
  }
  return sumOdd;
}
getOddSum(10);
```
5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.
```js
function getProductOfDigits(num) {
  let product = 1;
  for(let i = 0; i < num.length; i++){
    product *= num[i];
  }
  return `${product}`;
}
getProductOfDigits(123);
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

getOutput('Arya'); // 'You are Arya'
getOutput('John'); // 'You are John'
getOutput(); // 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // You are arya 'Who are you'
getOutput('John'); // You are john 'Who are you'
getOutput(); // 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.

// No a function cannot have mupltiple return statement it will only apply when we call a function.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
for loop can have a value in it we have to define it with some inside of bracket but in while loop we have to define the value first .
```js
for(let i = 0; i <= 10; i++) {
  console.log(i);
}

let value = 1;
while(value < 10){
  console.log(value);
  i = value++;
}
```