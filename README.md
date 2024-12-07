# Unhandled Promise Rejection in Express.js Async Route

This example demonstrates a common error in Node.js Express.js applications: unhandled promise rejections in asynchronous routes.  The provided `bug.js` showcases the problem, where an error thrown within a `setTimeout` callback (simulating an async operation) isn't properly caught, leading to server crashes.

The solution, `bugSolution.js`, shows how to correctly handle such errors using `try...catch` blocks or `async/await` with error handling to prevent application crashes and provide graceful responses to clients.