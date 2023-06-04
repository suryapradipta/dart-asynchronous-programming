It’s time to practice what you’ve learned in one final exercise. To simulate asynchronous operations, this exercise provides the asynchronous functions fetchUsername() and logoutUser():

Function	Type signature	Description
fetchUsername()	Future<String> fetchUsername()	Returns the name associated with the current user.
logoutUser()	Future<String> logoutUser()	Performs logout of current user and returns the username that was logged out.
Write the following:

Part 1: addHello()
Write a function addHello() that takes a single String argument.
addHello() returns its String argument preceded by 'Hello '.
Example: addHello('Jon') returns 'Hello Jon'.
Part 2: greetUser()
Write a function greetUser() that takes no arguments.
To get the username, greetUser() calls the provided asynchronous function fetchUsername().
greetUser() creates a greeting for the user by calling addHello(), passing it the username, and returning the result.
Example: If fetchUsername() returns 'Jenny', then greetUser() returns 'Hello Jenny'.
Part 3: sayGoodbye()
Write a function sayGoodbye() that does the following:
Takes no arguments.
Catches any errors.
Calls the provided asynchronous function logoutUser().
If logoutUser() fails, sayGoodbye() returns any string you like.
If logoutUser() succeeds, sayGoodbye() returns the string '<result> Thanks, see you next time', where <result> is the string value returned by calling logoutUser().