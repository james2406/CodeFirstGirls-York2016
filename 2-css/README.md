# Intro to CSS

Cascading Style Sheets (CSS) is a style sheet language used for describing the presentation of a document. It was created by the World Wide Web Consortium (W3C) to solve the problem of formatting and styling a document

A great example of the power of css is CSS Zen Garden. They provide a [single html file](http://www.csszengarden.com/1/), and encorage people to change the design just with css. The featured designs can be found [here](http://www.csszengarden.com/)

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

## Task One

1. 
