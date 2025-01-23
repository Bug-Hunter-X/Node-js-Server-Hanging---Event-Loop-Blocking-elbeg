# Node.js Server Hanging - Event Loop Blocking

This repository demonstrates a common issue in Node.js applications: blocking the event loop.  The `server.js` file contains a simple HTTP server that hangs for 5 seconds before responding.  This demonstrates how long-running operations can prevent the server from handling other requests.

The `serverSolution.js` file provides a solution using asynchronous operations to prevent event loop blocking.

## How to reproduce

1. Clone the repository.
2. Run `node server.js`.
3. Try to make requests to `http://localhost:3000/` while the server is hanging. You will experience delays.

## Solution

Refer to the `serverSolution.js` file for a corrected version that uses asynchronous techniques to avoid blocking.