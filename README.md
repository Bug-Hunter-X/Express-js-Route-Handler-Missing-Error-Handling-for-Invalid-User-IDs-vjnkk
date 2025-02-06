# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: the lack of error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID.  If the ID is not a valid number, the code will throw an error.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides a corrected version with proper error handling.

## How to reproduce the bug

1. Clone this repository.
2. Run `npm install express` to install the required dependency.
3. Run `node bug.js`.
4. Send a GET request to `/users/abc` (or any non-numeric ID).

You will likely observe a server error or unexpected behavior.

## How to fix the bug

The solution involves adding input validation to ensure that the user ID is a valid number before attempting to use it.  The `bugSolution.js` demonstrates this corrected implementation.