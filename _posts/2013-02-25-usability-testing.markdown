---
layout: posts
title: Usability Testing
date: February  25, 2013
---

<h2>Usability testing is crucial to making your website easier to use.</h2>
<p>
In this article, I'll explore my reading of <a href="http://www.sensible.com/rsme.html" target="_blank">Rocket Surgery Made Easy</a> by
Steve Krug and how it applied to an application that I recently designed.
</p>

<p>
So what is usability testing?
</p>

<blockquote>
<p>Watching people try to use what your creating, with the intention of (a) making it easier to use or (b) proving that it is easy to use.</p>
</blockquote>

<p>
There are two different types of testing available each with their own implications:
</p>

<div class="row cf">
<div class='column half'>
<h3>Qualitative</h3>
<ul>
  <li>Deals with descriptions</li>
  <li>Do it yourself or with a few people</li>
  <li>Gain insight through context</li>
  <li>Capture emotion</li>
</ul>
</div>

<div class='column half'>
<h3>Quantitative</h3>
<ul>
  <li>Deals with numbers</li>
  <li>Requires larger sample size</li>
  <li>Data/fact driven</li>
  <li>Prove something</li>
</ul>
</div>
</div>

<p>
I'm more interested in gaining insight through qualitative research so I can actually apply my learnings rather than rely on pure, emotionless statistics. The whole idea behind <a href="http://www.sensible.com/rsme.html" target="_blank">Rocket Surgery Made Easy</a> is that you can do qualitative testing yourself or with just a few people.
</p>

<h3>ChiScore</h3>

<p>
I recently had the opportunity to work on an application with Brian Pratt and Rylan Dirksen. It's called ChiScore and was built to track teams for the 2013 <a href="http://www.chiditarod.org/" target="_blank">Chiditarod</a>:
</p>

<blockquote>
<p>Chiditarod (think <a href="http://en.wikipedia.org/wiki/Iditarod_Trail_Sled_Dog_Race" target="_blank">Iditarod</a>) is Chicago's Epic Urban Iditarod. A charity food drive, beauty pageant, costumed shopping cart race, talent show, fundraiser and chaos generator all in one. And probably the world's largest mobile food drive, benefitting the <a href="http://www.chicagosfoodbank.org/site/PageServer" target="_blank">Greater Chicago Food Depository</a>.</p>
</blockquote>

<p>
My role in this project was to design and implement the front end interface. I decided to challenge myself by making the application responsive too!
</p>

<p>
Brian wanted ChiScore to be clean and simple, but trusted me with the details. I started with some layout sketches then did almost all of my designing in-browser. I rarely do traditional mockups in Photoshop or Illustrator these days, and I believe that we've entered the <a href="http://bradfrostweb.com/blog/post/the-post-psd-era/" target="_blank">The Post-PSD Era</a>.
</p>

<p>
The final design was simple and clean, just like we wanted:
</p>

<img src="/images/checkin3-desktop.jpg" alt="Desktop Checkin" />

<p>
With the design ready to go, we had to demo the app for the Chiditerod volunteers and organizers. I didn't realize it at the time, but I was about to get my first opportunity to do some qualitative usability testing.
</p>

<h3>(Unwitting) Test Participants</h3>
<p>
We finally had a working prototype (with responsive elements) and it was time to show off the app to the Chiditarod team for feedback. This was such a rewarding experience.
</p>

<p>
Brian presented to over 40 volunteers and organizers. I went around the room and helped the volunteers load up ChiScore and realized that I just gained a room full of vocal test participants!
</p>

<blockquote>
<p>In usability testing, we call the people we're observing "test participants," not "test subjects," to remind ourselves that we really aren't testing them &mdash; we're testing the thing they're using.</p>
</blockquote>

<p>
I walked around observing volunteers using ChiScore on their phones, tablets and laptops. Sometimes I just watched, other times I took notes and asked for feedback.
</p>

<p>
I gathered some useful insights:
</p>

<ul>
<li>Volunteers were impressed by the speed and the "clean new look"</li>
<li>Everyone was really excited that they could use ChiScore on their phone</li>
<li>Long team names were breaking to another line, wasting precious space</li>
<li>Test participants were confused whether the "X" button deleted or checked out teams</li>
<li>Comments were made regarding the extra white space, font and button sizes</li>
</ul>

<h3>Fixing the Problems</h3>

<p>
When it came time to implement these changes, I turned to my reading to help me:
</p>

<blockquote>
<p>When you're trying to fix a usability problem, the question you should always be asking is: What's the smallest, simplest change we can make that's likely to keep people from having the problem we observed?</p>
</blockquote>

<p>
I gained so much insight from watching the volunteers use ChiScore. It's one thing to design a feature and test it yourself, but to have a whole group of
people test it is invaluable. Having another set of eyes catches things that you might have missed.
</p>

<h3>The Final Design</h3>
<p>
I came up with a few simple solutions and I'm really happy with the results! Here is the final design incorporating all my notes and feedback from the meeting:
</p>

<img src="/images/checkin-limit-desktop.jpg" alt="Checkin Limit Desktop">

<p>
When the team names get too long, I hide them using some css:
</p>

<script src="https://gist.github.com/aekaplan/67c25d2358791c079013.js"> </script>

<p>
For the mobile layout, I completely redesigned the Check Out button by changing the language back to "Check Out" from the icon "X".
</p>

<div class="row cf">
  <div class='column half'>
    <img src="/images/checkin2-mobile.jpg" alt="Mobile Checkin" />
  </div>

  <div class="column half">
    <img src="/images/checkin3-mobile.jpg" alt="Mobile Checkin" />
  </div>
</div>

<p>
The Check Out link also becomes a button making it easier to see and tap. To allow for more information on the screen, I decreased the font size and tightened the overall white space.
</p>

<h2>You have no excuse not to test your websites. Qualitative usability testing is really quite simple!</h2>
<p>
Just ask a friend, family member or coworker. You will be surprised what another set of eyes finds. The insight is invaluable and will almost always make your website easier to use.
</p>

<div class="note">
<p>This article uses my own handcrafted framework for easily making columns responsive.</p>
</div>
