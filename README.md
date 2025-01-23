# Unhandled Exception in Node.js HTTP Server

This example demonstrates an unhandled exception in a Node.js HTTP server and how to properly handle it.

## Bug
The `server.js` file contains an HTTP server that throws an unhandled exception when the `/error` route is accessed. This leads to the server crashing.

## Solution
The `serverSolution.js` file demonstrates the proper way to handle exceptions within an asynchronous Node.js application.  A `try...catch` block ensures that errors are caught and logged gracefully without causing the server to crash. 

## How to Run
1. Clone this repository.
2. Navigate to the repository's directory in your terminal.
3. Run `node server.js`. 
4. Access `http://localhost:3000` in your browser. 
5. Access `http://localhost:3000/error` to trigger the unhandled exception (in `server.js`).
6. Compare the behavior of `server.js` with `serverSolution.js` by running `node serverSolution.js` and following steps 4 and 5.
