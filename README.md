tumblr-plugin-loader
==============

Load JavaScript code based on the tags of a Tumblr post.

### Installation

- Add the ```jquery.tumblr.plugin.js``` file to your HTML page.  
- Define your plugins like this:

```js
  plugins = {};
  plugins.tag1 = function($elem) { … }; // $elem is the jQuery representation of the post
  plugins.tag2 = function($elem) { … };
  plugins.tag3 = function($elem) { … };
```
- Launch the plugin: 

```js
  $(function() {
    $(".post").tumblrPlugins({ tag: "li.tag a", plugins: ["tag1", "tag2", "tag3"] });  
  });  
```

----

This jQuery plugin was created using the [jQuery Plugin Template](http://kolodny.github.io/blog/blog/2013/12/27/my-favorite-jquery-plugin-template/) by Moshe Kolodny.
