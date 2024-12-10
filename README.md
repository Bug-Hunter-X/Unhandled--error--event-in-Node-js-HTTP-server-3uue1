# Unhandled 'error' event in Node.js HTTP server

This repository demonstrates a common error in Node.js applications: the unhandled 'error' event. This event occurs when an unexpected error happens in the server, causing it to crash without proper logging or error handling.

## Problem

The `server.js` file contains a basic HTTP server.  However, it lacks proper error handling.  If an error occurs (e.g., network issue, unexpected request), the server will crash without providing any useful information. 

## Solution

The `server-solution.js` file shows how to properly handle the 'error' event using `server.on('error', ...)` This ensures that even if errors occur, the server gracefully handles them, logs the error, and prevents abrupt termination.

## How to run

1. Clone this repository.
2. Navigate to the repository's directory.
3. Run `node server.js` (or `node server-solution.js` for the solution)
4. Observe the output (or lack thereof for the unhandled error case).