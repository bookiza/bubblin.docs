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
		<p>It is a social book reader that is both offline first (a PWA) and <em>tablet first</em>, i.e. designed with iPad users on mind. Bubblin comes with a REST api and a pre-integrated client to form a strong <em>developer like</em> book-making toolchain called the <a href="https://bookiza.io">Bookiza Abelone</a>. </p>
	</div>
	<div class="one-third flex">
		<a class="right" href="https://bubblin.io"><img src="https://raw.githubusercontent.com/marvindanig/assets/master/bubblin.png" width="100px" /></a>
	</div>

</div>


---

Here's what you can do on Bubblin:

- Publish a well-formatted corpus easily, manage editions and collaborate using `git-scm`. 
- Introduce line-tracking, widows and orphan handling on live responsive books over the web browser. 
- Create short stories, picture books, childrens' books with immersive animations. 
- Produce books with elegant typography using design principles of web.
- Paginate cross-browser cross-device and cross-OS books with page level [referential-ability](https://bubblin.io/blog/referential-accessibility). 
- Concoct new generation of books with AR/VR, webgl, shaders that's ideally meant for the 
<a rel="nofollow" href="https://en.wikipedia.org/wiki/Post-PC_era">post-pc era</a>. 
- Drive engagement and profit with [transparency](https://bubblin.io/pricing) using the simplicity of web.

The following document explains how Superbooks are made and how they work. Get started with your first book on the web!


This documentation is also available in form of a [Superbook](https://bubblin.io/book/official-handbook-by-marvin-danig/1) for your iPad.

### What is a Superbook?

Superbook is the _native_ book [format](https://bubblin.io/docs/superbook) for the web.

> Superbook means **superclass** of an object like book.

It is an empty container for any kind of longform: books, novels, comics, magazine or anything that needs multi-page storytelling. You can also publish ergonomic greeting cards like this [one](https://bubblin.io/book/i-love-you-by-marvin-danig/1) if you want. Superbooks are ordinary websites that work offline via a modern web browser using a serviceworker, i.e. a standard PWA—and this means that you can take advantage of open web on your books, collaborate, edit, update, publish, share and republish a live book any number of times.

In fact readers can talk about your book on each page of the story separately!

### Why Superbooks?

Web has been generally bad at longform. Handling a large corpus of text has not only been traditionally difficult (from the beginning of web/time?) but nigh impossible to relax with and enjoy as a reader. As compared to say a physical book, a digital file leaves a lot to ask for and frankly books are not files to begin with! It is no wonder that most people including the developers themselves prefer buying a physical copy even for subjects like CSS, or Rust or JavaScript where tech moves faster than print could ever be rolled out. 

Apart from issues of inaccessibility of the inner pages of book (or of content deep down on a long infinite scroll), the scourge of propreitary file formats that are generally incompatible with each other along with a loose reflowable layout makes it hard — nearly impossible — for even the most ardent book fans to be on the same page. 

With Superbooks people can finally enjoy longform online the way they do with a physical book. It brings tight scalable and responsive formatting using [strong layouts](https://bubblin.io/docs/layouts) and a high quality finish that sports even [page-level referenceability](https://bubblin.io/blog/referential-accessibility). Unlike an enterprise-y file (like PDF or Epub) that people are forced to download a Superbooks is simply a website with the native experience of books. Superbook format is a live specification. All feedback and inputs are welcomed on [forum](https://news.bubblin.io) to make it as robust and accessisble as possible. 

Wish to learn how it all works? Start with a chapter on the underlying [concept]({{ site.baseurl }}{% post_url 2018-01-01-concept %}).

### Advantages 

Publishing your book directly on web has some direct advantages. 

- The distribution part comes to the mind first. Naturally, web is the most efficient machine for distribution for near zero cost. People can enjoy your work anywhere in the world without needing to download an artifact to the disk. Without need to own specialized and often propreitary hardware to be able to do that. 

- Attract impulsive readers who do not plan on reading a book ahead through social media. What's notable here is that your book is going to be available offline too using a [Service Worker](https://developer.mozilla.org/en-US/docs/Web/API/Service_Worker_API) to such readers. 

- Natural SEO. With the entire content online it is easier for people to be able to find your book via a search engine. 

- Frictionless. Readers can read and share the story on the device they are on without need special hardware or separate apps—a Superbook is generally [supported](https://bubblin.io/support) on all devices and browsers between an Apple Watch and an OLED TV. 

- Transparent metrics down to the very last page on your book. See how the world is enjoying your work in real time. 

- There are other advantages of publishing on Bubbblin—like you get to own 100% rights and the process is secured with industry-grade encryption and you get to engage with a very vibrant community of book lovers on the web.


### Terminology and important links:

The website [https://bubblin.io](https://bubblin.io) and our wrapper [app](https://play.google.com/store/apps/details?id=free.books.bubblin) on Google Playstore are the `production` environment for all your works. It is the place where your final and latest edition of the book will live. Bubblin comes with a tiny but robust RESTful `api`, a browser-side book editor (a code playground) and an npm package (CLI tool) that can be installed locally to produce books. 

Here are some of the important links:

1. [Bookiza Abelone](http://bookiza.io)—a book baking tool (CLI) in nodejs and its [documentation](https://bubblin.io/bookiza/docs/).
2. [H2S](https://github.com/bookiza/h2s)—an automatic paginator & HTML2Superbook convertor.
3. [Gutendown](https://github.com/bookiza/gutendown)— a free resource with all Gutenberg titles in markdown format. 
4. A [demo book](https://bubblin.io/cover/bookiza-documentation-by-marvin-danig#frontmatter) that doubles as documentation for Bookiza.
5. And a [contact us](https://bubblin.io/blog/contact/) page.

Along with the tools here are some [strong layout templates](https://github.com/bookiza/templates) that are super easy to configure and reuse on any type of book.
