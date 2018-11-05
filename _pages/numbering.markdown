---
layout: post
title:  "Page numbering"
date:   2018-01-01 00:00:00 -0500
categories: documentation page numbering textbooks
published: true
permalink: numbering.html
---

Textbooks require displaying page numbers to tell the readers where they are on the book. To enable page numbering:

Check the checkbox on `page` dropdown as shown below:

<br/>
<br/>
<div class="two-third center">

<img src="https://raw.githubusercontent.com/marvindanig/assets/master/numbering.jpg" width="100%" />
</div>
<br/>
<br/>

If you're using Bookiza, set the `has_page_numbers` property on [.bookrc](https://bubblin.io/bookiza/docs/preprocessors) to `true`, like so:

	$ vi .bookrc 	// In your project root.

```json
{
  "mode": {
    "HTML": "haml",
    "CSS": "scss",
    "JS": "js",
    "HEAD": "html"
  },
  "name": "My next great textbook!",
  "type": "text",
  "has_page_numbers": true  
}

```