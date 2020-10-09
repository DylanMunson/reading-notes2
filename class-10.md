# Read: 10 - Error Handling and Debugging

## The Stack

In JS, the code is processed one line at a time. When a statement needs data from a function, it will pile the new function on top of the current task. If another statement need other code to be able to do its job, that task will go on the pile as well. Once that task is performed, the interpreter goes back down the line. When a new item is added to the pile, it'll create new *execution content*. the execution content is only available in that function. When a function gets called a second time, it can have a different variable than the first time.

## Execution Context and Housing

When a script enters a new execution conext, it has two phases of activity and the first is the preparation. In this phase, the new scope is created, variables, functions, and arguments are created, and the value of the *this* keyword is determined. This phase is sometimes described as **hoisting**. In the execution phase, values are assigned to variables, functions are refrenced and the code is run, and statements are executed. Understanding these 2 phases are important for understanding that you can call functions before they've been declared (using function declarations), and assigning a value to a variable that has not yet been declared.

[Back](https://dylanmunson.github.io/reading-notes/)
