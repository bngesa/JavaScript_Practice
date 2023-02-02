# Java Script

1 [Installing Development software](#installing-development-software)
2

## Installing Development software

cmd prompt
git --version
git-scm.com   Downloads
npm  --version

Node.js
<https://nodejs.org/en/download/>

Downloads  
Visual studio code

* Hello world project from github

github.com/pluralsight/web-dev-starter

git clone <https://github.com/pluralsight/web-dev-starter.git>

cd web-dev-starter
code .  for open the VS code

npm install in command prompt

sudo npm install    **

restart PC

  In VS Code ctrl +

npm run start

select project

open in cmd prompt

dir

check package.json in project

npm install

dir

check node modules in project

index.html

css
main.css

npm run start

===================

## Java Script Beginnings

Adding javascript code to html
multiple javascript files
formatiting code
detecting and fixing errors
case sensitivity
commenting code

### Adding javascript code to web page

<script>
    // javascript code here...

</script>

alert('Helle world!');

<http://localhost:3000/>

### working with javascript files

javascript in index.html

<script src = "./filename.js"> </script>

<script src = "./homejs"> </script>    // created new .js file

jquery-3.3.1  

<script src="./utils.js"> </script>
<script src="./home.js"> </script>

function showMessage(message) {
  document.getElementById('message').textContent = message;
  }

### Formatting Code

home.js
      showMessge("changed");
  showMessge(
  "changed"
  );
  
  showMessge     ("changed");
  
### Detecting and Fixing Errors

right click Inspect  -> Console

# $#$#%%   // errors

showMessage("Tittle");
show
Message("Tittle2");   // uncaught ReferenceError

console.log("any message");

### Case Sensitivity

showMessage("Tittle");
ShowMessage("Tittle");  // Uncaught ReferenceError

### Commenting Code

Comments
// Single Line Commenting
/*
Multiple line commenting

Detail complex logicc...
some algorithm...

*/

### Summary

Including JS in HTML

<script> </script>

<script src ="./filename.js"> </script>

Formatting code
Detecting Errors
Case Sensitivity
Js is case sensitive
Commenting Code
single line and multiple line

## Variable and Constants

What is Variable?

Declaring Variable
Naming Variables
Common Errors Using Variables
Changing Variable Value
Constants
The Var Keyword

### Variables

### Declaring Variables

let total = 149.99;

let - keyword
let product  ='Hinking Boots';
let discounted = true;

## Using let to Declare variable

### Declaring Variable

VS code

home.js
 let welcome  = 'Welcome';

 showMessage(welcome);

 let price = 59.99;
 let name = 'test';
 let discounted = true;

 let price= 49.99,
     name = 'test',
  discounted = false;
  
showMessage(name);

### Naming Variables

Valid Variable Names

start with one of  _ $ letter

followed by zero or more  : _ $ letter number  

```
a
account
account_99
accountNumber Camel Case
_accountNumber
$accountNumber   - automatically generated code
_123
_proto__
```
  
### Common Errors using Variables
  
  let 99times = 99;
  showMessage(99times);
  
  //uncaught Syntax Error:
  
  showMessage(_times);
  let let =  99;
  
  let price;
  showMessage(price);
  console.log(price);    // error generated - undefined
  
### Changing Variable Values
  
  let price = 0;
  price = 49.99;
  showMessage(price);

### Constants
  
  const price = 40 ;
  price = 59.99     / uncaught typeerror: assignment to constant value
  showMessage(price);
  
### The Var Keyword
  
  var price = 20;

  var price = 25;
  
  showMessage(price);
  
  console.log(price);
  let price = 25;
  
  var price = 25;
  
### Types and Operators

 Numbers
 strings
 Converting between Types
 Booleans
 Null and undefined
 objects and symbols

### Numbers

  data type
  
  home.js
  
  let price = 30.99;
  showMessage(typeof price);
  
   let price = '30.99';

   price = price +1;
   showMessage(price);

   operator (+-*/%   -= +=*= /= %=)

   let price =12, tax rate =12.333;

   Increment and Decrement operator
   ShowMessage(price++);
   console.log(price);
  
### Operators Prcedence
  
  let price 3 + 2 * 2;
  
  showMessage(price);
  
  mdn operator precedence  
  
### Number Precision
  
  let price = 1.1 + 1.3;
  
  ShowMessage(price);
  
  ##Negative Number
  
  let amount = -20;
  
  let amount = 20 - - 2;  //  (-2)
  
  showMessage(amount);
  let amount = 0;
  
  showMessage(--amount);
  
### Strings
  
   let message = 'Hello';

   showMessage(message);

   for double quotes  \"

   medn

    string  

 escape notation

 \'   \"   \m  \t \b

 let messge `hello`;

 let name = 'Andera';
 let messge `hello ${name}`;

 showMessge(message);
 console.log(message);

### Manipulating Strings

 let messsage = 'hello';

 message = message + 'world';

 message = message.toLowerCase();
 showMessage(message);

 let message = 'Hello';
 message = message.substring(1);
 message =message.length;

 showMessage(typeof message);

 let message = '123';   // "123"
 showmessage(message + 2);

### Converting strings and Numbers

 let amount =123;

 amount =amount.toString();
 showMessage(typeof amount);

 let amount = Number.parseFloat("123.12");
 showMessage(typeof amount);

 showMessage(amount);

 let amount = Number.parseFloat("123.12A");

### Boolean Variable

 let saved = false;

 showMessage(typeof saved);

 saved = !saved;
 showMessage(saved);

### null and undefined

 let saved;
 saved = null;
 showMessage(saved);
 console.log(saved);

 saved =undefined;

### Objects and Symbols

 let person = {
        firstname:  'John',
     lastname: 'Adams'

 };
 showMessage(person.firstname);

### Summary

 Numbers
 String  - 3 styles of quotes:  "" " ``

 Converting between types
 variable.toString()
 Number.parseFloat("123")
 NaN(Not a Number)

 Boolean
 true or false
 !symbol(not)

 null and undefined

* undefined is assigned by JS
 null is assinged by developers

 Objects and symbols
 objects created by { ...}

## Program Flow

### Introduction

 if.. else statements
 truthy and falsy expressions
 Comparing  === to ==
 the ternary operator
 block scope
 loops: for, while, do ... while

### Conditional Using

```
 if statements

 if( 5 === 5)      // true
 {
   console.log ('Yes');
  }
  
  if( 5 > 5)        // false
 {
   console.log ('No');
  }
  
  if( 5 >= 5)      // true  
 {
   console.log ('Yes');
  }
  
 let state = 'FL'
 let taxPercent = 7;

 if(state !== 'FL') {
  taxPercent = 0;
  }
  
  console.log(taxPercent);   // 7
  
  home.js
  
  if(true)
  {
  showMessage('true');
  }

    let price = 20;
    
    if(price <= 15)
    {
      showMessage('discounted');
    }
```

### Truthy and Falsy

  falsy   false   0  "" or " (empty strings)
   null   undefined   NAN

   truthy
     Everything not falsy
  true
  0.5
  "0"
  
  ```
  if("0")
  {
    showMessage('true');
  }

    if(+(1.1 +1.3) .toFixed92) === 2.4) 
    {
       let message = 'hello';
       showMessage(message);
    }

  if() .. else
  
  let state = 'FL';
  
  let taxPercent = 0;
  
  if(state === 'FL')
  {
   taxPercent = 7;

   }
   else  if (state === 'NY')
   {
      taxPercent = 8.875;
  }
  
  console.log(taxPercent);   //7
  
  if(true){
  showMessage('true');
  }
  else
  {
    showMessage('false');
   }

   let price = 4;
   if(price >10)
   showMessage('true');
   else if(price <5)
   {
     showMessage('less than 5');
   }

   let price = 4;
   if(price >10)
   {
   showMessage('true');
   }
   else if(price <5)
   {
     showMessage('less than 5');
   }
  
  else if(price >5)
   {
     showMessage('greater than 5');
   }
```

### Comparing === and  ==

```
   if ( 1 === "1")     // false
   {
     showMessage('true');
   }

   else
   {
    showmessage('false');
   }

     if ( 1 == "1")     // true 
   {
     showMessage('true');
   }

   else
   {
    showmessage('false');
   }
  
   if ( 1 !== "1")     // true
   {
     showMessage('true');
   }

   else
   {
    showmessage('false');
   }
  
    if ( 1 != "1")     // false
   {
     showMessage('true');
   }

   else
   {
    showmessage('false');
   }
  ```

### The Ternary Operators
  
```
  // (Condition) ? true-statement : false-statement;
  
  let message = (price > 10) ? 'expensive' : 'cheap';
  
  showMessage(message);  // expensive
```
  
  ```
   let price =20;

   (price < 10 ) ? showMessage('yes') : showMessage('no'); // yes

    price < 10  ? showMessage('yes') : showMessage('no');  // no
```

  inspect console
  
  let price = 20;
  let message = (price < 10) ? 'yes' : 'no';
  showMessage(message);
  
### Block scope using let
  
  ```
   if(true)
   {
     let value = 'yes';
  showMessage(value);
   }

   console.log(value);

   if(true)
   {
     var value = 'yes';
  showMessage(value);
   }

   console.log(value);

   if(true)
   {
     const  value = 'yes';
  showMessage(value);
   }

   console.log(value);
```

### Looping with for()

```
    for ( let i= 0; i< 3; i++)
 {
   console.log(i);
   }
  // 0 1 2
  
  check console
  
  for i-- infinte
 restart wen server
```

### Looping with while()

```
 while()

 let count =1;

 while (count <5)
 {

 console.log(count);
   count ++;
   }
   //  1 2 3 4

   let i =4;

 while (i >0)
 {

 console.log(i);
   i--;
   }

   console   // 4 3 2 1
```

### Looping with do.. while() loops

```
   let count =1;

   do {
     console.log(count);
      count ++;
   }  while(count <5);

   // 0 1 2 3 4

   let i =4;
   do{
     console.log(i);
  i--;
   } while(i>0);

   // 4 3 2 1

   let i =-4;
   do{
     console.log(i);
  i--;
   } while(i>0);

   // -4  
```

### Summary  

   always use === and !== as a best practice

   block scope
    - variable declared with let or const are cblock scoped

## Functions 
    
### Introduction
   
      Functions basics

   Functions expressions

   passing information to functions
   function return values

   function scope
   using function to modify web pages

### Functions Basics

  function showMessage(){

   console.log('in a function');
}  

showMessage();

showMessage();

### function expersion

function showMessage(){

}

  let fn = function (){
  
  }
  
  fn();  // call the function
  
  let fn = function loggingfunction(){
  
  }
  
  fn();  // call the function
  
### passing information to fun

function showMessage(message){
   console.log(message);
}

showMessage('First Message');
showMessage('Second Message');

  function showMessage(message, anothermessage ){
   console.log(message, anothermessage);
}

showMessage('message', 'anothermessage');

let myfunction = function(message, firstname)
{
   console.log(message);
   console.log(firstname);
}

myfunction('Hello' , 'John');
myfunction('Hello');  // undefined
myfunction();    // undefined  undefined

### Function Return Values

function getSecretCode(value)
{

  let code = value * 42;
  return code;
  }
  
   console.log(getSecretCode(2)); // 84

   function getSecretCode(value)
{

  let code = value * 42;
 // return code;
  }
  
   console.log(getSecretCode(2));

   // undefined

   let secretCode = getSecretCode(2);

   showMessage(secretCode);

### Function Scope

   function getSecretCode(value)
   {

let code = value * 42;
  return code;
  }
  
  let secretCode  = getSecretCode(2);
  console.log(code);
  
  // ReferenceError : code is undefined
  
let key = 42;

  function getSecretCode(value)
  {
  
let keyGenerator = function() {
    
let key = 12;
  console.log('in keyGenerator: ' ,key);
  return key;
  }
  
  let code = value * keyGenerator();
  console.log('in getSecretCode:',key);
     return code;
 }

  let secretCode = getSecretCode(2);
  showMessage(secretCode);
  
  // in keyGenerator: 12
  
  // in getSecretCode: 42  
  
### using function to modify web pages

utils.js

function showMessage(message) {

   document.getElementById('message').textContent = message;
}
  
  <h1  id="message" class="col-sm-12"> GET  </h1>
  
  function changePercentOff(percentage)
  {
    document.getElementById('percentage-off').textContent = percentage + "% OFF";

  }
  
  index.html

   < h2 id = "percentage-off"> 20% OFF </h2>

   home.js

   changePercentOff( 32);

### Summary
  
## Objects and the DOM

### Introduction

   Object properties and methods
   Passing objects to function
   standard built in objects
   The document object Model
   styling DOM Elements
   Detecting Button Clicks
   showing and Hiding DOM Elements

### Object properties and methods

   let person = { };

      let person = {
     name :  "John",
  age: 32,
  partTime : false
   };

    console.log(person.name);
 console.log(person.age);

   showMessage(person.age);
   showMessage(percentage.country);

   person.age =33;
   person['age'] = 44;

   let mySymbol  = Symbol();
   let person = { };

      let person = {
     name :  "John",
  age: 32,
  partTime : false,
   };
    person['age'] = 44;
 showMessage(person.age);

### Object Methods

     let person = {
     name :  "John",
  age: 32,
  partTime : false,
  showInfo : function() {
    showMessage(name);
    showMessage(this.name);
     showMessage(this.name + 'is' + realAge);
  }
   };
    person.showInfo(34);

 showMessage(type person.showInfo);

### pasing object to functions

 let message = 'Hello';

 function changeMessage(message)
 {
     message = 'Hi!;
  
 }

 changeMessage(message);
 showMessage(message);

 let person = {
    name: 'John',
    age: 32,
    partTime: false
    };

    function incrementAge(person)
    {
       person.age++;
    }
    
    incrementAge(person);
    
    showMessage(person.age);
    
    
     function incrementAge(p)
    {
       p.age++;
    }
    
    ## Standard built-in Objects
    
    Javascript Reference Global objects
    
    Methods
    
    Date 
   
   
     let now = new Date();
  showMessage(now.toDateString());
  
  Math  
  
     showMessage(Math.abs(-42));

  String
  
     let s = 'hello';
     
     showMessage(s.charAt(0));

   Number

### Document Object Model (DOM)

   explore in vscode

   document.getElementById('messge').textContent = message;

   DOM Interface

  index.html
  
   utils.js       - document

### styling DOM

   HTMLElement

     styles
     
     home.js
      const header = document.getElementById('message');

   header.style.font = '#FFF';
   header.style.fontWeight = '800';

### Detecting Button Clicks

    < a class ="btn btn-default"> see  Review </a>
    
    cosnt button = document.getElementById('see-review');
    
    button.addEventListener('click', function()
    {
       console.log('click')'
    }
    
    
    ## showing and Hiding DOM elements

    index.html
    
    
    <div id= "review"  class "container d-none">
    
     </div>
     
     
      cosnt button = document.getElementById('see-review');
    
    button.addEventListener('click', function()
    {
     const review = document.getElementById('review');
     
       if(review.classList.contains('d-none'))
    {
      review.classList.remove('d-none');
      button.textContent = 'CLOSe REVIEW';
    }
    else {
      review.classList.add('d-none');
      button.textContent= 'SEE REVIEW';
    }
    }

### Summary

 Styling DOM Elements
  element.style.cssProp = 'value'
  
  Detecting Button Click
  element.addEventListener(event,fn)
   showing and Hiding DOM Elements
   element.classList.add(className)
   element.classList.remove(className)
   Element.classList.contains(className)

## Arrays

     # Introduction
   creating and Intiailzing Arrays
   accessing array items
    manipulating arrays
    slice() and splice()
    array searching and looping
    arrays in the DOM

    ## creating and Intiailzing Arrays 
    
    
    // create an Array
    
    let values = [];
    // create and Intilize an Arrays
    let values = [1,2,3 ];
   
      // Intialize an array
   let values = Array.of(1,2,3);

   home.js

   const values = [ 'a', 'b', 'c'];

   console.log(values);

  console.log(Array.isArray(values)); // truen
  
  Global Object - Array
  
### Accessing array items

      // Accessing an array

   let values = [ 'a', 'b', 'c' ];
   console.log(values[0]);  //a
   console.log(values[3]); // undefined

   let values = [ 'a', 'b', 'c' ];
   values[0] = 'aaa';
    console.log(values[0]);  //aaa

    ## manipulating array
    
    // push()
    const values = [ 'a' , 'b' , 'c' ];
   values.push('d');
    console.log(values); //  a b c d

    // pop()
    const values = [ 'a' , 'b' , 'c' ];
    const last = values.pop();
    console.log(last); // c  
    
    
    shift()
     const values = [ 'a' , 'b' , 'c' ];
    cosnt first = values.shift();
    console.log(first ); // a  
    
    
       const values = [ 'b' , 'c' ];
    values.unshift('a');
    console.log(first ); //a b c  

   values.push( 'd' , 'e', 'f');

   values.pop();
   console.log(values, first);

### Slice() and Splice()

   // slice()

   const values = [ 'a', 'b', 'c' ];

   const newvalues = values.slice(1,2);
   console.log(newvalues);  //b

   //splice()
   const values = [ 'a', 'b', 'c' ];

   values.splice(1,1);
   console.log(values);  // a c

   const values = [ 'a', 'b', 'c' ];
   values.splice(1,0, 'foo');
   console.log(values);  // a foo b c

### Array Searching and Looping

    // indexOf()
    
    cosnt values = [ 'a', 'b', 'c'];
    console.log(values.indexOf('c'));  // 2
    console.log(values.indexOf('d'));  // -1 
    
    // filter()
    const values  [ 'a', 'b', 'c' ];
    const set = values.filter(function(item) {
    
    return item > 'b';
    
    });
    
    console.log(set);  // c

   //  find()
    const values  [ 'a', 'bbb', 'c' ];
   const found = values.find(function(item) {
      return item.length >1 ;
   });

   console.log(fount) ;  // bbbt

   // foreach() // find()
    values.forEach(function(item) {
    console.log(item);
    });   // a b c

  Global Object Array

     ## Arrays in the DOM 

    index.html
    
     < div class   > 
  
  home.js
  const containers =
  document.getElementByclassName('container');
  
  containers[2].classList.add('d-none');
  console.log(containers);
  
### Summary
  
    # Scope and Hoisting 

 #Introduction
       Global Scope

    Function Scope
    var and Hoisting 
    
    Undeclared Variables
     strict Mode 
  
### Global Scope

   home.js

     function showProductID()
     {
       console.log(productId);
     }
     
     showProductID();
     
     // ReferenceError  productID is not defined at showProductId 
     
     
     
     const app  ={
     
        productID : 1245,
     username : 'joe'
     };
     
     function showProductID(){
       console.log(app.productID);
     }
     showProductID();
     
     
     /// 1245 
     
     
     // Function Scope 
     
     function showProductID(){
     let product = 1235;
       console.log(productID);
     }
     showProductID(1234);    //not working
     
     
     function showProductID() {
     let productId = 12345;

   function fix(){
    let productId = 4567;
    console.log('in fix: ', productId);
    }

    fix();
    console.log('in showProductID: ', productId);
    }
    
    showProductID();

  // in fix : 456

   let productId = 4567;
     function fix(){

    console.log('in fix: ', productId);
    }
    
    fix();
    console.log('in showProductID: ', productId);
    }
    
    showProductID();

### Var and Hoisting

      productId = 456;

   console.log(productId);
   var productId = 123;

   let productId = 123;

   ==============

   showProductID() ;

   function showProductID()
   {
     console.log(123);
   }

### Undeclared variable and strict mode

   productId = 1234;

   console.log(productId);

   console.log(window.productId);

   'use strict'
   productId = 1234;

   console.log(productId);

   console.log(window.productId);

   'use strict'
   cosnt productId = 1234;

   console.log(productId);

   console.log(window.productId);

### Summary

    Global scope 
    
      all functions can access items
   
     Function scope 
  
      resolve name by looking at function, then 
   surrounding functions, then global scope

  var and Hoisting
  
  use let and const
  function declaration are fine
  
  undeclered variable and strict mode
  
   'use strict';
