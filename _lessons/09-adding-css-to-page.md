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

**Try it!** 

1. Copy the above code into a new `.html` file and open it in your web browser. 
2. Use an online color picker (search for "hexadecimal color picker online") to find more color codes, and try changing the color and background color of the text. 
3. Try adding a header (`<h1>` tag) and try changing the color and background color of this with CSS as well. (Hint: the code we have changes the `strong` tag, so your code will look very similar to that, but with `h1` instead of `strong`.)
