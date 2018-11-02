---
layout: post
title:  "Structure of <page>"
date:   2018-01-01 00:00:00 -0500
categories: documentation HTML structure concept
published: true
permalink: structure.html
---

A <`page`> inside a Superbook is a typical `webpage`.

The only difference is that it has only a limited amount of responsive content. The `<page>` is expected to fit the entire available height of the viewport (and remain above the fold) and go from portrait to landscape not only responsively but also with an intent to occupy maximum visual size. Since in case of a Superbook, a `<page>` is a virgin `iframe`, it contains everything: a `<head>`, a `<body>` alongwith `<style>` and `javascript` if necessary.

Here's how the internals look:

{% highlight html %}
<!DOCTYPE html>
<html>
    <head>
        <title> { _title_of_the_book_ + /page_no } </title>
        <style>
        	{ /* Insert _book_layout_template_ + _page_specific_styles_ if any? */
        	  /* Generally, the html, body {} elements are assigned a height of 100vh and width 100vw.  */
        	  /* See CSS template of a book deployed in production: */
        	  /* https://github.com/marvindanig/bookiza-framework/blob/master/templates/style.scss */ }
      	</style>
      	<!-- Other head resources via cdnjs or polyfill.io if any -->
    </head>
    <body>
      <!-- Few paragraphs of neatly formatted content here. -->
      …
      …
      …
      <!-- Author scripts inserted here at the bottom of iframe -->
    </body>
</html>
{% endhighlight %}

As you can see above there are four pieces that go into making a page: HEAD resources, BODY text, STYLE for layout and SCRIPTS at the bottom of the iframe, if required. All these four pieces can be fiddled with using Bubblin's [in-browser]({{ site.baseurl }}{% post_url 2018-01-01-setup %}) editor as shown below:

<div class="two-third center">
  <img src="https://raw.githubusercontent.com/bubblin/Official-Handbook/master/assets/images/bubblin-editor-browser-frame.jpg" width="100%" />
</div>