---
layout: post
title:  "Typography"
date:   2018-01-01 00:00:00 -0500
categories: documentation introduction
published: true
---

Choosing typography for your Superbook is like choosing it for a website. 

Needless to mention, any typography that you opt for must be web compatible. Bubblin provides a handful selection of fonts that is strongly cached using a `serviceworker`. The following `import` is available via the root window i.e. `spine_url` into a `seamless` `iframe`, ala `<page>`:

```
@import url(https://fonts.googleapis.com/css?family=Raleway|Lobster|EB+Garamond);
```

- EB Garamond, serif for all content,
- Raleway, sans serif for occasional tang, especially with numbers, and
- Lobster, cursive on invoice, ledgers or tang.

Using any of the fonts listed above (or browser defaults) will keep the number of requests off and weight of your book in control.

## Custom fonts

If you're considering the [Google Fonts API](https://developers.google.com/fonts/) or any other font hosting service for custom fonts on your book, we recommend you do so as described in the section on [best practices]({{ site.baseurl }}{% post_url 2018-01-01-practices %}) for typography.

```HEAD
<link href='//fonts.googleapis.com/css?family=Playfair+Display:400' rel='stylesheet' type='text/css'>
```


```CSS
	/*
	* Add the following snippet for
	*  typography via layout templates:
	*  path/to/{bookiza project}/templates/style.css
	*/
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

Generally speaking use lightweight fonts with a specific weight (for example, `Playfair+Display:400` and not `Playfair+Display:400, 700, 900` or the entire selection) and `serif` motifs for the body of text. Use `viewport units` to scale the `font-size` responsively. Use a high contrast between text and background as recommended in WCAG 2.1 guidelines of 2018. Always test your book for text scaling and overflow as per design principles of `strong layouts`.

