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

1. Go to the [Bootstrap documentation on tables](http://getbootstrap.com/css/#tables), and study how to set it up correctly
2. Create a table using the appropriate class name
3. Complete the table by adding the head (&lt;thead&gt; ... &lt;/thead&gt;) and body (&lt;tbody&gt; ... &lt;/tbody&gt;) sections
