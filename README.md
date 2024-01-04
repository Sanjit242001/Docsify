# Introduction To Programing #

>Programing is a  way to talk to computers a language like hindi and english or bengoli can be used to task to a human but for computers we need straight forwrd insturction.

## Computer is Domb ##

>When was the last time you ordered same cerial and got DVD of Serial.

>Programming is the act of constructing a Program a set of precise instructions telling a computer wgat to do.

## What is Ecmascript ##

>Ecmascript is a standard on which `javascript` is pased it was created to ensure that different documents on javascript are actually talking about the same language.

>Javascript & Esmascript can almost always be used interchangably javascript is very liberal in what it allows.

## How to execute javascript ##

>Javascript can be excuted right inside one's browser you can open the javascript conslole and start writing javascript there.

>Ans ther why to execute javascript is a runtime Like `Node.js` which can be installed and used to run javascript code.

>Vet another why to execute javascript is by inserting it inside `<script>` tag of an HTML document.

# Variable & Data #

>Just like we follow some rules which speaking english (The Gramunar), we have some rule to follow which writing a  javascript program. The set of these rule is called syntex in javascript.

## What is variable ##

>A variable is a container that store a value. this is very similar to the container used to store rice, water and oats(Treat this as an analogy).

>The value od a javascript variable can be changed during the excution of a program.

**Example of variable declaration**

>var a = 7;
>let a = 7;

>In this variable, `a` is an identifier, `=` is an assignment operator, `7` is a literal, and hole processes is a declaring variable.

## Rule for choosing variable name ##

- Letters , digit , underscores & $ sing allowed.
- Javascript reserved words cannot be used as a variable name.
- Sanjit & sanjit are different variable(case sensitive).

## ver vs let in javascript ##

  >1. ver is globally scoped while let & const are block scoped.
  >2. ver can be updated & re-declared within its scope.
  >3. let can be updated but not re-declared.
  >4. const can neither be updated not be re-declared.
  >5. ver variables are initialiged with undejined whereas let and const variables are not initialiged.
  >6. const must be initalijed during declaration let and ver.

## Primitive Data type & objects ##

>Primitive data types are set of basic data types in javascrpt.

>Objects is a non primitive datatype in javascript

**These are the 7 Primitive datatype in javascript**

- Null
- Number
- String
- Symbol
- undefined
- Boolean
- Bigint

## Object ##

An object in javascript can be created as follows

**Example of Object**

Const item = {

    name : "Leb Bulb",
    price : "150"
}

In this object, `name` and `price` are keys, `Led Buld` and `150` are values, and hole processes are an Object creation.


# Expression & Condition #

>A fragment of code that produces a value is called an expression. Every written literal is an expression. For ex: 77 or "Sanjit"

## Operator in javascript ##

### Arithmatic Operators ###

- `+`      Addition
- `-`      Subtraction
- `*`      Multiplication
- `**`     Exponentiation
- `/`      Division
- `%`      Modulus
- `++`     Increment
- `--`     Decrement

### Assignment Operators ###

- `=` Assignment
- `+=` Addition Assignment
- `-=` Subtraction Assignment
- `*=` Multiplication Assignment
- `/=` Division Assignment
- `/=` Modulus Assignment
- `**=` Exponentiation Assignment

### Comparision Operators ###

- `==`    Equal to
- `!=`    Not equal
- `===`   Equal value and type
- `!==`   Not equal value or not equal type
- `>`     Greater then
- `<`     Less then
- `>=`    Greater then or equal to
- `<=`    Less then or equal to
- `?`     Trnary Operator

### Logical Operators ###

- `&&`    Logical and
- `||`    Logical or
- `!`     Logical not

>Apart From these, we also have type and biturse operator. Biturise operator perfrom bit by bit operations on number.

**Example of Orerator and Operands**

> 7 + 8 = 15

- The operator is "+" and the operands are 7 and 8.

## Comments in javascript ##
>Sometime we want our programs to contain a text which is not executid by the `Js` engine

>Such a text is called comment in javascript a comment in javascript can be written as follows:

**Example of Comment**

>let a = 2;   // this is a single line comment.

/*

 i am a

  multiline Comment

*/

>Sometime comment are used to present the execution of some line of code

>let switch = true;
//switch = false

- comment line went eecuit

## Conditional statements ##

>Sometime we might have to execute a block of code based off some condition 

>For Example a prompt might ask for the age of used and if its greater then is display a special message.

**In Javascript we have there from of if else statement.**

- if statement
- if....else statemant
- if....else if....else statemant

**if Statement**

>The if statemant in javascript looks like this:

if(condition){

//code that will be executed if the condition is true

}

>The if statement evalutes the condition inside the `()` if the condition is evaluated to the code inside the body of if is executed else the code is not executed.

**if else statement**

>The if statemant can have an optional else clause the syntex looks something like this.

if(condition1) {<br>
  //code that will be executed if the condition is true<br>
  } <br>else{<br>
    //code that will be executed if the condition is false<br>
    }
>If the condition is true code inside if is execuited else code inside else block is executed.

**if else if statement**

>Sometime we might want to keep recheking a set of condition one by one until one matches
we use if else if for achiering this.

let number = 10;<br>

if (number > 0) {<br>
    console.log('The number is positive');<br>
} else if (number < 0) {<br>
    console.log('The number is negative');<br>
} else {<br>
    console.log('The number is zero');<br>
}

## Javascript ternary Operator ##

>Evaluats a condition and executes a block of code based on the condition.

>condition ?  Exp1 : exp2

>Example syntax of ternary oprator looks like this.

(marks>10) ? 'Yes' : 'No'

- In above example marks greater than 10 returns Yes otherwise it returns No.</s>

# Loop & Fuction #

>We use loops to perform repeated action for example - if you are assigned a task of prenting number from 1 to 100 it will be very hectic to do it manually loops help us automate such tasks.

## Type of Loop in javascript ##

>For Loop -> Loop a block of code no of times
>For in Loop -> Loops through the keys of an object
>For of Loop -> Loops through the valuse of an object
>While Loop -> Keeps looping till the given condition becomes false.
>do-while Loop -> while loop variant which run atleast ones

### The for loop ###
>The syntex of a for loop looks something like this.

for(Statement1;Statement2;Statement){<br>
  //code to be executed<br>
}

- Statement1 is excuted one time;
- Statement2 is the condition base on which the loop runs (Loop body is executed)
- Statement3 is excuted everytime the loop body is executed.

### The for-in Loop ###

>The syntex of for-in loop looks like this.

for(key in object){<br>
  // Code to execute with key here<br>
}

`Note - for-in loops also work with arrags which will be discussed in the later value`

### The for-of Loop ###

>The syntex of for-of loop looks like this.

for(variable of iterable){
  <br/>//Code to execute with variable here<br/>
}

`Iterable data stucture like arrays,string etc`

### The while Loop ###

>The syntax of while loop looks like this.

While(condition){<br>
  // Code to execute if condition is true<br>
}

`Note: if the condithon never become false, the will never end and this might crash the runtime`

### The do...while Loop ###

>The do while loops syntex looks like this.

do{<br>
  // code to be execute<br>
}<br>
while(condithion){<br>
}

`Note: This loop always executes at least once.`</s>

## Function in javascript ##

>A javascript function is a block of code designed to perform a particular task

>Syntex of a function looks something like this.

function myfune(){<br>
  //code goes here<br>
}


function Sanjitfunc(parameter1,parameter2){<br>
  //code here<br>
}
>Function can have multiple parameters separated by comma.</s>

Sanjitfunc(10,11) This is function invocation.

>Function invacaion is a way to use the code inside the function.

>A function can also return value the value is `returned` back to the caller.

Const sum = (a,b){<br>
  let c=a+b;<br>
  return c;<br>
}

`sum(5,7); Here we are calling the function sum and it's returning the value 12 which is assigned to variable sum`

# Strings #

>Stings are use to store and manipiulate text strings can be exeated using the following systax.

let name = "Sanjit"<br>
name.length

`Note: Sanjit is a string, and length is a property that prints the length of the string.`

`Strings can also be created using single quotes`

let name = 'Sanjit'

## Templeate literals ##

>Template literals use backtics insted of quots to define a string.

let name = 'Sanjit'

>With tcmplate literals it is possible to use both single as well as double quates inside a string

let sentence = 'the name "is" Harry 's'.

>We can insert variable dirctlly in template literal. this is called string interpalation.

let a = 'this is {name}'

`name is a variable, and 'this is {name} is do the print this is a Sanjit`

## Escapt sequence characters ##

> If you try to print the following string javascript will missundestande it

let name = 'adom D'angelo'

>we can use single quote essape sequence to solve the problem

let name = ' adam D\'angel'

>Similarly we can use \" unside a string with double quotes.

>Other escape sequence characters are as follows

>\n - new line \t - tab \v - vertical tab \b - backspace \f - form feed \r - carriage reture

## String properties and methode ##

- let name = "Sanjit"<br>
  name.length

`This is to print the length of the name, which means that the name Sanjit has six digits. The print 6 output`

- let name = "Sanjit"<br>
  name.Touppercase()

`This is work to convert the lower case letter to upper case.`

- let name = "Sanjit"<br>
  name.toLowerCase()

`This is work to convert the upper case letter to lower case`

# Arrays #

>Array are variable which can hold mmore then one value.

Const fruits = ["banana","apple","grapes"]

Const a1 = [7,"Sanjit",false]

## Acuessing values ##

let numder = [1,2,3,4]

number[0] // output: 1<br>
number[1]//output : 2

## Finding the length ##

let number = [1,2,3,4]

number[0] -> 1 <br>
number.length // Output: 4 <br>

## Changing the values ##
Let number = [1,2,3,4]
number[0]=5;

`"number" new become [5,2,3,4] arrays are mutable arrays can be changed`

>In javascript arrays are object. the type of operator on arrays returns object

const n = [1,2,3,4]

>typeof n is return "object"

`Arrays can hold many values under a single name`

## Array methods ##

>The are some important array methods in javascript some of them are as follows: 

- toString() -> Converts an array to a string of comma separated values.
  
<body>

     let n = [1,2,3,4]
     n.toString(); // Output: 1,2,3,4
</body>

- join() -> Join all the arrays elements using a separater<br>

    let n = [1,2,3,4]<br>
    n.join("*"); // Output: 1*2*3*4<br>
- pop() -> Removes last element from the array

let n = [1,2,3,4]<br>
n.pop(); // Output: 4<br>

`updates the origenal array returns the popped value`

- push() -> Adds a new elemant at the end of the array

let n = [1,2,3,4]<br>
n.push(5); // Output: [1,2,3,4,5]<br>

`Modifies the orignal array returns the new array length`

- shift() -> Removes first element and returns it

- unshift() -> Adds element to the beginning returns new array length
- delet -> Array elements can be deleted using the delet operator

  let d = [1,2,3,4] <br>
delete d[1]; -> delet is an operator.

- Concat() -> used to join arrays to the given array

  let c1 = [1,2,3]<br>
  let c2 = [4,5,6]<br>
  let c3 = [7,8,9]

c1.Concat(c2,c3) -> Returns [1,2,3,4,5,6,7,8,9]

`concat return a new array does not change existing arrays`

**</b>`Note: This a some method of arrays `**

# Javascript in the browser #

>Javascript was initially create to make web pages alive. Js can be written right in a web pages HTML to make it interaction

>The browser has an embedded engine called the javascript engine or the javascript runtime

>Javascript alrility in the browser is very limited to project the user safety for example a webpage on http://google.com cannot access https://www.facebook.com/ and steal information from there.

## Developer tools ##

>Every browser has some developer tools which makes a developer's life a lot easies

>Ctrl+Shift+I+F12 press on the chrome opens dev tools

We can also write javascript commands in the console

**Console**
>A place where we can run our code and see the results

## The script tag ##

>The script tag is used to insert javascript into an HTML page.

> The script tag can be used to insert externel or internal scripts

<body>

    <script>
        // Internal JavaScript code
        alert('Hello, World!');
    </script>

</body>

`<script src="external.js"></script>`

>The benifit of a separate javasprit file is that the browser will drurload it and store it in its cache.

## Console object method ##

>The console object has servral method log being one of them some of them as follows.

- assent() -> Used to assert a condition.
- clear()  -> Clear the console.
- log() -> Outputs a message to the console.
- table() -> Display a tabular data.
- warn() -> Used for warning.
- error() -> Used for errors.
- info() -> Used for special.

>You will naturally remender some all of these with time

>Comperhensive list can be looked up on MDM.

## Interaction : alter,prompt and confirm ##

- alert : Used to invokl a mini windiw with a msg<br>
  
  alert("hello")

- prompt : Used to take user input as string
inp = prompt("Hi","No")

- confirm : show a message and wails for the user to press ok or cancle returns rtue for ok ans false for cancle

>The exact locatin & look is determined by the browser which is a limitation

## Window object BOM & DOM ##

> We have folling when javascript runs in a browser.

>Window object represents browser window and peovides methods  to control it .It is a global object.

### Document Object model ###
>Dom represents the page content as HTML

>Document . body  -> `page body as js object`

>Document . body . background ="grean"<br>
`Change page background to green`

### Browser Object model (BON) ###

>The browser object model (BOM) represent additionel object provide by browser (host environment) for working everything except the document.

>The function alert/confirm/prompt are also a part of the BOM.

location href = "https://www.google.com/"

`Redirect to another url`

# Working the DOM #

>DOM ther relers to the HTML page where all the nodes are object there can be 3 main type of nodes in the DOM 

> 1. Text nodes 
> 2. ekment nodes 
> 3. comment nodes

>In an HTML page, `<html>` is at root and `<head>` and `<body>` are its children etc

>A text node is always a left of the trll

## Auto Correction ##
>If an erroneous HTML encountered by the browser, it tend to correct it for example, if we put somthing after the body,it is automatically moved inside the body another example is `<table>` tag which must contain `<tbody>`

## Walking the DOM ##

`<html>`<br>
`<head>`<br>
` <title>Page Title</title>`<br>
` </head>`<br>
`<body>`<br>
;<br>
`</body>`<br>
`</html>`

`Note: Document body can something be null if the javascript is written before the body tag`

## Children of an element ##
>Direct as well as deiply nested elements of an element are called its children.

>Child node -> Element that are driect children for example head & body children of `<html>`

>Descendant nodes -> All nested elements,children,thier children and so on ....

## Firstchild,lastchild & childbodes ##
>element firstchild -> first child element

>element lastchild -> last child element

>element childnodes -> all childrens (including text nodes)

### Following is always true : ###
>element child Nodes [0] === elem.firstchild
>element child Nodes [(elem.childNodes.length -1)] === elem.last
