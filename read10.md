## ERROR HANDLING & DEBUGGING

#### it's about how to find the errors in your code

### Order of execution

To find the source of an error, it helps to know how scripts are processed.The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run.

### Execution contexts

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.

### the stack
The JavaScript interpreter processes one line of code at time when a statement need data from anther function,it stacks (or piles) the new function on top of the current task.
pic

### Each time a script enters a new execution context, there are two phases of activity

##### PREPARE
* The new scope is created.
* Variables, functions, and arguments are created.
* The value of the this keyword is determined.

##### EXECUTE
* Now it can assign values to variables.
* Reference functions and run their code.
* Execute statement.

### Understanding scope
In the interpreter,  each execution context has its own variables object. It holds the variables, functions,  and parameters available within it. Each execution context can also access its parent’s variables object.
p

### Understanding errors

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code.
Error objects
can help us find where our mistakes are and browsers have tools to help us read them.
p

### How to deal with errors

* debug the script to fix errors.
* handle errors gracefully.

### A DEBUGGING WORKFLOW

Debugging is about deduction: eliminating potential causes of an error.
The JavaScript console will tell us when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

1. Look at the error message.
2. Check how far the script is running.
3. Use breakpoints
4. When you have set breakpoints, you can see if the variables around them have the values you would expect them to.
5. Break down I break out parts of the code to testnsmaller pieces of the functionality.
6. Check the number of parameters for a function, or the number of items in an array.

### Browser dev tools & JavaScript console

The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be
The JavaScript console is just one of several developer tools that are found in all modern browsers.
The console will show you when there is an error in your JavaScript. It also displays the line where it became a problem for the interpreter and You can also just type code into the console and it will show you a result in Chrome.

### Logging data to the console

1. The first line is used to indicate the script is running
2. Next an event handler waits for the user leaving a text input, and logs the value that they entered into that form field.
3. That the user clicked submit
4. The value in the width input
5. The value in the height input
6. The value of the area variable

### Handling exceptions

If you know your code might fail, use try, catch, and finally. Each one is given its own code block.

* try : First, you specify the code that you think might throw an exception within the try block.
* catch: If the try code block throws an exception, catch steps in with an alternative set of code.
* finally : The contents of the finally code block will run either way - whether the try block succeeded or faile.
*if you know that you may get an error, you can handle it gracefully using the try, catch, finally statements. Use them to give your users helpful feedback.*

* If you understand execution contexts (which have two  stages) and stacks, you are more likely to find the error  in your code.
* Debugging is the process of finding errors. It involves a  process of deduction.
* The console helps narrow down the area in which the error is located, so you can try to find the exact error.
* If you know that you may get an error, you can handle it gracefully using the try, catch, finally statements.