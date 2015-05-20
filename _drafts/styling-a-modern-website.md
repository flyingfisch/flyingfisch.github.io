---
layout: post
title: "Styling a Modern Website"
date: 2015-05-18
categories: frontend design
---

These are some guidelines I have developed from my experience in designing websites. I hope they can help 

# Color

The human eye perceives color quite well. Often just a slight change in shade is all that is necessary to make an element stand out, and a large change in color will make a design look gaudy. I think the best way to ensure that your colors don't clash is to use a color theme generator like [Paletton](http://paletton.com) until you develop a feel for choosing colors on your own.


# Whitespace

An important part of making an interface look designed is giving it whitespace. Crowded layouts are difficult to navigate, whereas well-spaced layouts are a pleasure to behold. One of the first things I do when designing a website is adding copious line-height to the `html` element. This relieves strain on the eyes, making long paragraphs much more readable.

~~~css
html {
    line-height: 2em;
}
~~~

Another thing I do is add lots of margin and padding between different elements on the page, like headers, footers, and navigation. Here is an example of a crowded design:

<p data-height="268" data-theme-id="6851" data-slug-hash="zGBMqy" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/zGBMqy/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

Here is the result with `line-height` set to 2em and margin added between the `aside` and `header`:

<p data-height="426" data-theme-id="6851" data-slug-hash="EjyMwz" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/EjyMwz/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>


# Remember the itty-bitty things

Often, the difference between an award-winning design and an amateur site lies in the details. Take for instance, the following info box:

<p data-height="400" data-theme-id="6851" data-slug-hash="MweMLL" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/MweMLL/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

I have some very basic colors, harsh contrast, and a lot of gray. Here are some examples using the same markup but with attention paid to the 'small things':

<p data-height="400" data-theme-id="6851" data-slug-hash="GJqVgO" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/GJqVgO/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

The first alternative has a subtle `box-shadow` around it, `text-transform: uppercase` is set on the header, and a 2 pixel border is added underneath to distinguish it from the text below.

The second one shoots for a flatter look, with a 10 pixel border instead of `box-shadow` around the whole thing, a light blue background, and a border is added again below the header.

The third example accentuates the typography by removing almost all other visual elements. There is a 10 pixel border on the top which shows where the info box starts, and also subtly shows where the sides are as well. The header has `font-variant: small-caps` applied to it, which is a property I recently discovered and have been having fun playing with lately.


# Less is More

> Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away.
>
> <cite>[Antoine de Saint-Exupéry](https://en.wikipedia.org/wiki/Antoine_de_Saint-Exup%C3%A9ry) --
> French aristocrat, writer, poet, and pioneering aviator</cite>


