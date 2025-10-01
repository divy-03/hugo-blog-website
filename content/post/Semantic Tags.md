---
title: Semantic Tags
description: HTML tags

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - interview
  - html
categories:
  - prep
---

Semantic HTML tags are **meaningful tags** that describe the purpose of the content inside them — both to the **browser** and to **developers** (and also screen readers for accessibility).

```html
<header> for top section (logo, nav, intro)
<nav> for nav menu with nav-links
<main> for main content of the doc
<section> sections of content 
<article> for blog post, news article
<aside> sidebar content, i.e. not related to main content
<footer> bottom section with links and copyright license
<figure> to wrap media images, diagrams, charts with captions
<figcaption> caption for figure
<mark> highlight text with yellow
<time> represent datetime="" attribute for machine readability  
```

also a new semantic tag added <address /> which is used to wrap personal social media address like email, linkedin, etc and **NOT** the actual postal address.

```html
<address>
You can contact us directly at <a mailto="contact@html.com">contact@html.com</a>.
</address>
```
