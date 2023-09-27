---
title: Classes and IDs
lesson: 12
layout: default
---

Next, let's say you want your page to have three distinct sections: the header, the content, and the footer. And you want each of these to look a little differently, using CSS. It's time to talk about CSS classes and IDs. 

A CSS ID is just another way to specify that something needs to be styled. We use an ID on something when there is only one of it on the entire webpage. For example, there is usually only one header and footer on a webpage, so these commonly are styled using IDs. To give something an ID, we name the ID anything we would like (like "header"), and then use the `id` HTML attribute:

```html
<div id="header">
  <h1>Welcome to my Webpage!</h1>
</div>
```

Then, in the CSS, we can style this. For example, we could give a header a width and a height. To style an ID, it is just like styling a tag, except we put a **hashtag symbol** in front of the ID's name.

```html
<style>
#header {
  width: 100%;
  height: 100px;
}
</style>
```

This code will style everything with `id="header"` (which should only be one thing!) A note about the new attributes here: `width` and `height` can be specified either in pixels (px) or in percentages, in which case it is the percentage of the browser's width or height. (There are a few other options too, but we don't have to worry about them now.)

CSS classes work almost the same way, except you can have **multiple** elements on a page with the same class. You would specify a class using the HTML attribute class. For instance, say we have a class called "red":

```html
<div class="red"></div>
```

We style this just like the id, except we use a **period** instead of a hashtag in front of the name. The following code will give a red background to every element with the attribute class="red".

```
<style>
.red {
  background-color: #ff0000;
}
</style>
```

### Try it Yourself

Try making an HTML page with a header, footer, and content. You might remember that, in the HTML section of the tutorial, we discussed a `div` tag which defines a section of a page. This is the perfect time to use it! The header, footer, and content sections should each be a `div`: 

```
<body>
  <div id="header">
    <h1>Welcome to my Webpage!</h1>
  </div>
  <div id="content">
    <p>I'm learning HTML and CSS!</p>
  </div>
  <div class="footer">
    <p>Website made with love.</p>
  </div>
</body>
```

Take a moment to understand what is happening here: There are three `div` tags, with the IDs of `header`, `content`, and `footer`. We've written a little bit of HTML inside of each `div`. Whatever CSS you write for the `div` will apply to everything that is inside it by default!

Now, try using CSS to give each section a different style. You can give them different background colors, font colors, and fonts. You can even give them different widths and heights. Give it a try!
