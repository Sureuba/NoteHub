# JavaScript makes a page interactive

**Syntax:**
    let variable;       #Uninitialized variable - default value is undefined
    let var = 2;        #Initialized variable
    console.log();      #print to screen
    "hello" + "world"   #concatenation
    \n                  #new line

**Naming convention**: camelCase

**Datatypes/Datastructures:**
    
    string = "immutable, reassignable" or ''
    number = 1; 2; 3; 
    array = [];         #order is important
    const var           #declare constant variables which cannot be reassigned
    boolean             #true or false value

Non-primitive: hold more complex data

Primitive: strings and numbers can only hold 1 value at a time

**Arrays:**

    * Acessing arrays: array[index];     
    * First element: 0     
    * Mutation: arrays are mutable, can change the value at an index directly (Ex: array[0] = 2)

Array functions

    * .length: returns length of array
    * array.length-1: last element of array


**Methods:** a function associated with certain values or objects

    .log() function part of console object
    .push() push a value to the end of an array, returns new length of array.
    .pop()  removes last element from an array and returns that element 
    .repeat() available for strings, accepts a number as an argument, specifying the number of times to repeat the target string.

**Loops:** repeating tasks

    For loop:
    for (let i = 0; i < count; iteration) {
        logic;
    }

    for (const value of iterable) {

    }
    NOTE: const value exists for a single iteration not during the entire loop

**Functions:** 

    function name(parameter) {

    }

**Scope:** 
* Global scope: all functions have access in its definition
* variable declared in a function can only be used inside that function