# JavaScript

JavaScript is a high-level, dynamic, untyped, and interpreted programming language.It has been standardized in the ECMAScript language specification. Alongside HTML and CSS, JavaScript is one of the three core technologies of World Wide Web content production; the majority of websites employ it, and all modern Web browsers support it without the need for plug-ins

What is programming:

1. Programming is the way humans tell computers to do logical things for them in a systematic fashion. It lets humans create ways for other people to interact using computers
2. There are a wide variety of programming languages, BUT to decide which to use, we need to decide what we want to use it FOR, and then pick the language best suited for the use

JavaScript is powerful because it is:

1. multi-paradigm (can accommodate a range of thinking/programming styles)
2. prototype-based (things defined can be changed easily)
3. designed to be used for the Web 
4. also is a full-stack language (can be used both on the client / server)

To being, open up the Chrome developer tools (make sure you're on the console tab)

## Lesson One - javascript variables

A variabel is a way to store a value for later on

Similar to algebra, we can set x to equal 1

To do this in javascript we would write the letters 'var'

Each line is then closed with a semi collon 

```
var x = 1;
```

Then we perform actions on this variable such as +(add) -(minus) *(times) /(divide)

```
var x = 1;
x + 2

// 3
```

There are also other variable types such as Strings, so if I want to store the users name of our website I can. Strings work in the same way, however we let the computer know its a string by surrounding the variable with quote marks

```
var name = "James";
```

## Lesson Two - javascript functions

Every programming language lets you create blocks of code that, when called, perform tasks. This is called a function.All programming functions have input and output. The function contains instructions used to create the output from its input

### alert function

There are also functions built directly into javascript, the alert function. A function is decalred by using its:

1. name - alert
2. brackets - letting the computer know it's a function
2. parameters - within the brackets

```
alert();
```

The alert function is one that runs with ot without parameters however, it makes sense to use them

```
var name = "James";

alert(name);
```

### prompt function

Another useful function is the prompt function. It allows us to ask the users for data that we can set to a variable, and then use however we like

```
prompt();
```

We can then expand on that by setting prompt to a variable, and alerting that on our screen

```
var name = prompt();

var alert(name);
```

We can then expand on that, by passing a parameter to prompt() and concatenating two strings together

```
var name = prompt("What is your name?");

var alert("Your name is " + name);
```

## Task One - alert name and age



## Lesson Three - javascript if/else statements

// crtl + enter / shift + enter
