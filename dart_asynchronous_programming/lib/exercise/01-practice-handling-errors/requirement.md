The following exercise provides practice handling errors with asynchronous code, using the approach described in the previous section. To simulate asynchronous operations, your code will call the following function, which is provided for you:

Function	Type signature	Description
fetchNewUsername()	Future<String> fetchNewUsername()	Returns the new username that you can use to replace an old one.
Use async and await to implement an asynchronous changeUsername() function that does the following:

Calls the provided asynchronous function fetchNewUsername() and returns its result.
Example return value from changeUsername(): "jane_smith_92"
Catches any error that occurs and returns the string value of the error.
You can use the toString() method to stringify both Exceptions and Errors.