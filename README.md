# fizz-buzz-test

 Fizz Buzz starter code for FEW 2.1

 The contents of this repo contain an implementation of the Fizz Buzz program. You may have heard of Fizz Buzz before. It's a program that counts to any value. Along the way it counts values that are multiples of 3 as `fizz` and values that are multiples of 5 as `buzz`. When a number is a multiple of 3 and 5 it counts this as a `fizzbuzz`. 

 When calling the `fizzbuzz(count)` function you inlcude a count and the function returns an object with the count, the count of fizz, count of buzz, and the count of fizzbuzz. 

 Typical output might look like:  

 `{ count: 16, fizz: 5, buzz: 3, fizzBuzz: 1 }`

The program has been broken down into several functions and a couple constants. 

## Getting started 

- Download or Clone this repo
- Navigate the terminal to the project directory
- `npm init -y`
- `npm install --save-dev jest`
- `mkdir tests`
- `touch tests/test.js`

Write your tests in `tests/test.js`. 

A typcial test with Jest looks like: 

```JavaScript
test('Sanity check', () => {

})
```

Run your tests with: 

`npm run test`

The example test above would be "passing" since it does not throw an error. 

Add an assertion: 

```JavaScript
test('Sanity check', () => {
  expect(2+2).toBe(5)
})
```

Run the test. Here the test fails since 2+2 != 5. 

Fix the math and run the test again. This time the test should pass. 

## Testing fizzbuzz

To test the fizzbuzz you'll need to import it into `tests/test.js`. Using a node.js environment you can use: 

`const fb = require('../fizzbuzz')`

From here you can access any of the methods and properties exported from `fizzbuzz.js`. 

`fb.fizzbuzz(16)`

or 

`fb.isFizzy(4)`

## Checking Coverage

How much of your code is covered by the test you wrote? Pretty good question huh?

Jest will automate this for you. 

`npx jest --coverage`

<!-- > -->

This should provide output similar to: 

```
----------|----------|----------|----------|----------|-------------------|
File      |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
----------|----------|----------|----------|----------|-------------------|
All files |    96.88 |      100 |       80 |    96.55 |                   |
 index.js |    96.88 |      100 |       80 |    96.55 |                70 |
----------|----------|----------|----------|----------|-------------------|
```

This tells you what % of code statements were covered by the tests. What % of code branches were covered, these are if else, switch cases etc. What % of functions were tested. What % of lines of code were tested, and line numbers for lines of code that were not tested. 

Check coverage and identify what has not been tested.




