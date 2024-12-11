# Unhandled Error in Asynchronous Node.js Express App

This repository demonstrates a common error in Node.js applications: unhandled exceptions within asynchronous callbacks.  The `bug.js` file contains an Express.js server that simulates an asynchronous operation that might fail. If the simulated operation fails, an error is thrown, but it's not caught, leading to a crash.

The `bugSolution.js` file shows how to properly handle this type of error using a `try...catch` block or by using promises and `.catch()` method.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node bug.js`.
4. Observe the server crashing intermittently (approximately 50% of the time).

## Solution

Refer to the `bugSolution.js` file for a corrected implementation that uses error handling to prevent crashes. The solution demonstrates how to avoid unexpected application crashes by appropriately handling errors in asynchronous operations. This is crucial for building robust and reliable Node.js applications.