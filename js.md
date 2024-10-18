## Difference between static type and dynamic type language


## Client side and server side
- A client is a device, application, or software component that request and consumes services or resource from a server.
- A server is a device, Computer, or Software application that provides services, resources, or function to a client.

## Differnce between var, Let and const.

- Scope:
- var: Function-scoped. Variables declared with var are function-scoped, meaning they are accessible throughout the function in which they are defined.
- let and const: Block-scoped. Variables declared with let and const are block-scoped, meaning they are only accessible within the block (enclosed by curly braces) where they are defined, such as a loop or an if statement.
- Hoisting:
- var: Hoisted. Variables declared with var are hoisted to the top of their containing function or global scope. This means you can access them before they are declared in the code, but they will be initialized with undefined.
- let and const: Hoisted but not initialized. Variables declared with let and const are also hoisted, but they are not initialized until their declaration statement is executed. Trying to access them before the declaration will result in a ReferenceError.
- Reassignment:
- var and let: Can be reassigned. Variables declared with var and let can be reassigned new values after their initial declaration.
- const: Cannot be reassigned. Variables declared with const are read-only and cannot be reassigned once they are given a value. However, it's important to note that for objects and arrays declared with const, their properties or elements can still be modified.
- Temporal Dead Zone (TDZ):
- var: Variables are not affected by the Temporal Dead Zone (TDZ) because they are hoisted and initialized with undefined.
- let and const: Variables declared with let and const are affected by the TDZ, which means you cannot access them before their declaration in the code.
- Global Object Property:
-var: Variables declared with var become properties of the global object (window in a browser or global in Node.js) if declared in the global scope.
-- let and const: Variables declared with let and const do not become properties of the global object when declared in the global scope.
## String Built in methods

```javascript
let myString = "Prince"
console.log(myString.length) // output 7
console.log(myString.toUpperCase) // output PRINCE
console.log(myString.chatAt('0')) // output p
console.log(myString.indexOf(P)) // output 0
console.log(myString.substring(0, 4)) // output Prin
console.log(myString.slice(0, 4)) // output Prin // it follows negative indexing also 
let newString = "   Prince   " 
console.log(newString.trim()) // output "Prince" // it removes extra spaces
let url = "https://PrinceKumar%20gmail.com"
console.log(url.replace('%20', '@'))// output: https://PrinceKumar@gmail.com
let url = "https://PrinceKumar%20gmail.com"
console.log(url.includes('sss')) // output: false 
// it search provided data inside given string if found then return true otherwise false
let name = "Prince Kumar"
console.log(name.split(' ')) // output: ["Prince","Kumar"]

// it saperates the strings as per given data here we pass space so it saperates by coma(,)where spaces are present.
```

## DOM(Document object model)
- It represent a web page as a tree like structure that allows javasscript to dynamically access and mainipulate the content and structure of a web page.

## Data-types 
- It detremine type of a variable
-  Primitive 
     1. Nubers
     2. string 
     3. boolean
     4. undefined
     5. null
- non-primitive
     1. Object 
     2. array 
     3. function
     4. date
     5. Regexp
