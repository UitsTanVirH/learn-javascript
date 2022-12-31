# learn-javascript

# Execution Context
```
When we run a javascript program an execution context is created.
it has two components... Memory component and Code component
Memory component is also called Variable Environment and
Code component is also called Thread of Execution

Execution context is created in two phases.
Memory creation phase, Code execution phase.
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
