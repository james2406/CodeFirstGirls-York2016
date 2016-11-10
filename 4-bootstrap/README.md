# Bootstrap

You’ve seen quite a bit of CSS now; it all seems quite straightforward. Unfortunately, browsers will render CSS with subtle differences. Making your site look good (or even presentable) across browsers takes time, effort and experience

Also, in the last 5 years the mobile web has exploded. So, you need to ask yourslef: how will my website look when viewed on a mobile?

## Lesson One - twitter bootstrap

Twitter Bootstrap  is a 'Web Application Framework'. It includes a set of CSS (and JavaScript) files, released by the makers of Twitter, and maintained by some of its developers.

Bootstrap provides a set of ready-made CSS files that provide pre-built functions for common web development requirements, and pre-built solutions to common presentation requirements in a cross-browser / responsive way.

To make use of Twitter Bootstrap, you need to do two things:

Link to the Twitter Bootstrap stylesheet in the head of your html page

```
<head>
  <title>Page title</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
  <link href="css/bootstrap.css" rel="stylesheet">
</head>
```

Attach the relevant Twitter Bootstrap class to your html element

```
<button class='btn btn-lrg'>Twitter</button>
```

To understand how to use Bootstrap, or any framework for that matter, it is vital to read the documentation. The documentation for Bootstrap is available [here](http://getbootstrap.com/getting-started/)

## Task One

In this task we are going to create a table, with a zebra pattern

1. Go to the [Bootstrap documentation on tables](http://getbootstrap.com/css/#tables), and study how to set one up correctly
2. Create a table using the appropriate class name/s
3. Complete the table by adding the head (&lt;thead&gt; ... &lt;/thead&gt;) and body (&lt;tbody&gt; ... &lt;/tbody&gt;) sections
4. Preview your page, and inspect the Bootstrap styles applied using your browsers developer tools

## Lesson Two - responsive design

Responsive design means designing your sites so that they look good on all screen sizes

It is common pratice to design your website with a ‘mobile first’ approach. Bootstrap encourages you to do this, meaning your site will look good at all sizes from the very beginning

Bootstrap does this by including a responsive, mobile first fluid grid system that lets you split the screen up into 12 columns and lets you customise the size of your HTML element as a fraction of 12. The documentation goes through this [here](http://getbootstrap.com/css/#grid-example-basic)

## Task Two

1. [Download this link](https://github.com/code61/bootstrap_exercise/archive/master.zip)
2. Extract the zip file into your coding_course folder, and delete the zip

The tasks from now will be to create the website for ("Sam's Sarnies")[http://code61.github.io/bootstrap_exercise/] using Twitter Bootstrap

1. Goto the [Bootstrap website](http://getbootstrap.com/) and click the Download Bootstrap button
2. Unzip and copy the 'dist' folder into the bootstrap_exercise folder
3. Open bootstrap_exercise in Sublime Text, and bootstrap_exercise/index.html in Chrome
4. Add a link to the twitter bootstrap stylesheet into index.html (shown in Lesson One ^)
5. Refresh the page in Chrome. Notice the changes

## Lesson Three - bootstrap layout

Bootstraps responsive, mobile first fluid grid system gives you several options on how to layout your page. We’ll just look at Containers and Columns for now:

Containers - Bootstrap requires a containing element to wrap site contents and house our grid system. You may choose one of two containers to use in your projects. Note that, due to padding and more, neither container is nestable.

```
<div class="container">
  ...
</div>
```

Columns - Predefined grid classes like '.row' and '.col-md-' are available for quickly making grid layouts. Less mixins can also be used for more semantic layouts.

```
<div class="row">
  <div class="col-md-8">.col-md-8</div>
  <div class="col-md-4">.col-md-4</div>
</div>
```

The number after the 'col-sm' determines how many of the 12 grid columns that page column takes up

The '-sm' bit determines the width at which the columns will collapse on top of each other

## Task Three

1. Add a div class='container' around the page content
2. Create a row at the top of the page, with two columns
3. Set the left column to be twice as wide as the right column
4. Put the h1 in the left column and the img(src='images/sandwich.png') on the right
5. Create a row with three equal columns to hold each of 'The Buzz' divs

## Task Four

Now that we have set up our layout, we can being experimenting with some other features has to offer!

### Typography

1. Open and skim the [typography section](http://getbootstrap.com/css/#type) of the bootstrap docs
2. Change the quotes in 'The Buzz' to use blockquotes
3. Change the paragraphs in 'Our mission' to be [lead body copy](http://getbootstrap.com/css/#type-body-copy)

### Buttons

1. Open and skim the [buttons section](http://getbootstrap.com/css/#buttons) of the bootstrap docs
2. Change the 'Send' button to a success button
3. Make the social links at the bottom into large buttons

### Images

1. Open and skim the [images section](http://getbootstrap.com/css/#images) of the bootstrap docs
2. Make the images in 'The Buzz' round, by adding the img-circle class
3. Center the image by adding the alignment class text-center
4. Change the main sandwich image into an img-responsive, as described in the [responsive images section](http://getbootstrap.com/css/#overview-responsive-images)


## Lesson Four - modifying bootstrap

You don't modify Bootstrap styling within the Bootstrap document, but in your 'main.css' file

When a new version of Bootstrap comes out you can upgrade by dragging the new version over the top of the old, without losing any modifications!

To set this up you add your css link underneath the bootstrap.css link. It goes underneath as the browser will read your css in order of its position, allowing you to override existing Bootstrap styles

```
<head>
  <title>Page title</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  
  <link href="css/bootstrap.css" rel="stylesheet">
  <link href="css/main.css" rel="stylesheet">
</head>
```

## Task Five

1. Create a file called main.css
2. Add the main.css file to the head of your document

### Buttons

1. Add the folowing code to your main.css file
2. View the changes in your browser

```
#social-buttons button {
  color: white;
}

.btn-twitter {
  background-color: #00acee;
  border-color: #009ad5;
}

.btn-facebook {
  background-color: #4868ac;
  border-color: #314776;
}

.btn-pinterest {
  background-color: #b62f26;
  border-color: #b62f26;
}
```

### Background
