

# Exercises: JavaScript loops

Paste your answers into this file.

<br>

## Print every number from 0 to 10

```js
for(let i = 0; i < 11; i++){
  console.log(i);
}
```

<br>

## Print every number from 10 to 0

```js
for(let i = 10; i > -1; i--){
  console.log(i);
}
```

<br>

## Print every number from 4 to -16

```js
for(let i = 4; i > -17; i--){
  console.log(i);
}
```

<br>

## Print every fifth number from 8 to 41

```js
for(let i = 8; i < 42; i+=5){
  console.log(i);
}
```

<br>

# Exercises: JavaScript loops with array:

Paste your answers into this file.



1. Change all **odd** numbers to be those numbers multiplied by two:
```js
const numbers = [4, 9, 7, 2, 1, 8];

  // your code here
for(let i = 0; i < numbers.length; i++){
  if(numbers[i] % 2 !== 0){
    numbers[i] *= 2;
  }
}
numbers; // => [4, 18, 14, 2, 2, 8]
```

2.  Create an array to hold your favorite colors.  For each choice, log to the screen a string like: `My #1 choice is blue.`

```js
const favColors = ['blue', 'red', 'green', 'yellow'];
for(let i = 0; i < favColors.length; i++){
  console.log('My #' + (i+1) + ' choice is ' + favColors[i] + '.');
}
```

3.  Create an array of ages.  Loop through and log only the ages that are over 21.

```js
const ages = []

for(let i = 0; i < 90; i++)
  ages[i] = i+1;

for(let i = 0; i < 90; i++){
  if(ages[i] > 21)
  console.log(ages[i]);
}
```

1. Create an array to hold your top five choices of something (music, books, movies, whatever).

    - For each choice, log to the screen a string like: "My #1 choice is blue."
    - **Bonus:** Change it to log "My 1st choice, "My 2nd choice", "My 3rd choice", picking the right suffix for the number based on what it is.

```js
const favorites = ['music', 'books', 'movies', 'video games', 'coffee'];

for(let i = 0; i < favorites.length; i++){
  (i === 0)? console.log('My 1st choice is ' + favorites[i]):
  (i === 1)? console.log('My 2nd choice is ' + favorites[i]):
  (i === 2)? console.log('My 3rd choice is ' + favorites[i]):
  (i === 3)? console.log('My 4th choice is ' + favorites[i]): console.log('My 5th choice is ' + favorites[i])
}
```


## The classic Fizzbuzz Program

For every `number` between 1 and 100...

If the `number` is evenly divisible by 3, print "Fizz"

If the `number` is evenly divisible by 5, print "Buzz"

If the `number` is evenly divisible by 3 AND evenly divisible by 5, print "Fizzbuzz"


```js
for(let i = 1; i <= 100; i++){
  if(i % 3 === 0 && i % 5 === 0){
    console.log('FizzBuzz');
  }
  else if(i % 3 === 0){
    console.log('Fizz');
  }
  else if(i % 5 === 0){
    console.log('Buzz');
  }
  else {
    console.log(i);
  }
}
```

<br>


## The even/odd reporter

Write a for loop that will iterate from 0 to 20. For each iteration, it will check if the current number is even or odd, and report that to the screen (e.g. "2 is even").

```js
for(let i = 0; i <= 20; i++){
  i % 2 === 0? console.log(i + ' is even.') : console.log(i + ' is odd.');
}
```

<br>

## Multiplication Tables

Write a for loop that will iterate from 0 to 10. For each iteration of the for loop, it will multiply the number by 9 and log the result (e.g. "2 * 9 = 18").

Bonus: Use a nested for loop to show the tables for every multiplier from 1 to 10 (100 results total).


```js
// Main question
for(let i = 0; i <= 10; i++){
  console.log(i + ' * ' + ' 9 ' + ' = ' + i * 9);
}

// bonus
for(let i = 1; i <= 10; i++){
  for(let j = 1; j<= 10; j++){
    console.log(i + ' * ' + j + ' = ' + i * j);
  }
}
```

<br>

## The Grade Assigner

Check the results for every value from 60 to 100 - so your log should show "For 89, you got a B. For 90, you got an A.", etc.

```js
for(let i = 60; i <= 100; i++){
  (i >= 90)? console.log('For ' + i + ', you got an A.'):
  (i >= 80)? console.log('For ' + i + ', you got a B.'):
  (i >= 70)? console.log('For ' + i + ', you got a C.'):
  console.log('For ' + i + ', you got a D.');
}
```
