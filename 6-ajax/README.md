# AJAX

Firstly, download the website.zip from [here](https://drive.google.com/open?id=0B6i1g6ETAjs6UHlqZjRBR2tBcEU)

## Lesson One - plugins

### Google Analytics

Google Analytics is an analytics service provided for free by Google. It allows you get an overview of how many people are visiting your site, where they come from and what they do on your site

To use Google Analytics you need to place JS Plug-In, a snippet of JavaScript, (that they provide) on each of the HTML pages on your site. When a user visits the page, the javascript sends a message to the Google Analytics site logging the visit

1. Set up a Google Analytics account [here](https://analytics.google.com)
2. Go to the Admin section and create an account for your site
3. Click on the Tracking Info under the Property section, click on “Tracking Code” and install the analytics code on all the pages of your site

### Google Forms

Google Forms uses the &lt;style&gt;iframe&lt;/style&gt; tag to embed a mini-form document into your web page, where you want it. This can be a quick and easy way to collect information from users on your website via online forms.

1. Create a google form adding in your own content to the form
2. Make it available by clicking on the “Send” button in the top right corner of the screen and click the “&lt;style&gt;&lt;/style&gt;” icon to “Embed HTML”
3. Copy and paste the link provided by this icon

### Github Pages

Remember in Session 1 we previously introduced you to Domain Names? In case you need a quick recap, in order to put up your own website at your own domain name you need two things:

1. A web server to serve your site
2. A domain name to point towards it

As you’ve been working with Github and publishing your sites via Github pages we wanted to give you some more guidance on setting up a custom domain using [Github Pages](https://help.github.com/articles/quick-start-setting-up-a-custom-domain/)

## Lesson Two - api's

### API

We can use AJAX to interact with an API. But what is AJAX and what is an API?

An API (Application Programming Interface) is best thought of as a contract provided by one piece of computer software to another

Your website would send a request to an API (in a structured format), and it with a structured response. The structure of request and response would be documented upfront by the API we us and is likely to remain constant

So, instead of our website opening [DarkSky](https://darksky.net/) and reading the webpage like a human does, interpreting the content. We can use the API they provide to easily traverse the data

Sign up to use this API [here](https://darksky.net/dev/register)

### JSON

The format returned by the API's we will be using is known as JSON. JSON is a way of sharing data (usually between the browser and a server)

JSON returns the data to JavaScript in an the form of an Object, which JavaScript understands, and can then store, manipulate and use that data on your site. An Object is just a really easy and convenient way to store data in JavaScript

```
var person = {
  "name": "James",
  "age": 20
}

alert("My name is " + person.name);
alert("I am " + person.age + " years old");
```

## Lesson Three - ajax (part 1)

We connect to an API using AJAX. AJAX stands for Asynchronous Javascript and XML and supports partial updates to pages without having to post the entire page back to the server.

There are plenty of options for AJAX. The two most notable are Microsoft's ASP.NET AJAX (formerly Atlas) and jQuery (which we'll be using!). It is is easy to set up with jQuery, and allows very granular control over the querying and updating of your page

To make an ajax request we start by writting some jQuery

```
$.ajax();
```

We then give it an object, which will be it's options

```
$.ajax({
  type: 'GET',
  url: 'https://api.json.com/request/'
});
```

Now, to recieve and store the response we use a success option

```
$.ajax({
  type: 'GET',
  url: 'https://api.darksky.net/forecast/37.8267,-122.4233',
  success: function(data) {}
});
```

And we can access that data like so
```
$.ajax({
  type: 'GET',
  url: 'https://api.darksky.net/forecast/37.8267,-122.4233',
  success: function(data) {
    alert(data.timezone);
  }
});
```

## Lesson Four - ajax (part 2)

Some of this weather data is useful, but is stored in an array object - meaning that we have to iterate over it to access each variable

An Array object is used to store multiple values in a single variable

```
var people = ["James", "Mike"]
```

Array indexes are zero-based: The first element in the array is 0, the second is 1, and so on. So, to take Mike's name out of the array we would do

```
var people = ["James", "Mike"]

alert( people[1] );
```

To iterate over array we can use jQuery. As an example we will iterate over the "daily" value from the API, to get the "summary"

```
$.ajax({
  type: 'GET',
  url: 'https://api.darksky.net/forecast/37.8267,-122.4233',
  success: function(data) {
    var summary = "";
    
    $.each(data.daily.data, function(index, value) {
      summary = summary + value.summary;
    });
    
    alert(summary);
  }
});
```

## Lesson Five - ajax (part 3)

Finally, if you want to add this list to your page you can do the following

```
$.ajax({
  type: 'GET',
  url: 'https://api.darksky.net/forecast/37.8267,-122.4233',
  success: function(data) {
    var summary = "<ul>";
    
    $.each(data.daily.data, function(index, value) {
      summary += "<li>" + value.summary + "</li>";
    });
    
    summary += "</ul>";
    
    $('.list').html(summary);
  }
});
```
