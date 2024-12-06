# Express.js - Empty req.body Bug

This repository demonstrates a common issue in Express.js applications where the request body (req.body) is empty when processing JSON POST requests that lack a `Content-Type: application/json` header.  The bug and its solution are provided in separate JavaScript files.

**Bug:** The `bug.js` file showcases the problematic Express.js code.  A POST request to `/data` without the correct header will result in an empty `req.body`.

**Solution:** The `bugSolution.js` file demonstrates the fix.  It uses the `express.json()` middleware with an extended configuration to handle requests that are missing a Content-Type header. 

This example highlights the importance of proper middleware configuration and error handling in Express.js to prevent unexpected behavior.