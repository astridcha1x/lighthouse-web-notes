# Passing Command Line Arguements in Node.js
_source material via [Lighthouse Labs](https://www.lighthouselabs.ca/)  and an [article by Scott Robinson.](https://stackabuse.com/command-line-arguments-in-node-js/)_

## process.argv
`process.argv` is a global object that can be used without importing any additional libraries. Just pass arguments to a Node.js application, and the argument can be accessed within the application via the `process.argv` array.

> __KEY IDEA__: `process.argv` is an array!
- first element of the array will always be a file system path pointing to the `node` executable
- second element is the name of the JavaScript file being executed
- third element is the argument passed by the user