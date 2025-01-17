---
title: Adding CSS to the Page
lesson: 9
layout: default
---

Now you might be wondering... where does the `style` tag go in an HTML page? The answer? It goes inside the `head` section. Here's an example of what your entire page might look like now: 

```html
<!DOCTYPE html>
<html>
  <head>
    <style type="text/css">
    strong {
      color: #eeeeee;
      background-color: #000000;
    }
    </style>
  </head>
  <body>
    beautiful <strong>constellations</strong>
  </body>
</html>
```

Now you should have a basic idea of what CSS is, how to use it, and what you can do with it. Just like we styled the strong tag, we can also style other HTML tags, like `p`, `h1`, `em`, and more. In the remainder of this tutorial, you'll see some other CSS attributes as well.

<div class="try-it">

<ol>
  <li>Copy the above code into a new <code class="language-plaintext highlighter-rouge">.html</code> file and open it in your web browser.</li>
  <li>Use an online color picker (search for “hexadecimal color picker online”) to find more color codes, and try changing the color and background color of the text.</li>
  <li>Try adding a header (<code class="language-plaintext highlighter-rouge">&lt;h1&gt;</code> tag) and try changing the color and background color of this with CSS as well. (Hint: the code we have changes the <code class="language-plaintext highlighter-rouge">strong</code> tag, so your code will look very similar to that, but with <code class="language-plaintext highlighter-rouge">h1</code> instead of <code class="language-plaintext highlighter-rouge">strong</code>.)</li>
</ol>

</div>
