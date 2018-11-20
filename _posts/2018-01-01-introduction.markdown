---
layout: post
title:  "Introduction"
date:   2018-01-01 00:00:05 -0500
categories: documentation introduction
published: true
---

Bubblin is a storytelling substrate for longform.

A site for the creative ones to publish a "well formatted" corpus like that of a book, novel, comics or a magazine. It is a fully managed Superbook container service that hosts open and accessible *codex* over the web. Bubblin comes with a deeply integrated publishing toolchain for the 
<a rel="nofollow" href="https://en.wikipedia.org/wiki/Post-PC_era">Post-PC era</a>.

<a href="https://bubblin.io"><img src="https://raw.githubusercontent.com/marvindanig/assets/master/bubblin.png" width="200px" /></a>

You can also read this documentation in form of a [Superbook](https://bubblin.io/book/official-handbook-by-marvin-danig/1) on your iPad.

### What is a Superbook?

> Superbook means **superclass** of an object like book.

It is an empty container for any kind of longform: books, novels, comics, magazine or anything that needs multi-page storytelling. Or even a greeting card like [this](https://bubblin.io/book/i-love-you-by-marvin-danig/1). 

Superbooks work like a blog so you can publish, update or unpublish any time you like. 

### Why Superbooks?

Web is generally bad at longform. Handling a large body of text has not only been traditionally difficult (from the beginning of web/time?) but nigh impossible to enjoy as a reader, as compared to say a physical book. It is no wonder that most people (including developers themselves) prefer buying a physical book even for subjects like CSS or JavaScript where the tech moves faster than print could roll out. Apart from issues of inaccessibility of inner pages (or of content deep down a long scroll) and a scourge of propreitary file formats that are generally incompatible with each other, a loose layout and reflow of text makes it hard for book lovers to enjoy longform online the way they do with a physical book: ala, tight packaging and formatting, and a high quality product. A website or an enterprise-y file (like PDF) could never equal the firm experience of a physical book. It wasn't designed that way.

Enter, Superbooks. :-)

Superbooks introduce tradtional book reading experience on web. It uses some of the very same design principles that make physical books so successful. And goes beyond from there. We revisited every accessibility principle out there by picking up best of both the worlds: physical books and web, and smushed it together to build a robust Superbook container that is both scalable and responsive. For example, primary control of a Superbook is page turn.

Want to learn how it all works? Start with a chapter on the underlying [concept]({{ site.baseurl }}{% post_url 2018-01-01-concept %}).

### Advantages 
Publishing your book directly on web has some natural advantages. For example, web takes care of the distribution part automatically and at a very low cost. People can enjoy your work without needing to download an artifact to their disk or owning specialized hardware. You can attract readers who don't plan ahead on reading a book as much and gain on impulsive readers. Despite being on web your book is available offline using a [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) under the hood. And SEO is on your side. 


Readers can enjoy and share the story without being tied to specific hardware—a Superbook is generally [supported](https://bubblin.io/support) everywhere. Measure metrics down to the very last page of your book, see the world enjoy your work in real time. Transcend geographies because your readers can be anywhere and on any device.


### Environment
The site [https://bubblin.io](https://bubblin.io) is the `production` environment for all your work. It is where your live book will live.

Bubblin comes with a robust pre-built `RESTful` api, a browser-side `development` environment (code playground) and a locally installable client apparatus [Bookiza](http://bookiza.io) (a `nodejs` based `development` environment and CLI tool) to help writers or developers create, test and publish their best work onto web.

Our FREE and opensource templates make it super easy to work with.
