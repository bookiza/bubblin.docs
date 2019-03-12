---
layout: post
title:  "Accessibility"
date:   2019-01-01 00:00:00 -0500
categories: documentation introduction
published: true
---

Accessibility is critical for the success of your book.

In general, your work should be available to all readers no matter what their device, situation or abilities are.

An empty Superbook container meets *nearly* all acessibility guidelines per WCAG 2.1 (2018), but there are still some areas where the challenges of the longform creep up. Prevent a reader from completing your book. 

To help readers glide through your work without interruption, make sure that you follow the below given accessibility guidelines: 

1. Never hardcode values for text size such as using `16px` or `24pt` on your book. Use only viewport units like `4vw` to make sure the body of text scales accurately across all devices thus covering maximum readership potential between mobile phones and television sets. Done right, a Superbook can be displayed correctly on an Apple Watch as well.

2. Use JavaScript sparingly. While a tablet like iPad with a powerful processor and a large surface is ideal for immersive book reading there are billions of smaller underpowered devices to support. Keep fancy to minimum. 


3. Do not hardcode page numbers within the contents of your book. Use `has_page_numbers: true` on `.bookrc` instead to display page numbers on publshing. Page numbers can also be enabled via the online [editor console](https://bubblin.io/docs/numbering.html) on Bubblin.