---
layout: posts
title: Write Better CSS
date: March 28, 2013
---
<h2>Writing better CSS can be easy. Remember to normalize, organize and alphabetize!</h2>

<p>
I'm going to be giving a short presentation titled "Write Better CSS" at Apprentice Learning Hour but wanted to start collecting my thoughts here first. Spoilers ahead!
</p>

<p>
Steps to writing better CSS (I couldn't help myself with the naming):
</p>

<ul>
  <li>Normalize</li>
  <li>Organize</li>
  <li>Alphabetize</li>
  <li>DRY and write reusable CSS</li>
</ul>

<h3>Normalize</h3>
<p>
Resets remove the default styles for all elements while <a href="http://necolas.github.com/normalize.css/" target="_blank">normalize</a> retains most of the useful default browser styles. When starting a new project, I prefer normalize over resets.
</p>

<blockquote>
<p>Normalize.css is a small CSS file that provides better cross-browser consistency in the default styling of HTML elements. It’s a modern, HTML5-ready, alternative to the traditional CSS reset.</p>
</blockquote>

<p>
It also corrects bugs commonly found in browser inconsistencies and doesn't clutter your debugging tool. Simply download and use <a href="http://necolas.github.com/normalize.css/" target="_blank">normalize.css</a> as-is, or customize it to meet your requirements.
</p>

<h3>Organize</h3>
<p>
Organize your CSS code to reflect the flow of your website's layout. For example, your navigation CSS should be at the top of your file and your footer should be closer to the bottom:
</p>

<script src="https://gist.github.com/aekaplan/4f1cad35c6c791542c10.js"> </script>

<p>
Put properties related to one another close together and <em>use comments sparingly</em> to break up the different sections of your CSS. The combination of a few comments and grouping similar elements together will make it much easier to quickly find what your looking for.
</p>

<h3>Alphabetize Your Properties</h3>
<p>
Write your CSS properties in alphabetical order; it will help reduce the time it takes to find a specific property.
</p>

<p>
Jen Myers' post on <a href="http://jenmyers.tumblr.com/post/45339751868/why-you-should-order-css-properties-alphabetically" target="_blank">Why you should order CSS properties alphabetically</a> made me a believer:
</p>

<blockquote>
<p>Here’s the simple truth up-front: alphabetical CSS ordering makes your CSS most easily accessible to the widest group of people with the least amount of clutter in your stylesheets.</p>
</blockquote>

<p>
This principle is fairly new to me, but has really helped make my code more navigable. Which example makes it easier to find specific properties:
</p>

<script src="https://gist.github.com/aekaplan/8f0f05409107f339cafb.js"> </script>

<p>
The second CSS block is easter to skim through, right? I know the z-index will always be at the bottom of the block. Don't worry about alphabetizing vendor prefixes (like box-sizing or transition, for example) with the rest of your properties, as you will want to keep those grouped together.
</p>

<h3>Don't Repeat Yourself and Write Reusable CSS</h3>
<p>
<a href="http://en.wikipedia.org/wiki/Don't_repeat_yourself" target="_blank">DRY</a> up your code! Repeating yourself leads to huge CSS files and unnecessary code bloat. Take the time to plan out your elements in a simple and reusable way. Reuse your classes and tag on additional classes when needed.
</p>

<p>
Here's some really repetitive code:
</p>

<script src="https://gist.github.com/aekaplan/4cf7c42030c0885770d8.js"> </script>
<script src="https://gist.github.com/aekaplan/1cd17e1728522e397c33.js"> </script>

<p>
Lets DRY this up and make it a bit more reusable:
</p>

<script src="https://gist.github.com/aekaplan/1de0549cc4ee559823d9.js"> </script>
<script src="https://gist.github.com/aekaplan/c068be2d748c8c9f03c1.js"> </script>

<h3>Be Consistent and Thoughtful... and Clean up Your Code!</h3>
<p>
These simple steps will make your CSS more organized, lightweight and easier to read. This will only benefit you and anyone else who needs to make changes to your code.
</p>

<div class="note">
<p>
My "Write Better CSS" presentation will be on April 12.
</p>
</div>
