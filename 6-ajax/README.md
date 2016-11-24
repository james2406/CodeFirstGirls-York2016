<<<<<<< HEAD
# Welcome to Code First: Girls (York 2016)

We are going to teach you the basics of how web pages work and also introduce you to programming for the web in 2016.
Skills you'll practice include:
* [HTML](https://github.com/james2406/CodeFirstGirls-York2016/tree/master/1-html%20)
* [CSS](https://github.com/james2406/CodeFirstGirls-York2016/tree/master/2-css)
* Github
* Bootstrap
* JavaScript
* jQuery

This will be a great place where you'll be able to see a summary of what we've taught you and tasks set in the lessons. If there are any problems feel free to either message me or Mike!

## Before You Begin

1. [Create a GitHub Account](https://github.com/join) and sign up for a [GitHub Student Developer Pack](https://education.github.com/pack)
2. [Install Google Chrome](www.google.com/chrome/)
3. Install [Sublime Text](https://www.sublimetext.com/download) or [Atom](https://atom.io/)
4. Install [GitHub Desktop Client](https://desktop.github.com/)
5. Create a folder called coding_course. This will be used to store all of your files for this entire course, so keep it in an easy to reach / memorable place

Now we're ready to start making a website!

## Instructions

1. At the top of the page I have created a single folder for each session
2. Click into the relevant folder



=======
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

A variable is a way to store a value for later on

Similar to algebra, we can set x to equal 1

To do this in javascript we would write the letters 'var'

Each line is then closed with a semi colon 

```
var x = 1;
```

Then we perform actions on this variable such as +(add) -(minus) *(times) /(divide)

```
var x = 1;
x + 2

// 3
```

There are also other variable types such as Strings, so if I want to store the user's name of our website I can. Strings work in the same way, however, we let the computer know it's a string by surrounding the variable with quote marks

```
var name = "James";
```

## Lesson Two - javascript functions

Every programming language lets you create blocks of code that, when called, perform tasks. This is called a function.All programming functions have input and output. The function contains instructions used to create the output from its input

### alert function

There are also functions built directly into javascript, the alert function. A function is declared by using its:

1. name - alert
2. brackets - letting the computer know it's a function
2. parameters - within the brackets

```
alert();
```

The alert function is one that runs without parameters however, it makes sense to use them

```
var name = "James";

alert(name);
```

### prompt function

Another useful function is the prompt function. It allows us to ask the users for data that we can set to a variable, and then use however we like

```
prompt();
```

We can then expand on that by setting prompt to a variable and alerting that on our screen

```
var name = prompt();

alert(name);
```

We can then expand on that, by passing a parameter to prompt() and concatenating two strings together

```
var name = prompt("What is your name?");

alert("Your name is " + name);
```

## Task One - alert name and age

1. Open the Developer Tools
2. Create two prompts, one for age and one for name
3. Display that using an alert

## Lesson Three - javascript if/else statements

// crtl + enter / shift + enter

In javascript, we can create code that only runs when conditions are true. This is done by writing an 'if statement'

1. if - statement type
2. brackets - where our condition goes
2. code - within the curly brackets

```
if () {
  // code goes here
}
```

So, we can create a program what checks a users age on whether they are allowed to drink

```
var age = prompt("How old are you?");

if (age > 17) {
  alert("Welcome to the party!");
}

if (age < 17) {
  alert("Sorry, you're not old enough");
}
```

However, what if the user is 18? We could fix it like this

```
if (age >= 18) {
```

Or we could use an else statement. So, if this doesn't work, do this

```
var age = prompt("How old are you?");

if (age > 17) {
  alert("Welcome to the party!");
} else {
  alert("Sorry, you're not old enough");
}
```

## Task Two - alert name and age

1. Open the Developer Tools
2. Create a program which checks if the user is old enough to drive
3. Display an appropriate alert if the can / can't

# jQuery

jQuery is a fast, small, and feature-rich JavaScript library. It makes things like HTML document traversal and manipulation, event handling, animation, and Ajax much simpler with an easy-to-use API that works across a multitude of browsers

## Lesson One - adding javascript and jquery to your site

If you don't have a site to work on already, create an index.html file using this template

```
<!DOCTYPE html>
  <html>
    <head>
      <title>Page Title</title>
      <link rel='stylesheet' type='text/css' href='main.css'>
    </head>

  <body>
  </body>
</html>
```

Create and link a javascript file to the document (this is added to the body, as it will wait for all of the html to load before it runs)

```
  <body>
  
    <script src="main.js"></script>
  </body>
</html>
```

We can then add jQuery to use with our javascript (it is put above our main.js file as it needs to run before, as our main.js file will be accessing it)

```
  <body>
  
    <script src="http://code.jquery.com/jquery-3.1.1.min.js" integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8=" crossorigin="anonymous"></script>
    <script src="main.js"></script>
  </body>
</html>
```

## Lesson Two - using jquery

jQuery makes selecting elements on the page and manipulating them easy.

This can be done using the jQuery function, which includes a:

1. $ sign to define/access jQuery
2. (selector) to "query (or find)" HTML elements
3. jQuery action() to be performed on the element(s)

```
$('ul li').hide();

$('.page_one').addClass('active');

$('a.link_one').on('click', alert("Click!"));

$('a.link_one').on('click', function() {
  $(this).hide();
});
```

[CodePen demo](http://codepen.io/dianaklee/pen/epBypZ)


## Lesson Three - using jquery with bootstrap

You can use all Bootstrap plugins purely through the markup API without writing a single line of JavaScript. This should be slightly familiar to you, as it works similarly to how you set up bootstap.css with your html

So, to add Bootstrap.js, just include the CDN (or file location) under jQuery. Then add your personal .js file underneath (optional)

```
<!DOCTYPE html>
  <html>
    <head>
      <title>Page Title</title>
      
      <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/css/bootstrap.min.css" integrity="sha384-BVYiiSIFeK1dGmJRAkycuHAHRg32OmUcww7on3RYdg4Va+PmSTsz/K68vbdEjh4u" crossorigin="anonymous">
      <link rel='stylesheet' type='text/css' href='main.css'>
    </head>
    
  <body>
    <script src="http://code.jquery.com/jquery-3.1.1.min.js" integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8=" crossorigin="anonymous"></script>
    <script src="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha384-Tc5IQib027qvyjSMfHjOMaLkfuWVxZxUPnCJA7l2mCWNIpG9mGCD8wGNIcPD7Txa" crossorigin="anonymous"></script>
    <script src="main.js"></script>
  </body>
</html>
```

## Lesson Four - using jquery with bootstrap

[Dropdown menus](http://getbootstrap.com/javascript/#dropdowns) - Add dropdown menus to nearly anything with this simple plugin, including the navbar, tabs, and pills

[Popup boxes](http://getbootstrap.com/javascript/#modals) - Modals are streamlined, but flexible, dialog prompts with the minimum required functionality and smart defaults 

[Image slideshows/carousels](http://getbootstrap.com/javascript/#carousel ) - A slideshow component for cycling through elements, like a carousel

## Task One - adding image carousel to site

We're going to be adding an image slideshows, so if you don't want it on your site today you can add it to your Sam’s Sarnies site from last week!

1. Add an image carousel to the site (you can find images [here](https://drive.google.com/drive/u/0/folders/0Bwo5bTC_RuNia2EzQjFXa0Y0RDQ?usp=sharing#))
2. Add another feature from the [Bootstrap documentation](http://getbootstrap.com/javascript/) to your site

## Projects

For anyone struggling for ideas with their projects CFG has a list of additional ideas for things you can include in your project using JavaScript/JQuery [here](https://docs.google.com/document/d/1u8yT5evLWzAW3O9TGAfFhd7olPRDWc1bhTmXeaNBXVY/edit#)

The guidelines are:

* A visually appealing design - good use of CSS, HTML elements, and Twitter Bootstrap
  * Good formatting
  * Code split into the appropriate files
  * Files indented properly
* A live website (Github page, Heroku or own domain)
* Extras e.g. 
  * A contact form (for example name and email)
  * Social buttons
  * As many different HTML elements you can manage
  * Interactive elements (like forms) on the website don’t need to be functional but should be present if they need to be for the visual aspect of the design
* (optional) Good organisation
  * Version control using GitHub
  * Sensible commit messages
>>>>>>> 9940c068762ab1ed199e5e4aae1a315acda4c6c7
