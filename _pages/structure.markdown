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
    </head>
    <body>
      <!-- Few paragraphs of neatly formatted content here. -->
    </body>
</html>
{% endhighlight %}