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
  <link href="css/main.css" rel="stylesheet">
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
