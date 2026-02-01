---
title: HTML
description: My HTML notes for interview

date: 2025-09-14T20:12:52+08:00
lastmod: 2025-09-14T20:12:52+08:00
tags:
  - blog
  - html
  - interview
  - notes
categories:
  - prep
---



Hyper Text Markup Language is the backbone of any website. 

- Avoid using more than 1 <h1 />  as it is the biggest heading, only one h1 should be present in one sheet.
- Always use headings in order, first h1 then h2 and so on.
- Always use img tag inside a figure tag when images have caption
 ``` html
<figure>
	<img src="" />
	<figcaption>Caption</figcaption>
</figure>
```
-  Use [[post/Semantic Tags]] like header, footer, section, article
- Avoid using <b/>, <i/> for bold and italics, instead use [[CSS]] properties like font-weight and font-style: "italic" or use <strong/> for bold and <em/> for emphasis/italics.
- Don't use [block](#block-and-inline-element) elements inside [inline](#block-and-inline-element) elements
### Block and Inline element

> Block elements always start on a new line and take up the **full width** available.

`<div>`, `<p>`, `<h1>`–`<h6>`, `<section>`, `<article>`, `<header>`, `<footer>`, `<ul>`, `<ol>`, `<li>` `<form>`, `<table>`

> Inline elemets do **not start on a new line**. Only take up as much width as their content.

`<span>`, `<a>`, `<strong>`, `<em>`, `<img>`, `<label>`, `<input>`, `<button>`

  Special Case: Inline-Block
  - **Inline-block** behaves like inline (stays in line) **but** allows you to set width/height like a block element.

Usage of blockquote with accessibility, abbreviation with tooltips, subscript & superscript, and time tag for machine readable date time. 

```html
<h1>Advanced text semantics</h1>
<p>Let's start with a quote:</p>

<blockquote cite="https://developer.mozilla.org/en-US/docs/Learn/Accessibility">
  <p>
    <abbr title="HyperText Markup Language">HTML</abbr>, Hypertext Markup
    Language is by default accessible, if used correctly.
  </p>
</blockquote>

<p>
  <abbr title="Cascading Style Sheets">CSS</abbr>, Cascading Style Sheets, can
  also be used to make web pages more, or less, accessible.
</p>

<p>
  Chemical Formulae: H<sub>2</sub>O (Water), C<sub>2</sub>H<sub>6</sub>O
  (Ethanol).
</p>

<p>
  Dates:
  <time datetime="2019-12-25">December 25<sup>th</sup> 2019</time>
  (Christmas Day),
  <time datetime="2019-11-02">November 2<sup>nd</sup> 2019</time> (Día de los
  Muertos).
</p>
```

### Image Map

```html
<img src="workplace.jpg" alt="Workplace" usemap="#workmap" width="400" height="379">  
  
<map name="workmap">  
  <area shape="rect" coords="34,44,270,350" alt="Computer" href="computer.htm">  
  <area shape="rect" coords="290,172,333,250" alt="Phone" href="phone.htm">  
  <area shape="circle" coords="337,300,44" alt="Cup of coffee" href="coffee.htm">  
</map>
```

### Base Url 

```html
<head>  
  <base href="https://www.w3schools.com/" target="_blank">  
</head>  
  
<body>  
<img src="images/stickman.gif" width="24" height="39" alt="Stickman">  
<a href="tags/tag_base.asp">HTML base Tag</a>  
</body>
```





TODO: 
- [ ] Revise all html tags from w3
- [ ] Understand the html boilerplate
- [ ] Revise the notes
- [ ] Practice through projects
- [ ] Watch interview videos