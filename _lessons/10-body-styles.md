---
title: Body Styles
lesson: 10
layout: default
---

So far, we've seen two CSS **properties**: `color`, which changes the color of your text, and `background-color`, which changes the background color of whichever **element** is selected. Now... what if you want to change the font color and background color of the entire page? 

As we learned in the "Structure of an HTML Page" section, everything visible on your page is contained within a `body` tag. So if we want to change something about the entire page, we can select `body`! 

```html
body {
  background-color: #eeeeee; 
  color: #ff0000; // red
}
```

The code above will change the background color of the page to #eee, a light gray, and change the font color to #f00, red. The syntax `// red` is called a **comment** - if you write two slashes `//` at the end of a line, anything you write after them will be ignored. You can use this to leave notes to yourself, for example, about what color your hex code is. 

<div class="try-it">
<p>Try it! Open up your <code class="language-plaintext highlighter-rouge">my_webpage.html</code> and add the CSS above in between your <code class="language-plaintext highlighter-rouge">style</code> tags. What do you see?</p>
</div>
