---
title: Structure of an HTML Page
lesson: 6
layout: default
---

Now that you know a bit of basic HTML, let's talk about the structure of an HTML page. While you can write any HTML into a file and run it, web pages have a particular HTML structure that can be followed. Following this structure will ensure your web page runs correctly even as it gets more complicated. 

First, all HTML documents have to start with a special line that declares that the document type is HTML. This line looks a bit like a tag, but it's actually not an HTML tag, it's a "declaration". It tells the web browser what type of document it is, in this case, HTML. 

```html
<!DOCTYPE html>
```

Whenever you make an HTML file, be sure to write this as the very first line. 

Next, the entire document is enclosed within `html` tags, which acts as a container for everything else. Within this, our HTML page is split into two parts, which are also opening and closing tags: a `head` and a `body`. 

```html
<!DOCTYPE html>
<html>
  <head>
  </head>
  <body>
  </body>
</html>
```

Inside the `head`, we place information about the page which isn't directly visible on the page. One such tag is the `title` tag, which controls the text displayed in the top of the browser tab. 

Inside the `body` is where our actual visible HTML elements go. This is where we can write paragraphs of text, titles with the `h1` tag, and more. 

So for example, a simple page could look like this: 

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My Website</title>
  </head>
  <body>
    <h1>Welcome to my web site!</h1>
    <p>Thanks for visiting today!</p>
  </body>
</html>
```

<div class="try-it">
<p>Try copying this into a new file with a <code class="language-plaintext highlighter-rouge">.html</code> extension, and open it in your browser to see what it says. You’ll notice that it says “My Website” in the browser tab, which is the result of the <code class="language-plaintext highlighter-rouge">title</code> tag. Then, on the actual page, you’ll see what’s in the <code class="language-plaintext highlighter-rouge">body</code>.</p>
</div>

Congratulations on sticking with me this far! You now know enough basic HTML to move on to the next section: basic CSS. 
