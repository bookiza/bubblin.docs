---
layout: post
title:  "Structure of <page>"
date:   2018-01-01 00:00:00 -0500
categories: documentation HTML structure concept
published: true
permalink: structure.html
---

A `<page>` inside a Superbook is a typical iframe. Or in other words a standard `webpage` HTML.

The only difference is that it has only a limited amount of content which _must_ remain above the fold and _must_ also scale responsively. The `<pages>` will automatically fit the entire available height and width of the viewport and go from `portrait` to `landscape` mode automatically, all while maintaining a fixed aspect ratio that occupies maximum available real estate. 

To see this in action, trying resizing your browser on any page of the following book:


> [Bookiza Documentation](https://bubblin.io/book/bookiza-documentation-by-marvin-danig/1) (Resize the browser after flipping through a few pages.)




Since a `<page>` on a Superbook is a virgin `iframe`, it contains the usual markup that is plainly used on web. By and large there are four main components of a `<page>`, and here's what the skeletal structure looks like:

{% highlight html %}
<!DOCTYPE html>
<html>
    <head> <!-- COMPONENT-IV -->
        <title> { _title_of_the_book_ + /page_no } </title>
        <style> 
        	{ /* <!-- COMPONENT-II --> */ 
            /* Insert _book_layout_template_ + _page_specific_styles_ if any? */
        	  /* Generally, the html, body {} elements are assigned a height of 100vh and width 100vw.  */
        	  /* See CSS template of a book deployed in production: */
        	  /* https://github.com/marvindanig/bookiza-framework/blob/master/templates/style.scss */ }
      	</style>
      	<!-- HTML of other head resources via cdnjs or polyfill.io here. (COMPONENT-IV) -->
    </head>
    <body>
      <!-- COMPONENT-I (This is the content of the page that the reader sees) -->
      <!-- Few paragraphs of neatly formatted content here. -->
      …
      …
      …
      <script type="text/javascript">
        // COMPONENT-III
        // Author scripts inserted here at the bottom of iframe 
      </script>
    </body>
</html>
{% endhighlight %}

As you can see from above there are four main pieces that go into making a complete `<page>`: 

1. BODY HTML (Component-I), 
2. STYLE rule for layout (Component-II), 
3. SCRIPTS at the bottom of the `iframe` (Component-III), if required, and
3. HEAD resources (Component-IV), if required.

All four components can be fiddled with using Bubblin's [in-browser]({{ site.baseurl }}{% post_url 2018-01-01-setup %}) editor as shown below:

<div class="two-third center">
  <img src="https://raw.githubusercontent.com/bubblin/Official-Handbook/master/assets/images/bubblin-editor-browser-frame.jpg" width="100%" />
</div>


If you're using [Bookiza Abelone](https://bookiza.io) to manage your manuscript, it will show the same `<page>` structure inside the `manuscript/` folder. There you'll see subdirectories like `page-1`, `page-2`, `page-3`… `page-2N`, with each to carry four components that make up a `<page>` i.e. a `body.html` file (mandatory), a `style.css` file, a `head.html` file and a `scripts.js` file if required. 

