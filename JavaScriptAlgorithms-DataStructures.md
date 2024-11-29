# JavaScript makes a page interactive

**Syntax:**
    let variable;       #Uninitialized variable - default value is undefined
    let var = 2;        #Initialized variable
    console.log();      #print to screen

**Naming convention**: camelCase

**Datatypes/Datastructures:**
    
    string = "immutable, reassignable" or ''
    number = 1; 2; 3; 
    array = [];         #order is important
    const var           # declare constant variables which cannot be reassigned
    
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

**Loops:** repeating tasks

    * for loop
    for (iterator; condition; iteration) {
        logic;
    }