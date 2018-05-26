---
layout: post
title:  "Best Practices"
date:   2018-01-01 00:00:00 -0500
categories: superbooks documentation best practices css html javascript
published: true
---

Here are a bunch of goodies and "no goods" when you're making a book for the web:

1. **Never use a CSS framework on your book.**
	+ i) Avoid `bootstrap`, `foundation` or even Eric Meyer's `_reset`, it will ruin your layout.
	+ ii) CSS frameworks are designed for apps and not books.
	+ iii) Use open source CSS [templates](https://github.com/bookiza/templates) for layouts.
	+ iv) Write your own style by hand if it is needed.
	+ v) Most books do not require more than 10 lines of css code, so writing by hand is highly recommended.


2. **Always set `typography` from the `<head>` of the parent**
	+ i) Use only the CSS template option to add typography for your book
	+ ii) Include `@font-faces` on the first line of your CSS.
	+ ii) Always use web-compatible fonts that are light.
	+ iii) More often than not, stick to the default typography set by Bubblin i.e. [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) by George Duffner for text heavy books.
	+ iv) Choose the largest possible `font-size` in `viewport units` only. We recommend keeping size of text between `4.0vw - 4.2vw` with `line height` of `1.25` at least.
	+ v) Always use high contrast between text & background on your book.


3. **Never copy paste HTML straight from a document**
	+ i) HTML extracted from PDFs or Epubs or other such file systems is usually very low quality. Use carefully.
	+ ii) Avoid copying HTML straight up from websites like Wordpress or Medium, unless it is just paragraph tags.
	+ iii) There is no one-to-one correlation between a PDF file and Superbook. Superbooks are far more capable and accessible.


4. **Internal links**
	+ i) Internal anchors must use Bubblin's (internal hyperlinking API)[https://bubblin.io/book/official-handbook-by-marvin-danig/33], i.e. use class name `page` and `href:` to `page_no`.
	+ ii) Always avoid reloading the whole book when the content is available locally on client.

5. **No ad scripts**
	+ i) No ad or tracking scripts are allowed inside a book. You'll be banned.
	+ ii) Try and keep your scripts to minimum.