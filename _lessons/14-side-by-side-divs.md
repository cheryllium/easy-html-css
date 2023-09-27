---
title: Side by Side Divs
lesson: 14
layout: default
---

There is just one last thing before we conclude our basic HTML and CSS tutorial. So far, the header, content, and footer of our page are all on top of each other. But what if we want to have two things side by side? For example, what if we wanted to add a sidebar, next to the content, that is beside it? 

The strategy we'll do is this: 

1. Put the sidebar and content inside a new div. 
2. Set some CSS on this new div to tell it, "put the things inside you side-by-side instead of stacked vertically"

So let's look at how to do this. First, we'll put the sidebar and content in their own div, which I'll give an ID of "main" to in order to be able to select it: 

```
<body>
  <div id="header">
    <h1>Welcome to my Webpage!</h1>
  </div>
  <div id="main">
    <div id="sidebar">
      <p>Some links could go here.</p>
    </div>
    <div id="content">
      <p>I'm learning HTML and CSS!</p>
    </div>
  </div>
  <div class="footer">
    <p>Website made with love.</p>
  </div>
</body>
```

Now, we need to put some CSS code on the `main` div that says, "put everything inside of you side-by-side". This is the code that will do this: 

```
#main {
  display: flex;
}
```

In short, this enables something called "flexbox" on the div, which is a modern way to arrange layouts in CSS. By default, something with `display: flex` will display everything in it side-by-side. 

Since this is a basic tutorial, we won't delve any further into flexbox. I just wanted to give you this piece of code so that you have a way of arranging divs side-by-side in your pages for now. If you would like to learn more about flexbox, I recommend checking out the awesome interactive tutorial [Flexbox Froggy](https://flexboxfroggy.com/). 
