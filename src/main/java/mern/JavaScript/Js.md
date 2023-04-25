## 1. What is JavaScript?
- JavaScript is a high-level programming language that commonly used for interactive webpages and web applications
- js developed by Brendan Eich in 1995
- JavaScript supports client side scripting language and also server-side applications
- Js is a single threaded synchronous 
## 2. What are the data types in JavaScript?
- Js has 6 primitive datatypes :Boolean,Number,String,Null,Undefined,Symbol 
- and non-primitive Object
- js is loosely typed Language
## 3. What are the new features introduced in ES6 (ECMAScript 2015)?
- Es6 has major updates for js in 2015 they are:
- arrow function
- let,const
- classes
- Destructing
- Template literals
- Default parameters
- Rest parameters
- Spread Operator
- Promises
- Modules
## 4. What is the difference between let and var in JavaScript?
- Scope:  
```
var is  function scoped they are accessible within the function in which they are declared,
 let is block scoped they are accessible in blocks
 const is aslo block scoped
```
- Re-Declaration:
```
varibales with var are redeclared with in the same scope otherhand let and const are cannot be re-declared
```
- Hoisting : we can do hoisting for let and const also
## 5. What is the difference between const and let in JavaScript?
## 6. What is hoisting in JavaScript?
- Hoisting is a behaviour in JavaScript where variable declaration or function declaration moved top of their scope executed before its intialized called hoisting
- it means that it does give error
- but if it is let variable it give the referenceError 
## 7. What is closure in JavaScript?
- Closure is a function that binds lexical environment  
- 
## 8. What is a callback function in JavaScript?
## 9. What is the difference between synchronous and asynchronous code in JavaScript?
## 10. What is the difference between == and === in JavaScript?
- == and === both checks for compare
- == checks for values irrespective of their dataTypes
- === checks for their values along with their dataTypes
## 11. What is the use of the this keyword in JavaScript?
## 12. What is an object in JavaScript?
- Object in javascript is a  collection of key value-pair where keys are string and values are any valid javascript dataTypes
- Object are reals time entities
- Objects are declared using object literals or using constructor
```javascript
// using object literals
const data={
    'name':'Radha',
    'age':20
}
```
```javascript
// using constructor
function Employee(name,age){
    this.name=name;
    this.age=age;
}
const Emp=new Employee('Jhaniki,22');
```
## 13. What is JSON in JavaScript?
- JSON stands for JavaScript Object Notation which is a light weighted 
- text-based data interchange format which is easy to read and write 
- it is used to format data between client and server
## 14. What is the difference between a function declaration and a function expression in JavaScript?
## 15. What is the difference between null and undefined in JavaScript?
## 16. What is the difference between call and apply methods in JavaScript?
## 17. What is the use of the bind method in JavaScript?
## 18. What is the use of the map method in JavaScript?
## 19. What is the difference between a for loop and a forEach loop in JavaScript?
## 20. What is the use of the try...catch statement in JavaScript?
## 21. What is TemporalDead Zone?
- TemporalDeadZone is time when a let,const variable is hoisted to until variable is being intialized
- when let ,const variables are in temporal dead zone we cannot access and it give reference error
```javascript
console.log(a);
let a=10;
```
## 22.Lexical Environment?
- Lexical environment are created at the time of context execution
- Lexical is a hirechachy which holds current data and their parent data
## 23.What is Block Scoped in javaScript?
- variables and function are accessed by the block called Block Scoped
- let and const are in block scope
## 24.Shadowing in javascript?
- when a variable is declared in other scope when we use same variable in block scope when we call that variable in inner scope the value is shadowed by the other scope
## 25. What are First Class Functions?
- The ability of functions to be used as values and can passed as arguments to another function and can be returned from functions called first class Functions
```javascript
var c= function (name){
    return function xyz() {
        console.log(name)
    }
}
var d=c('janu');
d();
```
## 26. What is Function Statement? or Function Declaration?
- A function with atleast one statement called function statement 
- Function statement also called as Function Declaration
```javascript
function a(){
    console.log('Helloo');
}
```
## 27. What is Function Expression?
- A function is assigned to a variable is called function expression
```javascript
var b =function c(){
    console.log('Bye')
}
```
## 28. Difference Between Function Statement and Function Expression?
- Whenever we do hoisting  the functions ,function expression give typeError
```javascript
a();
b(); // whenever we call b function it give the b is not a function
function a(){
    console.log('Hellooo')
}
var b=function c(){
    console.log('Byeee') 
}
```