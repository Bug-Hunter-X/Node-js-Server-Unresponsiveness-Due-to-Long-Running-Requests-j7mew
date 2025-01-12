# Node.js Server Unresponsiveness

This repository demonstrates a common issue in Node.js servers: unresponsiveness due to long-running requests.  The provided code simulates a long-running task within the request handler, causing the server to freeze while processing.  A solution is also included to address this problem.

## Bug

The `bug.js` file contains a simple HTTP server that simulates a 5-second long-running task.  During this time, the server becomes unresponsive to new requests.

## Solution

The `bugSolution.js` file demonstrates how to handle long-running requests asynchronously using promises or async/await, thereby preventing the server from blocking and maintaining responsiveness.