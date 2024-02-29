# ALX Backend JavaScript - Unit Testing Project

## Curriculum

### Short Specializations
- **UnitTests in JS**
  - Back-end Development
  - JavaScript (ES6)
  - NodeJS
  - ExpressJS
  - Mocha

## Resources
Read or watch:
- [Mocha Documentation](https://mochajs.org/)
- [Chai Documentation](https://www.chaijs.com/)
- [Sinon Documentation](https://sinonjs.org/)
- [Express Documentation](https://expressjs.com/)
- [Request Documentation](https://www.npmjs.com/package/request)
- [How to Test NodeJS Apps using Mocha, Chai, and SinonJS](https://scotch.io/tutorials/test-a-node-restful-api-with-mocha-chai-and-sinon)

## Learning Objectives
Upon completion of this project, you are expected to be able to explain to anyone, without the help of Google:

- How to use Mocha to write a test suite
- How to use different assertion libraries (Node or Chai)
- How to present long test suites
- When and how to use spies
- When and how to use stubs
- What are hooks and when to use them
- Unit testing with Async functions
- How to write integration tests with a small node server

## Requirements
- All code executed on Ubuntu 18.04 using Node 12.x.x
- Allowed editors: vi, vim, emacs, Visual Studio Code
- All files should end with a new line
- A README.md file, at the root of the project folder, is mandatory
- Code should use the js extension
- When running every test with `npm run test *.test.js`, everything should pass correctly without any warning or error

## Tasks

### 0. Basic Test with Mocha and Node Assertion Library
- Install Mocha using npm
- Set up a script in your package.json to quickly run Mocha using `npm test`
- Create a function named `calculateNumber` in 0-calcul.js and its test cases in 0-calcul.test.js
- Use assert for testing

### 1. Combining Descriptions
- Create a new file named 1-calcul.js
- Upgrade the function from task 0
- Add a new argument named `type` at the first argument of the function (SUM, SUBTRACT, or DIVIDE)
- Write test cases in 1-calcul.test.js using describe to organize them

### 2. Basic Test Using Chai Assertion Library
- Install Chai with npm
- Copy the files from task 1 to new files 2-calcul_chai.js and 2-calcul_chai.test.js
- Rewrite the test suite using expect from Chai

### 3. Spies
- Install Sinon with npm
- Create utils.js with a property `calculateNumber` and export the Utils module
- Create a new file 3-payment.js with a function `sendPaymentRequestToApi`
- Create 3-payment.test.js using sinon.spy to validate the usage of the Utils function

### 4. Stubs
- Create 4-payment.js, similar to 3-payment.js
- Create 4-payment.test.js, similar to 3-payment.test.js
- Stub the function `Utils.calculateNumber` to always return the same number (10)
- Verify that the stub is being called with specific arguments
- Add a spy to verify that console.log is logging the correct message

### 5. Hooks
- Copy code from 4-payment.js to a new file 5-payment.js
- Create 5-payment.test.js with two tests using a single spy
- Use beforeEach and afterEach hooks

### 6. Async Tests with Done
- Create 6-payment_token.js with a function `getPaymentTokenFromAPI`
- Create 6-payment_token.test.js to test the result of `getPaymentTokenFromAPI(true)` using the `done` callback

### 7. Skip
- Use 7-skip.test.js with a failing test
- Make the test suite pass without fixing or removing the failing test using skipping

### 8. Basic Integration Testing
- Create a new folder 8-api with package.json, api.js, and api.test.js
- Implement an Express server with a welcome message on GET /
- Write an integration test suite for the index page

### 9. Regex Integration Testing
- Use the previous project in 8-api
- Add a new endpoint GET /cart/:id with validation for :id as a number
- Write test cases for the cart page

### 10. Deep Equality & Post Integration Testing
- Use the previous project in 9-api
- Add endpoints GET /available_payments and POST /login
- Write test suites for /login and /available_payments using deep equality for object comparison

## Copyright
Copyright © 2024 ALX, All rights reserved.
