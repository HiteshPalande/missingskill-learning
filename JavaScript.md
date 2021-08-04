

















# 										JavaScript























---





## JavaScript Overview



### History

JavaScript also known as JS is object oriented language. This language has born in the year of 1995. In early 90s and even before that, Apple and Microsoft were two large organizations but Netscape decided to build its own language which can support browser. This language was called LiveScript or Mocha. 

Later Sunmicro System and Netscape came together to create a new language. The responsibility of creating a language was given to a developer called Brandon Eich, who had developed this language within just three weeks. Since, Sunmicro System was owning Java and newly developed language was scripting language, the name given to that language is "JavaScript".

Later this language was donated to ECMA to create some standard implementations. After that ECMA released many versions of JavaScript in which ES5 and ES6 are most popular and used in today's world.

  





### Tech Debts

Tech Debts are nothing but issues got ignored by developer mistakenly while creating JS.

1. ##### `+`

   This operator was designed for addition but along with addition it also does concatenation.

   If one of the operand is String type it always does concatenation irrespective of the another operand.

2. ##### `==`

   This operator just checks the content of operand not type but to check the type and content of operand they had to introduced === operator. 

3. ##### `null`

   When we check type of null it gives type as Object but null is not really an object.

   Actually while developing JS they had forgot to check the type of null.

   These Tech Debts could not be solved because all browsers were/are running on JS. If developers try to remove it possibly browsers will get crashed and they’ll have to design browser from beginning.



### Browsers Running on JS

-    Chrome 
-   Mozilla Firefox
-  Microsoft Edge
- Opera
- Safari
-  Brave

Google has derived V8 Engine from Chrome which is written in C++. Further node.js derived from V8 Engine which is particularly designed for backend. It’s actually not a language it’s runtime environment for JavaScript.



### Popular Frameworks in JS

- Node.js
- React.js
- Angular.js
- Vue.js
- Backbone.js
- jQuery



### Popular Websites Build Using JS 

- Amazon
- Google
- Youtube
- Facebook
- Yahoo
- Ebay
- Linkedin
- Twitter





---





## Basics of JavaScript



### JavaScript Data Types



The JavaScript is Dynamically Typed Language i.e. the type of the variable is determined at runtime.

Basically there are two main categories of JS Data Type:

1. Primitive Data Types
2. Non-primitive Data Types



#### 1. Primitive Data Types 

Primitives are most basic data types.

Primitive data types are further classified as:

- ##### **string** 

  In JS anything within “” (double quotes) or ‘’ (single quotes) is known as string value. Its respective prototype is String.

  e.g.

  `var name = “Harry Potter”;`

- ##### **number**

  The number data type is any value including Integer as well as Decimal. It also includes NaN (Not a Number) as it’s data type. Its respective prototype is Number.

  e.g.

  `var age = 22;`

  `var pi = 3.14;`

- ##### **boolean**

  This data type has only two values, either true or false which are keywords in JS. Its respective prototype is Boolean.

  e.g.

  `var flag = true`

- ##### **undefined**

  This type is mostly used by engines and not by the programmer. If engine finds any variable without value assignment, it assigns undefined value to that variable.

  e.g.

  `var location;`

  `console.log(location);       //undefined,`

  ###### Note: undefined is value as well as type.

- ##### **null**

  null is a primitive data type but because of Tech Debt if we check its type using typeof then it’s type is shown as Object.

  e.g.

  `var objA = null;`

- ##### **symbol**

  It is added in ES6 and not used now.



#### 2. Non-primitive Data Types 

These data types are complex type of data type which are made by primitive as well as non-primitive data types

Non-primitive Data Types are further classified as:

- ##### **Object**

  This stores the data in the form of key-value pair at run time.

  It can store primitive as well as non-primitive values. 

  e.g.

  ````javascript
  var details = {
  
       name: “Harry Potter”,
       age: 25,
       location: “Hogwarts”,
       friends: [“Ron”, “Hermione”, “Dobby”, “Hagrid”]
  }
  ````

  

   

  We can access object elements:

  ​      To insert or update value into an object

  ​        object_name.keyname = value 

  ​      

  ​      To read value from an object

  ​        object_name.keyname

   

  If there is space in key element (e.g. full name) then we use Bracket Notation to access the value from that key.

    e.g. object_name[“kay name”]

  

- ##### **Array**

  -  Array is indexed based data type.
  - It is also an Object, so index of an array acts as a key to the value where in an array key is only numeric (integer) type.
  - In JS, array does not have fixed length. Array length is always given as (last index + 1).
  - In an array we can insert any other type as key since it is also an object but that value will not be considered in a length.
  - It can store primitive as well as non-primitive values.

   e.g.

​		`var arr = [1, 4, 3, “a”, “b”, [22, 33, 55], {name: “abc”}]`

 

We can access array elements:

````javascript
   array_name[index] = 43;    //to insert or update value into an array

   console.log( array_name[index] )   // to read value from an array`
````





We can also access array elements by using Bracket Notation.

array_name[“index”]

​		e.g. 

​		`arr[“4”]  // “b”`





### Operators in JS

Operators in JavaScript is used to perform various mathematical and logical operations.

##### Table of Operators

| **Sr. No.** | **Symbol**             | **Description**                                              |
| ----------- | ---------------------- | ------------------------------------------------------------ |
| 1           | +                      | It  does addition of two operands and if one of the operand is string then it  concatenates the operand. |
| 2           | -                      | It  subtracts two operands                                   |
| 3           | *                      | It  multiplies two operands                                  |
| 4           | /                      | It  returns quotient after performing operation              |
| 5           | %                      | It’s  modulus operator. It returns remainder after performing operation. |
| 6           | --                     | It’s  unary operator and decrements the value by 1 and assigns it back to variable |
| 7           | ++                     | It’s  unary operator and increments the value by 1 and assigns it back to variable |
| 8           | =                      | It’s  assignment operator and assigns value to the variable  |
| 9           | +=  , -= , *= , %=, /= | It’s  assignment operator and after performing the respective operator it assigns  value back to the variable.  e.g.  var  a = 2;  a  += 3;  //a=a+3 |
| 10          | ==                     | This  operator checks the value of the operator              |
| 11          | ===                    | This  operator check value as well as type of the operator   |
| 12          | &&                     | It  performs AND operation on the operators and gives false if any one of the  value is false |
| 13          | \|\|                   | It  performs OR operation on the operators and gives true if any one of the value  is true |
| 14          | !                      | It  negates the result of the operator                       |
| 15          | !==                    | Returns  true if value the operands are not equal            |
| 16          | !===                   | Returns  true if value and type of the operands are equal.   |
| 17          | ?:                     | It’s  ternary operator.   e.g.  (3>4) ? false : true  It  checks the condition and accordingly gives values |



##### typeof' Operator

typeof is the operator which determines the type of the given operator:

| **typeof**       | **Output** |
| ---------------- | ---------- |
| typeof 10        | number     |
| typeof 10.33     | number     |
| typeof “myName”  | string     |
| typeof true      | boolean    |
| typeof True      | undefined  |
| typeof “False”   | string     |
| typeof NaN       | number     |
| typeof undefined | undefined  |
| typeof null      | object     |
| typeof []        | object     |
| typeof {}        | object     |





### Making Variables in JS

In JS, variables are created using **var**, **let** and **const** keywords. These three are act as container only the difference between them is scope.

The following table shows the difference between these three keywords:

| **Sr. No.** | **var**                                 | **let**                                         | **const**                                       |
| ----------- | --------------------------------------- | ----------------------------------------------- | ----------------------------------------------- |
| 1.          | Can  be re-declared                     | Can’t  be re-declared                           | Can’t  be re-declared                           |
| 2.          | Can  be re-initialized                  | Can  be re-initialized                          | Can  be re-initialized                          |
| 3.          | It  has functional scope                | It  has lexical scope                           | It  has lexical scope                           |
| 4.          | Varibles  with var keyword gets hoisted | Varibles  with get keyword does not get hoisted | Varibles  with get keyword does not get hoisted |
| 5.          | var  is introduced in ES5               | var  is introduced in ES6                       | var  is introduced in ES5                       |
| 6.          | e.g.:  var  a = 34;                     | e.g.:  let  a = 34;                             | e.g.:  const  a = 34;                           |

  *Note: If we’re not sure about variable getting updated the it’s recommended to use and if we’re sure that variable will not get updated, then we should use const.*

*const variables must be assigned at the time of declaration only.*



##### Points to remember

- ###### Operations with string 

  `console.log(10 + “final”)     // “10final”`

  `console.log(“10” * 12)       //120` 

  `console.log(“value is”+ false);       //”value is false”`

   

  This problem can be solved by two ways:

  - Converting string into a number by explicit type casting.

    e.g.

    ````javascript
    var a = 10 + Number(“12”);
    
     console.log(a)       //22
    ````
    
    

  ​        

  ​      Here, Number is Prototype of a number primitive type.

  - Another way is by adding + operator as prefix in String

    ````javascript
    var a = 10 + +”12”;
    console.log(a)          //22 
    
    ü var a = undefined + “12”;
    console.log(a)       // ”undefined12”
    ````

    
    
    

- ###### Operations with boolean

  `console.log(true+3)   // 4`

  `console.log(false-2)  //-2`

  `console.log(false-true)      // -1`

  `console.log(“abc”+ false)    // ”abcfalse”`

  `console.log(false-“abc”)     // NaN`

  These outputs are because true value is considered as 1 and false values is considered as 0.

  

-  ###### Operations with null

  `console.log(null+2)   // 2`

  `console.log(null-2)   // -2`

  `console.log(null*null) // undefined`

  `console.log(“a” - null) // NaN`

  

-    ###### Operations with undefined

  `console.log(undefined + 10)  // NaN`

  `console.log(undefined + “12”) // ”undefined12”`

  `console.log(“a” - undefined) // NaN` 

  

-  ###### Operations with Non-primitives

  Addition of any non-primitive value is always a concatenation. JS converts that non-primitive to string type and then performs concatenation.

  e.g.

  `console.log( [1,2,3] + [4,"a"] ) // 1,2,34,a`

  `console.log(true+[1,2,3])    //true1,2,3`

   `console.log({} + {} )   // [object Object][object Object]`

   `console.log( {age:12} + {name: "abc"} )  // [object Object][object Object]`

  `console.log( {} + [] )  //[object Object]`
  
  `console.log( [] + {} )  //[object Object]`

​      `console.log({}+334)   //[object Object]334`



*Note: In case of objects, JS uses special string notation.*

​            `console.log( ({}).toString() )  // [object Object]`





### Hoisting in JS

In JavaScript variable can be hoisted. Hoisting is moving variable declaration at the top of the respective scope of that variable. In this case even if we assign value at the time of declaration, the assignment left behind and declaration moves at the top.

The variables which are made by using var keywords gets hoisted but let and const variables can’t get hoisted. 

We can understand it by simple example of the aquarium tank. As the image shown below the air bubbles left by fish can be considered as var variable and the stones at the bottom of the tank can be considered as let and cost variables. 

As the bubbles gets at the top from wherever it has left but those bubbles can move till surface of the tank and not above than that. Similarly, var variables gets at the top irrespective of the declaration made but inside the scope. 

Now the stones and leaf insides the tank can’t float at top. Similarly, declaration of const and let can’t get to top of the scope if they are declared anywhere in between the scope, they remain wherever they are.

 



<img src="https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/fishTank2.png" alt="fishTank2" style="zoom:50%;" />





Let’s take an example:



![varHoist](https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/varHoist.jpg)



### Truthy & Falsy Values

In JavaScript Truthy values are evaluated as true and Falsy values are evaluated as false.

Falsy values are:

1.  Number: 0 , NaN
2. String: “ ” (Empty String)
3. Undefined
4.  False

In JS, all above mentioned values are considered as false values or Falsy values.

Any other values than all these falsy values are considered as **Truthy Values**.

In Non-primitive Data type we don’t have falsy value even if object or array is empty because as they are the container they always contain a space therefore they are always truthy values.

e.g.

`var arr = [ ]`

`var obj = { }`

In above example, arr and obj are truthy value even if they are empty.





### Scopes in JS

In JavaScript every variable has some specific scope. There are two types of scopes:

##### 1. Functional Scope

In JS, an application itself a functional scope and can be another functional scopes inside that.

Functional scope is inside any function.

Generally, variables declared with the var has functional scope.   

 

##### 2. Lexical Scope

Anything that starts with the pair of { } is known as Lexical Scope.

Generally, variables declared with let keyword and constant initialized with const keywords have Lexical Scope.

 

##### Illustration of functional and lexical scope:



 <img src="https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/ScopeinJS.jpg" alt="ScopeinJS"  />





### Copy by Value & Copy by Reference



##### 1. Copy by value

The concept of Copy by Value takes place in the case of Primitive Data Types. In this case the actual value is passed or copied from one location to another location.

So if we change a value in one location that does not affect the copy of that value to another location.

![callByVal](https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/callByVal.jpg)

 

##### 2. Copy by reference

The concept of Copy by reference takes place in the case of Non-Primitive data types. i.e. Objects and Arrays. In this case instead of passing actual value of container the reference of memory location is passed. Therefore, if one variable changes the content then all those variable pointing to that reference reflects the same changes. 

 ![callByRef](https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/callByRef.jpg)



### Variable Referencing:

In non-primitive data types value of a key can be assign to the another key of another non-primitive data type. This concept is known as Variable Referencing.

e.g.

````javascript
var person = {
		name: “xyz”,
	   	location: “Mumbai”
}


var cities = {
		first: “Mumbai”,
      	second: “Pune”
}
person.location = cities.second;     // variable referencing
````



 

  

---





## Functions in JS

In JavaScript, as everything is an Object function is also an object but function is known as **First Class Citizen** because it can perform various tasks other than being only a function. To understand this let’s take an example.

Consider function as all-rounder captain in JavaScript like M. S. Dhoni in a Indian Cricket team, who performs his role as per the requirement.

For particular condition he is hard-hitting batsman and for another particular condition he is wicket-keeper captain as well as he can bowl. This is why he is all-rounder captain who can perform his as well as role of  his team members.

 

<img src="https://github.com/HiteshPalande/missingskill-learning/blob/main/Images/dhoni.jpeg" alt="dhoni" style="zoom:50%;" />





Similarly, function can be considered as all-rounder in JS.

- Function can perform its own basic task of processing on data and may or may not returns a value which can be primitive or non-primitive.

- We can define another function inside a function.

- A function can return a function and can take another function as a parameter.

- As we use object to contain some data, function can also contain a data i.e. it acts as an object while working as a function.

  e.g.

  ````javascript
  function myFunc() {
  
     _______
  
     _______
  
   } 
  
  // Now this function can hold a value like an Object,
  
       myFunc.value = 20;
  ````
  
  

Still if we check type of the function using typeof operator then it gives function as a type.

- A function can be assigned to a var variable.
- Since variable can hold a function so it can be overridden like in the case of normal variable assignment.

 

### Ways of defining a Function

There are two ways by which function can be defined:

##### 1. Declaration of a function

The declaration of a function is a normal way of defining a function.

e.g.

````javascript
function myFunc() {

   _______

   _______

 } 
````



The function defined in this way gets hoisted. That means, we can call a function before defining it.



##### 2. Assignment of a function

In this type of function definition function can be assigned to a variable created using var keyword.

e.g.

````javascript
var myFunc = function(){

   _______

   _______

 } 
````



Here, `myFunc` holds the reference of the function.

This function does not get hoisted and known as anonymous as it has no name. Only var is used to assign a function. As the usual property of var is to hoist the declaration. Hence, if we have called function using this method before defining it declaration of function gets hoisted and function definition remains at the bottom. 





### Safeguarding a code

Before calling any function we must ensure that whether the called function exists or not. If we have called a function which not really a function and something else or simply doesn’t even exist, then calling such function gives error at runtime.

To solve this issue, we need to safeguard the code by simple logic.

`!! function_name && (typeof function_name === “function”) && function_name();`

In above logic, it will check function existence by !! function_name. Suppose if function_name = null, then it turns out to be false since null is falsy value. Then if that exists type of the function will be checked and if will call the function only if type is function.

This way crashing of a program at runtime can be prevented.





### Types of Functions in JS

In a JavaScript we can do a lot with functions. Combining all the ways of defining a function we can have various types of functions.

##### 1. Function defined inside a function

Unlike another programming language, in JS function can be defined inside a function.

 e.g.

````javascript
function firstFunc() {

   _______

   _______

	   function secondFunc() {

    	  _______

      	_______
    } 
} 
````



 Here, the secondFunc() is inside firstFunc(). Functions also have local and global scope. So, the scope of the secondFunc() is till firstFunc() only.

 If we call a function inside its own function definition, then recursion will take place.

e.g.

````javascript
function myFunc() {
   myFunc();            // resursion
}
````



 But this can be avoided If we define a function inside a function with same name.

e.g.

````javascript
function myFunc() {
	   myFunc();
	function myFunc() {
     }             
}
````



 Here, recursion will not take place even inner function has same name as outer function as function definition for inner call is already provided. So, hoisting will take place inside.



##### 2. Nested Functions

When a function returns a function and that inner function also returns another function and so on. Then the functions are known as Nested function.

Syntax:

````javascript
function first() {
	return function second() {
    	 return function third() {
		}
	} 
}
````



This function can be called by function short circuit way,

`first()()();`

 

##### 3. Higher Order Function

As function is a first class citizen, function reference can be hold in a variable. Therefore, function can be passed as parameter to another function and similarly a function can a return a function.

The function which takes function as parameter and/or return a function as a value known as Higher Order Function.

Example of higher order function can be:

````javascript
function add(a, b){
	var v1, v2;
	var ha = a(v1);
	var hb = b(v2);
	return (function(ha, hb){
			return(ha + hb);
    	})
	}


var hold = add(
	function(num1){
		 return num1;
	},
	function(num2){
		return num2;
	}
);

console.log(hold(4, 4));
````



 

##### 4. Pure Function

The Pure functions are those functions which returns the value that we passed to the function as parameter. The parameter that we pass inside function shouldn't be untouched that is parameter value should not get changed while executing the function.

In JavaScript one should always use Pure functions.

 

##### 5. Inline Function

A function can take a parameter as a function. So instead of assigning function to variable and then passing it to the function as parameter, function can be directly passed as a parameter.

e.g.

`function someFunc(function() { ____ }) {`

  `______`

  `______`

`}`

 

##### 6. Immediately Invoked Function Expression

Immediately Invoked Function Expression or IIFE also known as Self Executing Function or SEF.

This function should be called immediately after its definition. The function is anonymous and function definition should be wrapped inside a block ().

This function gets destroyed immediately after it’s execution is done.

 

Syntax for IIFE:

`(function(){`

 `_______`

 `_______`

`}`

`)();`

Here, semicolon after function call to safeguard a function otherwise if there are multiple IIFEs one after the another then JS executes them as function inside a function or call all of them together.

 

##### 7.  Arrow Function

In ES5 we have only two types of which are function expression and function assignment. In ES6 there is another way of defining a function which have only function expression and not a function name i.e. these functions are anonymous. Such functions are known as Arrow function.

Syntax:

````javascript
var myFunc = () =>{

 _______

 _______

}
````



 This function also known as Short Hand notation and works similar as other functions. This function cannot get hoisted.

 

*Note: Functions also has global and local scopes.*

*In functions by passing parameters we can localize the global variables.*

 



---





## Constructors & Prototypes in JS



In JavaScript everything is derived from Object as similar as we have Object class in Java. But in JavaScript we cannot track or inspect the parent object because every object always points to another object.

 **There are some Built in Prototype/Constructor in JS**

- Function: Not used
- String: Heavily used by shadow object creation
- Number: Normally used
- Boolean: Deprecated
- Array: Very heavily used by shadow object creation
- Object: Very heavily used by shadow object creation
- RegEx: Not much used but good to know
- Math: Normally used
- Date: Normally used

 

*Note: if we perform,*

````javascript
var a = Boolean(false);
!!a     //false
console.log(a);   //false

//But if we use new keyword,

var b = new Boolean(false);
!!a     //true
console.log(a);    // Boolean(false)  
````





 

### 1. Function Constructor & Prototype

Being the first class citizen, function can also create an Object.

As in every class we have variables and methods attached to it. In JavaScript method can be attached to an object by using prototype.

 For example,

````javascript
function User(name, id){
	 	this.name = name;
 		this.id = id;
	}
var user1 = new User(“abc”, 23);
````



Now, this User is object created by a function. This is known as Constructor in JS.

This prototype basically inherits the properties of parent as we do in any other object oriented programming language.

Now, if we want to attach method to the object we need to use prototype.

 `User.prototype.someFunc = function() { ______}`

 

### 2. Array Constructor & Prototype

Array is indexed based data structure i.e. we can access array elements using index.

In JS, array can hold all types of data i.e. primitives as well as non-primitive.

Array is special kind of object where keys are always integer value.



#### Built-in methods in Array Constructor

| Method     | Description                                                  |
| ---------- | ------------------------------------------------------------ |
| push()     | It  adds item at the end of the array. Multiple values can be passes as a  parameter in push() method to pass multiple elements into the array at the  end. |
| pop()      | It  removes element which are at the end of an array. This function doesn’t take  any parameter, it removes array element one by one when called. |
| unshift()  | It  adds elements at the beginning of an array.              |
| shift()    | It  removes elements from the beginning of an array.         |
| concat()   | It  concatenates old array with new array and gives single combined array. This  can’t be done with const keyword. |
| forEach()  | It  iterates through an array. This function takes another function as an  argument. This method is only used for Array. |
| map()      | It  iterates through an array and transforms each element of an array. It also  takes another function as an argument. |
| filter()   | It  filters unwanted elements from an array. It also takes another function as an  argument. |
| indexOf()  | It  checks the index of an element passed as an argument. If that element is not  present there it returns -1 value, if elements is present then returns the  index number. |
| includes() | It  takes element as an argument. If that element is present in an array then it  returns true otherwise returns false. |
| join()     | It  is used to convert an array into a String. It takes delimiter as an argument  and using this delimiter it separates each elements of an array. |
| sort()     | It  sorts an array. It takes function as parameter where we can customize  sorting. |
| slice()    | It  takes a number as parameter and slices that array according to parameter  passed and returns a new sliced array |
| splice()   | It  changes the existing elements of an array.               |
| reverse()  | It  works similar to sort() but reverses an array            |

*Note: In JS, Array and Object both are of type object. So we use a function that determines whether the passed parameter is array or not.*

`Array.isArray(arr);`





### 3.   Object Constructor & Prototype

In JavaScript Object can be created in following ways:

- `var arr = { }`

- `var arr = Object( )`;

- `var arr = new Object( );`

- `var arr = Object.create( );`

  

####  Built-in methods for Object Prototype 

| Method                   | Description                                                  |
| ------------------------ | ------------------------------------------------------------ |
| Object.keys(obj)         | It  returns an array of all keys present in the object as an argument. |
| Object.values(obj)       | It  returns an array of all values present in the object as an argument. |
| Object.freez(obj)        | It  freezes the object i.e value of object can’t be changed of an object passed  as parameter. It makes that object immutable. |
| Object.assign({  }, obj) | It  copies object that has passed in the function as a parameter to a new empty  object. It copies all key-value pair but it doesn’t copy deep objects. |
| Object.toString()        | It  converts an object to a string.                          |

 



### 4.String Constructor & Prototype

String is datatype which contain series of any character.



#### Built-in methods for String Prototype

| Methods                   | Description                                                  |
| ------------------------- | ------------------------------------------------------------ |
| toUpperCase()             | It  converts string to Uppercase alphabet                    |
| toLowerCase()             | It  converts string to Lowercase alphabet                    |
| split(delimiter)          | We  pass delimiter as an argument. It separates every character and stores inside  an array. |
| replace(value,  newValue) | It  replaces existing value in the string with new value that has passed as  parameter. |
| trim()                    | It  removes extra spaces that has added before and after string. It doesn’t  remove spaces between the two texts. |
| substr()                  | It  gives substring from main string from mentioned index number. |

 

 

### this keyword in JS

Like other object oriented programming languages JavaScript also has **this** keyword.

The keyword this referes to the current object.

In an object if we use a method, then inside that method ‘this’ keyword works properly i.e. it referes to the current object but the same this if we used in nested function or a function returned by a function or basically not in an immediate function/method then it points to global object.

The ‘this’ keyword of inner function pointing to global object instead of its own object was a problem in ES5, to overcome this issue Arrow function was introduced in ES6. What Arrow function does is, it allows value of ‘this’ of the arrow function to maintain the same reference of ‘this’ of its parent function. But in case of normal inner function ‘this’ refers to global object.

The problem created by inner function of ‘this’ keyword leads to scope leaking since being inside a method it refers to global object.

 



---





## Built-in Methods in JS

##### 1. setTimeout(function, millisecond)

This function takes two arguments: function and time in millisecond.

It delays the execution of passed function for mentioned amount of time which have passed as parameters.

It only runs once.

 

##### 2. setInterval(function, millisecond)

This function takes two arguments: function and time in millisecond.

This function keeps on executing the passed function repeatedly after every millisecond that has passed as parameter in function.

One need to be very careful while using this function since it can lead to memory leakage.

 

##### 3. clearInterval(timer_reference)

It stops execution of the function for that we need pass reference of timer.

 

##### 4. parseInt(param)

It converts passed parameter to an **integer** number. It strips out non-number value and converts it to a number. 

 

**JSON Object**

JSON is JavaScript Object Notation.

Object is data inside a program but outside of program it is a JSON format.

JavaScript has built in support for JSON.

 

##### 5. JSON.stringify({ })

This method converts an object JSON format.

 

##### 6. JSON.parse(“{ }”)

This method converts a JSON format to object.

 

##### 7. require( json_file)

This function imports outside file in current file as well as converts JSON file to object.

 `let obj1 = require(“./obj.json”);`

 



---







## ES6 Features

#### 1. Spread Operator (. . .)

In JS, non-primitives are pass by reference.

 If we use,

`let obj_new = Object.assign({ }, obj);`



It was introduced in ES5 and issue with this is that it creates new memory location for an empty object and copies all values i.e. all key-value to new object.

This works fine for primitive values i.e. primitive values changed by one object does not get reflected to another object because primitives are pass by value. But in the case of non-primitive type, changes made by one object reflects to another copied object since they are pass by reference.

It takes multiple parameters and overrides the first one.

But in ES6 Spread operator `(. . .)` was introduced which works same as `Object.assign().`

The ways of using spread operator are:

`let obj1 = {. . .user, arr: obj.arr.map(item => item)}`

Here, `obj` is object that we’re copying to new object `obj1.`

Here `arr` is non-primitive data of `obj.`

So, with the help of spread operator efforts of copying of elements from old object becomes easy.

 

#### 2. Destructuring

Destructuring in JS is unpacking array or object into a variable.

Spread operators make destructuring easy.

 Let’s assume that there’s an object called user and we want to access some values/parameters of user object. Then using just . notation to access the value we just use following syntax.

 `let {key1, key2, key3, …rest} = user;`

These keys are nothing but keys are from user object and we a indirectly accessing values of user object.

To access all other parameters other that key1, key2 and key3 from user object there is rest keyword used with spread operator.

Destructuring in case of object is easy as we have key names to access the value but on case of arrays we do not have key names and instead of this indexes are there. So, in case of array we can provide names explicitly while destructuring.



#### 3. String Literal

In ES6 String literals is used. Here instead of representing in double quotes(“ ”), back ticks are used (` `).

This reserves space given between two strings.

We can represent variables inside it by using `${ varName}`, it gives value assigned to the variable.

 

 

---

