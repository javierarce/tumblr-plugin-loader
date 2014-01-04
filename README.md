tumblr-plugins
==============

Load code based on the tags of a tumblr post.

### Installation

1. Add the ```jquery.tumblr.plugin.js``` file to your HTML page.
2. Define your plugins like this:
```js
<script type="text/javascript">
  plugins = {};
  plugins.tag1 = function($elem) { … }; // $elem is the jQuery representation of the post
  plugins.tag2 = function($elem) { … };
  plugins.tag3 = function($elem) { … };
</script>

3. Launch the plugin: 
```js
<script type="text/javascript">
  $(function() {
    $("article").tumblrPlugins({ tag: "li.tag a", plugins: ["tag1", "tag2", "tag3"] });
  });
</script>
```

----

This jQuery plugin was created using the [jQuery Plugin Template](http://kolodny.github.io/blog/blog/2013/12/27/my-favorite-jquery-plugin-template/) by Moshe Kolodny.
