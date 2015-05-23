---
layout: post
title: "Building a Minimal Modern Website"
date: 2015-05-18
categories: frontend design
---

I thought of writing a post going over the abstract concepts of building a modern website, but decided to scratch that idea in favor of a step-by-step demo of the way I build websites. In this post I will be going from design to delivery on a nautical themed website for a sailing club. Let's get started!


# Layout

The first thing I do when building a website is come up with a layout. For this site I thought we would keep the layout fairly minimal. I don't generally build wireframes, preferring building in the browser instead, but I whipped one up in this case to let you see what kind of layout I am envisioning.

<figure>
<img src="/assets/nautical-wireframe.svg" alt="Wireframe for desktop layout">
<figcaption>Wireframe for desktop layout.</figcaption>
</figure>

Since this is going to be responsive, we need to have a mobile layout as well.

<figure>
<img src="/assets/nautical-wireframe-mobile.svg" alt="Wireframe for mobile layout">
<figcaption>Wireframe for mobile layout.</figcaption>
</figure>


# Colors

The colors for this site are going to be blue and white. I got the exact shades straight from the [Tango project's color palette](http://tango.freedesktop.org/Tango_Icon_Theme_Guidelines#Color_Palette).

<figure>
<img src="/assets/nautical-palette.svg" alt="Palette colors: #ffffff, #eeeeec, #3465a4, #204a87">
<figcaption>Colors: #ffffff, #eeeeec, #3465a4, #204a87</figcaption>
</figure>

# Designing the Header

The first thing I do when designing in the browser is write the HTML for a simple header. For this project it will look like this:

~~~markup
<header>
    <h1>R. S. Sailing Club</h1>
</header>
~~~

The next thing I usually do is choose a font to use. For this project I just ran over to [Google Fonts](https://www.google.com/fonts/) and chose Montserrat for the headers and Alegreya for the copy. As a rule of thumb it is usually good to choose a serif font for your body text if the headers are sans-serif, and vice versa.

Here is the `link` tag for the fonts, we're just going to add it into the header. Although there are other methods of using Google Fonts, the `link` tag has the best browser support.

~~~markup
<link href="http://fonts.googleapis.com/css?family=Montserrat:400,700|Alegreya:400,400italic,700,700italic" rel="stylesheet" type="text/css">
~~~

We will also be using [Normalize.css](https://necolas.github.io/normalize.css/) which basically gives you a starting point that looks the same across all browsers. Since we want to override it's styles with ours we put it's link tag first. Our `head` tag should look something like this now:

~~~markup
<head>
    <title>R. S. Sailing Club</title>

    <link href="http://fonts.googleapis.com/css?family=Montserrat:400,700|Alegreya:400,400italic,700,700italic" rel="stylesheet" type="text/css">
    <link href="/css/normalize.css" rel="stylesheet" type="text/css">
    <link href="/css/style.css" rel="stylesheet" type="text/css">
</head>
~~~

We're going to be using [SASS](http://sass-lang.com/) for the stylesheets, but don't worry, I'll explain any nuances we come across in the project. For now, just think of it as CSS with extra features. Here is our stylesheet so far:

~~~scss
html, body {
    width: 100%;
    height: 100%;
}

body * {
    box-sizing: border-box;
}

body {
    font-family: 'Alegreya', serif;
    font-size: 16px;
}

h1, h2, h3, h4, h5, h6 {
    font-family: 'Montserrat', sans-serif;
}
~~~

