---
layout: post
title:  "Structure of <page>"
date:   2018-01-01 00:00:00 -0500
categories: documentation HTML structure concept
published: true
permalink: structure.html
---

A <`page`> inside a Superbook is a typical iframe or in other words a standard `webpage`.

The only difference is that it has only a limited amount of content which _must_ scale responsively. The `<pages>` will automatically fit the entire available height and width of the viewport and go from `portrait` mode to `landscape` mode automatically while maintaining a standard page aspect ratio that occupies maximum available real estate. To see this working, trying resizing your browser on any page of this book:


> Demo: [Bookiza Documentation](https://bubblin.io/book/bookiza-documentation-by-marvin-danig/1) (Resize the browser after flipping through the book.)




Since a `<page>` on a Superbook is a virgin `iframe`, it contains the usual markup and can contain everything else: like subresources of the `<head>`, HTML belonging to the `<body>` or `<style>` rules and even plain `javascript` if that is required.

Here's how the internals of a `<page>` look like:

{% highlight html %}
<!DOCTYPE html>
<html>
    <head> <!-- Component-IV -->
        <title> { _title_of_the_book_ + /page_no } </title>
        <style> 
        	{ /* <!-- Component-II --> */ 
            /* Insert _book_layout_template_ + _page_specific_styles_ if any? */
        	  /* Generally, the html, body {} elements are assigned a height of 100vh and width 100vw.  */
        	  /* See CSS template of a book deployed in production: */
        	  /* https://github.com/marvindanig/bookiza-framework/blob/master/templates/style.scss */ }
      	</style>
      	<!-- HTML of other head resources via cdnjs or polyfill.io here. (Component-IV) -->
    </head>
    <body>
      <!-- Component-I (This is the content of the page that the reader sees) -->
      <!-- Few paragraphs of neatly formatted content here. -->
      …
      …
      …
      <script type="text/javascript">
        // Component-III
        // Author scripts inserted here at the bottom of iframe 
      </script>
    </body>
</html>
{% endhighlight %}

As you can see above there are four pieces that go into making a complete `<page>`: 

1. BODY HTML (Component-I), 
2. STYLE rule for layout (Component-II), 
3. SCRIPTS at the bottom of the `iframe` (Component-III), if required, and
3. HEAD resources (Component-IV), if required.

All the four components can be fiddled with using Bubblin's [in-browser]({{ site.baseurl }}{% post_url 2018-01-01-setup %}) editor as shown below:

<div class="two-third center">
  <img src="https://raw.githubusercontent.com/bubblin/Official-Handbook/master/assets/images/bubblin-editor-browser-frame.jpg" width="100%" />
</div>


In general, if you're using [Bookiza Abelone](https://bookiza.io) to write your book, it will also contain the same `<page>` structure inside the `manuscript/` folder. There you'll see subdirectories like `page-1`, `page-2`, `page-3`… `page-2N`, each carrying the four components as discussed above i.e. a `body.html` file, a `style.css` if required, a `head.html` if required and a `scripts.js` file if required. 

