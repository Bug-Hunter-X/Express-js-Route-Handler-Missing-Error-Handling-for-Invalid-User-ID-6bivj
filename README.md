# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  lack of error handling for invalid input. Specifically, the code attempts to parse a user ID as an integer without checking for potential errors.  This can lead to unexpected behavior or crashes if the ID is not a valid integer.

The `bug.js` file shows the erroneous code. The `bugSolution.js` file provides a corrected version with proper error handling.

## How to Reproduce

1. Clone the repository.
2. Run `npm install express` to install dependencies.
3. Run `node bug.js`. 
4. Send a request to `/users/abc` (or any non-numeric ID).

The application will likely crash or produce an unexpected response.  Running `node bugSolution.js` and sending the same request will demonstrate the corrected behavior.