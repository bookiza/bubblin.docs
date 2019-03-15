---
layout: post
title:  "Typography"
date:   2019-01-01 00:00:00 -0500
categories: documentation introduction
published: true
---

Choosing typography for a Superbook is a lot like choosing it for a website. More or less. =)

First off, any typography that you decide to use _must_ be web-compatible. Bubblin provides a small selection of fonts that are strongly cached using a Service Worker so that no extra http request is fired for these fonts. 

The following `@import` is available via the root window i.e. `spine_url` of your book:

```
@import https://fonts.googleapis.com/css?family=Raleway|Lobster|EB+Garamond:400,400i

```



- [EB Garamond](https://fonts.google.com/specimen/EB+Garamond), serif for main content (text) of the book,
- [Raleway](https://fonts.google.com/specimen/Raleway), sans serif for occasional use, especially with numeric text on book (but not page numbers), and
- [Lobster](https://fonts.google.com/specimen/Lobster), cursive on invoice, ledgers or tang.

Using any of the fonts listed above or the default ones on a browser will keep the number of http requests and the total weight of your book in control, and thus not affect the speed at which your book loads on the client. This is specially important for users on low powered  devices such as mobile.

### Using custom fonts

If for some reason you are considering using custom web-compatible typography such as from awesome [Google Fonts API](https://developers.google.com/fonts/) (or any other font hosting service) on your book, we recommend you do so as specified in the section on [best practices]({{ site.baseurl }}{% post_url 2018-01-01-practices %}).

Include the font using link helper like so:

```HEAD
<link href='//fonts.googleapis.com/css?family=Playfair+Display:400' rel='stylesheet' type='text/css'>

```

And then on your layout template, add the clause to typeset your entire book:

```CSS
	
	/* Add the following snippet for
	*  typography via layout templates:
	*  path/to/{bookiza project}/templates/style.css */

	@charset "UTF-8";

	html, body {
	  color: #2f2f2f;
	  background-color: #f9f7f1;
	  font: 4.2vw/1.4 'Playfair Display', serif;
	  margin: 0 0;
	  overflow: hidden;
	  color: #444;
	  height: 100vh;
	  width: 100vw;
	}
	…
	…
	// Other styles below.
	…
	…
```

### General advice:

1. Use lightweight fonts with a specific weight. For example, use `Playfair+Display:400` to specify weight of 400 and not load `Playfair+Display:400, 700, 900` or the entire selection unless you _really_ need to. 

2. Use `serif` motifs for the body of text, they add a professional feel on your book. This tip is opposite to the general design advice on web, please note.

3. Use `viewport units` to scale the text responsively. 

4. Use a high contrast between text and background as per recommendation @WCAG 2.1 guidelines of 2018. 

5. Always test your book for scaling, responsiveness and overflow triggers per specification on [strong layouts](https://bubblin.io/docs/layouts).

