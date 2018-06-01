---
layout: post
title:  "Best Practices"
date:   2018-01-01 00:00:00 -0500
categories: superbooks documentation best practices css html javascript
published: true
---

A bunch of "goodies" and "no good" when you're making a Superbook for web.

1. #### Always set `typography` from the `<HEAD>` of layout template.
	+ Use `style.css` template option to add typography on your book
	+ Include `@font-faces` on the first line of your CSS.
	+ Always use web-compatible fonts that are light.
	+ More often than not, stick to the default typography provided by Bubblin i.e. use [EB Garamond](https://fonts.google.com/specimen/EB+Garamond) by George Duffner for your content.
	+ Choose the largest possible `font-size` in `viewport units` for readability. We recommend keeping the `font-size` between `4.0vw - 4.2vw` with a `line height` of `1.4` at least, and use hosted typography only when absolutely necessary.
	+ Always use a high contrast between text & background for your content.


2. #### Never use CSS framework on a Superbook
	+ Avoid CSS frameworks like `bootstrap`, `foundation` or even Eric Meyer's `_reset` CSS because it may ruin your layout.
	+ CSS frameworks are meant for apps and not books.
	+ Use layout [templates](https://github.com/bookiza/templates) for books instead, they are open source (MIT licensed) and meant for Superbooks. Contributions are welcome.
	+ Write style by hand if it is necessary, test scaling from mobile to television. Display support information clearly on `Cover` or landing page.
	+ Most books require no more than 10 lines of `CSS` code, so writing by hand is definitely recommended.


3. #### Avoid copy pasting HTML straight from a document
	+ HTML extracted from PDFs or Epubs or any other such file systems is usually low quality. Review carefully before placing it inside a Superbook.
	+ Unless it is just paragraph tags avoid copying HTML straight from websites like Wordpress or Medium.


4. **Internal links**
	+ Internal anchors must use Bubblin's [hyperlinking API](https://bubblin.io/book/official-handbook-by-marvin-danig/33) by adding a class attribute `page` and `href:` to `page_no` being linked.
	+ Avoid reloading the whole book when the content being jumped to is available locally on client via the `hyperlinking api` linked above.

5. **No ad scripts**
	+ No ad or tracking scripts are allowed inside a Superbook. You'll be banned.
	+ Try and keep your scripts to minimum.