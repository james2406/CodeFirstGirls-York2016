# Intro to HTML

## Task One

1. Within your coding_course folder create a new folder called first_site
1. Open the first_site folder created in your text editor of choice (sublimetext, atom...)
2. Write "Hello"
3. Save this file as index.html in the first_site folder
4. Open index.html in your browser of choice (chrome, firefox...)

We use index.html as our homepage as we may have other files in our folder, such as about.html and contact.html. When a user loads our site, they are automatically directed to our index file

## Lesson One - tags

HTML uses a set of elements for different types of content, which defines their value/meaning. For example, a "&lt;p&gt;" element indicates a paragraph and the "&lt;img&gt;" indicates an image

These elements are known as tags. Tags are enclosed by angle brackets (&lt;&gt;), and the closing tag begins with a forward slash. For example

```
<h1>Hello World!</h1>
```

Some tags close by default. An example of this is the &lt;img&gt; tag

```
<img src="imageOne.jpg" alt="Image One">
```

Finally, we can give our tags attributes, that can serve various different purposes. In the case below, our attribute is giving our tag an id

```
<div id="main"></div>
```

## Lesson Two - formatting

Formatting is generally up to the programmer when it comes to html however, the common practice is to nest tags that are present within other tags. So instead of this

```
<div id="main"><h1>Title</h1><h2>subtitle</h2></div>
```

The valid way would be to present it like this

```
<div id="main">
  <h1>Title</h1>
  <h2>subtitle</h2>
</div>
```

Much easier to read!

## Lesson Three - the HTML DOM

The Document Object Model (DOM) specifies the hierarchical layout of the HTML document, and is the agreed interface (that is platform / language independent). In other words, it tells the browser where to look for a specific parts to the document

Every HTML5 document requires this layout

```
<!DOCTYPE html>
  <html>
    <head>
      <title>Page title</title>
    </head>
    
  <body>
    ( html goes here! )
  </body>
</html>
```

And each element/tag does the following:

* The !DOCTYPE tells you what version of html you’re using
* Everything is wrapped in an &lt;html&gt; ... &lt;/html&gt; tag
* the &lt;head&gt; ... &lt;/head&gt; is used to provide information about the page
* the text within &lt;title&gt; ... &lt;/title&gt; will be displayed in the browser bar
* Only things within the &lt;body&gt; ... &lt;/body&gt; tags are displayed on the page

## Task Two

1. [Download this link](https://github.com/code61/learning_html/archive/master.zip)
3. Extract the zip file and delete the zip
4. Move those files to your first_site folder
5. Open the the first_site folder in your text editor
6. Open the file example.html in Chrome and look around with the developer tools
7. Open the file notes.html in your text editor.
8. Change notes.html into valid html so that it looks like notes_solution.jpg

## Homework

1. Complete the whole of Project 2 on the [General Assembly Dash site](https://dash.generalassemb.ly/)
2. What is CSS? Get ready for the next class by watching [this fun video](https://www.youtube.com/watch?v=s7ONvIgOWdM)
3. (Optional) Do the projects from the [Codecademy Web Track](https://www.codecademy.com/learn/web) Sections 4, 5 & 6
4. Use what you've learnt from the HTML exercise and the Dash projects to improve your first_site/index.html


