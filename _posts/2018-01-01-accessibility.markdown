---
layout: post
title:  "Accessibility"
date:   2018-01-01 00:00:00 -0500
categories: documentation introduction
published: true
---

Accessibility is critical for readers with different needs.

In general, an empty Superbook container meets nearly all acessibility guidelines per WCAG 2.1 (2018), but there are still some gaps a few challenges of the longform that a reader must overcome to enjoy your book to the very end. To help readers flow through your work without interruptions or hurdles make sure that you follow the below given accessibility guidelines: 

1. Never use hard values for text size such as `16px` or `24pt`. Use only viewport units like `4vw` to make sure the body of text scales accurately covering maximum readership between mobile phones and television sets. In general, a tablet like iPad with a large surface area is ideal for book reading but it is recommended to support smaller underpowered devices as far deep as possible. Done right, a Superbook can be displayed correctly on an Apple Watch as well.

2. Do not hardcode page numbers in the contents of your book. Use `has_page_numbers: true` on `.bookrc` instead to display page numbers upon publshing. Page numbers can also be enabled via the online [editor console](https://bubblin.io/book/official-handbook-by-marvin-danig/31) on Bubblin.    