---
layout: post
title:  "Introduction"
date:   2019-01-01 00:00:06 -0500
categories: documentation introduction
published: true
---

Bubblin is a longform storytelling substrate for writers and book makers. 


<div class="flex">
	<div class="two-third">
		<p>It's a web-based "iPad first" social book reader that comes with a strong pre-integrated developer-like book making toolchain. Additionally, you might want to look at [Bookiza Abelone](https://bookiza.io)—the book *reification* framework for web. Overall, Bubblin and Bookiza are meant for *codex* publishing straight on web. </p>
	</div>
	<div class="one-third flex">
		<a class="right" href="https://bubblin.io"><img src="https://raw.githubusercontent.com/marvindanig/assets/master/bubblin.png" width="100px" /></a>
	</div>

</div>


---

Here's what you can do on Bubblin:

- Publish a well-formatted corpus easily, manage your manuscript separately using `git`. 
- Collaborate with friends, track and update editions on live books. 
- Create short stories, picture books and children's book in an instant with immersive experiences. 
- Reproduce crisp typesetting on web with super close attention to line tracking. Responsively. 
- Create books on open web with razor sharp focus on *accessibility*. 
- Imagine new kind of books with AR/VR, webgl, shaders that's meant for the 
<a rel="nofollow" href="https://en.wikipedia.org/wiki/Post-PC_era">post-pc era</a>. 
- Drive engagement and profit with [transparency](https://bubblin.io/pricing) using the simplicity of web.

The following document explains how Superbooks are made and how they work. Get started with your first book on web!


This documentation is also available in form of a [Superbook](https://bubblin.io/book/official-handbook-by-marvin-danig/1) for your iPad.

### What is a Superbook?

Superbook is a native e-book [format](https://bubblin.io/docs/superbook) for web.

> Superbook means **superclass** of an object like book.

It is an empty container for any kind of longform: books, novels, comics, magazine or anything that needs multi-page storytelling. You can also publish ergonomic greeting cards like this [one](https://bubblin.io/book/i-love-you-by-marvin-danig/1). Superbooks work offline via a modern web browser i.e. like a weblog—meaning, you can collaborate, edit, update, publish and share a live book on web with page level [referential accessibility](https://bubblin.io/blog/referential-accessibility).

### Why Superbooks?

Web is generally bad at longform. Handling a large body of text has not only been traditionally difficult (from the beginning of web/time?) but nigh impossible to enjoy as a reader, as compared to say a physical book. It is no wonder that most people (including developers themselves) prefer buying a physical book even for subjects like CSS or JavaScript where the tech moves faster than print could roll out. Apart from issues of inaccessibility of inner pages (or of content deep down a long scroll) and a scourge of propreitary file formats that are generally incompatible with each other, a loose layout and reflow of text makes it hard for book lovers to enjoy longform online the way they do with a physical book: ala, tight packaging and formatting, and a high quality product. A website or an enterprise-y file (like PDF) could never equal the firm experience of a physical book. It wasn't designed that way.

Enter, Superbooks. :-)

Superbooks introduce tradtional book reading experience on web. It uses some of the very same design principles that make physical books so successful. And goes beyond from there. We revisited every accessibility principle out there by picking up best of both the worlds: physical books and web, and smushed it together to build a robust Superbook container that is both scalable and responsive. For example, primary control of a Superbook is page turn.

Want to learn how it all works? Start with a chapter on the underlying [concept]({{ site.baseurl }}{% post_url 2018-01-01-concept %}).

### Advantages 
Publishing your book directly on web has some automatic advantages. For example, web takes care of the distribution part naturally and at a very low cost. People can enjoy your work without needing to download an artifact to their disk or owning specialized hardware to do that. You can attract readers who don't plan ahead on reading a book as much and gain on impulsive readers. Despite being on web your book is available offline using a [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) under the hood. And SEO is on your side. 

Readers can enjoy and share the story without being tied to specific hardware—a Superbook is generally [supported](https://bubblin.io/support) everywhere. Measure metrics down to the very last page of your book, see the world enjoy your work in real time. Transcend geographies because your readers can be anywhere and on any device.


### Environment
The site [https://bubblin.io](https://bubblin.io) is the `production` environment for all your work. It is where your live book will live.

Bubblin comes with a robust pre-built `RESTful` api, a browser-side `book playground` (a code playground) and a locally installable client apparatus [Bookiza Abelone](http://bookiza.io), which is a `nodejs` based `development` environment and CLI tool to help  you _develop_ your story (book), test it and then publish straight on web.

These tools come with free and opensource [templates](https://github.com/bookiza/templates) that are super easy to work with.
