# Intro to CSS

Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document. It was created by the World Wide Web Consortium (W3C) to solve the problem of formatting and styling a document

A great example of the power of css is CSS Zen Garden. They provide a [single html file](http://www.csszengarden.com/1/), and encorage people to change the design just with css. The featured designs can be found [here](http://www.csszengarden.com/)

## Task One

1. Within your coding_course folder create a new folder called session_2
2. [Download this link](https://github.com/CodeFirstGirls/html2/archive/master.zip)
3. Extract the zip file and delete the zip
4. Move those files to your session_2 folder

## Lesson One - linking css to the DOM

There are 3 ways of adding your css to your html file:

1. Put the css inline in the html
2. Put the css in a &lt;style&gt; ... &lt;/style&gt; section in the &lt;head&gt;
3. Link to a separate .css file in the &lt;head&gt;

The first option means no seperation of html and css, and each element will have to be styled individualy
The second option is better, but it is recommended that html and css are kept completely seperate. So, not even on the same page

## Lesson Two - link to a separate css file

The third option is the best, as we will have a seperate file just for css. If we ever have more than one page, we can just add the link to that new page

```
<!DOCTYPE html>
  <html>
    <head>
      <title>Page title</title>
      <link rel='stylesheet' type='text/css' href='main.css'>
    </head>
    
  <body>
  </body>
</html>
```

## Lesson Three - changing link directory

The link below is set to 'main.css'

```
<link rel='stylesheet' type='text/css' href='style.css'>
```

However, if our css is not in the same directory we may have to navigate through our folder structure. For example, if this was our directory. How would we link to main.css or background.png from index.html?

```
Website
---- index.html
---- images
| ---- background.png
---- stylesheets
| ---- main.css

```

The answer can be found by using three different styles:

1. Absolute links - include the complete url to the resource you’re linking to (start with either http:// or https://) e.g href="http://www.website.com/stylesheets/main.css"
2. Root-relative links - contain the path to the resource relative to the site’s root, this links begin with a " / " e.g href="/stylesheets/main.css"
3. Document-relative links - contain the path to the resource relative to the file where the link is written. In the case that we want to travel from main.css to the image we don't start with " / " but " ../ " (meaning travelling up the file tree) e.g url("../images/background.png")

So, " ./ " means in the folder that I'm in and " ../ " means in the folder above the one that I'm in

## Task Two

1. Open the session_2 folder created in your text editor of choice (sublimetext, atom...)
2. Make a separate CSS file, called exercise1.css
3. Link your exercise1.css file to your exercise1.html file within the &lt;head&gt; tag

## Lesson Four - writing CSS & basic definitions

This is called a rule set a single section of CSS including a:
* selector (h1)
* curly braces ({})
* declaration of properties (color) and values (red)

```
h1 {
  color: red;
}
```

We can target various other selectors as well as altering an array properties with different values

```
p {
  font-family: 'Arial';
}

h2 {
  font-size: 20px;
}

h3 {
  background-color: green;
  font-size: 2px;
}
```

## Task Three

1. Open your exercise1.css file
2. Make the h1 of exercise1.html turn red
3. Make the exercise1.html look like exercise1_solution.png

---

## Lesson Five - using id & class selectors

HTML tags can have attributes which provide additional information about the element
e.g with a link you would use a href="" attribute
e.g with a img you would use a src="" attribute

However, there are attributes that can be added to any tag, including id's and classes

```
<h1 id="header_one">Header</h1>

<ul id="list">
  <li class="list_item">One</li>
  <li class="list_item">Two</li>
</ul>
```

The difference between an id and a class is:
id - can only target one elment on a page
class - can target multiple elments on a page

To target an id we use a " # ", and to target a class we use a " . "


```
h1 {
  font-family: 'Arial';
}

h1#header_one {
  font-weight: 600;
}

ul#list {
  background-color: yellow;
}

li.list_item {
  list-style-type: none;
}
```
