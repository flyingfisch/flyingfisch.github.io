---
layout: post
title: "Styling a Modern Website"
date: 2015-05-18
categories: frontend design
---

Building a "modern" website may seem daunting, especially since the default browser stylesheet is usually pretty ugly. I thought I would share some guidelines that I have come up with since I first started designing sites. Please note that these are things to keep in mind while designing a website, but not necessarily gospel truths.


# Color

One of the first things to remember about color is that subtle is often better. Consider using bright colors only for emphasis, and have your other colors fade into the background to a certain extent. Here is an example of a design that uses bright colors for everything:

<p data-height="268" data-theme-id="6851" data-slug-hash="EjyRWQ" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/EjyRWQ/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

This is obviously a somewhat exaggerated example, but you get the point. Let's try this again, this time with more subtle colors:

<p data-height="268" data-theme-id="6851" data-slug-hash="xGOzLz" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/xGOzLz/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

Although easier on the eyes, the colors in this example do not really match. Let's try using a monochrome palette where every  foreground color is a shade of blue.

<p data-height="268" data-theme-id="6851" data-slug-hash="pJbKPR" data-default-tab="result" data-user="flyingfisch" class='codepen'>See the Pen <a href='http://codepen.io/flyingfisch/pen/pJbKPR/'>example for a blog post</a> by flyingfisch (<a href='http://codepen.io/flyingfisch'>@flyingfisch</a>) on <a href='http://codepen.io'>CodePen</a>.</p>
<script async src="//assets.codepen.io/assets/embed/ei.js"></script>

You don't need to use the same color for your entire site, but these are some ideas to keep in mind when building your site. For more information on color theory, check out this [excellent article](http://www.colormatters.com/color-and-design/basic-color-theory). If you would rather generate your color schemes automatically, take a look at [Paletton](http://paletton.com).

# Whitespace

> Perfection is achieved, not when there is nothing more to add, but when there is nothing left to take away.
>
> <cite>[Antoine de Saint-Exupéry](https://en.wikipedia.org/wiki/Antoine_de_Saint-Exup%C3%A9ry) --
> French aristocrat, writer, poet, and pioneering aviator</cite>

An important part of making an interface look designed is giving it whitespace. Crowded layouts are difficult to navigate, whereas well-spaced layouts are a pleasure to behold. One of the first things I do when designing a website is adding copious line-spacing to the `html` element. This relieves strain on the eyes, making long paragraphs much more readable.

~~~css
html {
    line-spacing: 2.5em;
}
~~~

Another thing I do is add lots of margin and padding between different elements on the page, like headers, footers, and navigation. Here is an example of a crowded design:


