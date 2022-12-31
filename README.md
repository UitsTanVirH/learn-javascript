# Execution Context
```
When we run a javascript program an execution context is created.
it has two components... Memory component and Code component
Memory component is also called Variable Environment and
Code component is also called Thread of Execution

Execution context is created in two phases.
Memory creation phase, Code execution phase.
```
# Why javascript is a losely typed language
```
Because it supports all type of data type in a variable
Ex: var a = "tanvir";
var a = 20;
```
# Primitive vs non primitive
```
Non primittive share reference, Primitive share value
```
# Hoisting
```
Even after executing a single line of code, memory is allocated for all the variables and functions. this is called hoisting
```
# Functions
```
Function declaration / Function statement
function print(){
  //kichu ekta
}
------------------------------------------
First class function / first class citizen
A function which takes a function as a perameter or returns a function is called first class function
function call(a){
  a();
}
print(){
  console.log("Something");
}
call(print);
-----------------------------------------
Function expression
var a = function (){
  //kichu ekta
}
----------------------------------------
Named function expression
var a = function print(){
  //kichu ekta
}
----------------------------------------
Anonymous Function
(function(){
  //kichu ekta
})();
----------------------------------------
Arrow function
var print = () => {
  console.log("something");
}
```
# Type error and Reference error
```
A reference error occurs when you try to use a variable that doesn't exist.
A TypeError occurs when the variable exists, but the operation you're trying to perform is not appropriate for the type of value it contains.
```
# Scope
```
Scope can be defined in two ways. 
If the variable can be accessed here or where this variable is accessible
```
# Lexical Environment
```
Lexial environement is memory component of an execution context + it's parent class's lexical environment
```
# Scope chain 
```
Scope chain is a chain of memory components.
If a variable is not found in it's memory component then it will try in it's memory component, if not found then again will try in it's memory component. This creates a chain of memory and this chain is called scope chain
```
# Shadowing
```
If variables are declared with a same name then shadowing happens
```
# Closure
```
Function along with it's parent's lexical environment bundled together forms closure
```
# Memory leak // why let and const is used?
```
var leaks memory between block scopes
```
# Temporal dead zone
```
The time period between declaring let and assigning a value to it is called temporal dead zone
```
# undefined
```
Undefined is a placeholder in javascript. takes up it's own memory before assigining a value
```
# let and const
```
Let and const are used to solve var memory leak problems. they take memory in block scope or script scope
```

