# Node.js EADDRINUSE Error

This repository demonstrates a common error encountered when running Node.js servers: the `EADDRINUSE` error. This error occurs when the server tries to bind to a port that is already in use by another process (e.g., another server, a running application). 

## Bug
The `bug.js` file contains a simple HTTP server that attempts to listen on port 8080. If port 8080 is already in use, the server will throw an `EADDRINUSE` error. 

## Solution
The `bugSolution.js` file provides a solution by implementing error handling to gracefully manage the `EADDRINUSE` error. It includes logic to check if the port is in use and handles the error without crashing the application.