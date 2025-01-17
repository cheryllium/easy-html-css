---
title: Stand-alone Tags
lesson: 5
layout: default
---

Remember how I said there are two types of HTML tags? One of the types is the opening and closing tags. That makes sense for things like emphasizing text, because it encloses the text that you want to be affected. Some things, though, like images, just stand by themselves and don't need to enclose anything. These are made using **stand-alone tags**. Take a look at the `br` tag as an example:

```html
<br>
```

Pretty simple, right? It's just like the opening tags we already learned about, but without a closing tag. By the way, what the `br` tag does is make a line break. It's the same as pressing enter on your keyboard once.

The `br` tag is super simple - that's all there is to it. A more interesting stand-alone tag we can learn about is `img`, the image tag. This has the important attribute `src`, which should have the URL of the image as its value. It can also have `width` and `height` attributes, which are specified in pixels, to tell you how big the image should be. For example, consider the following code:

```
<img width="100" height="100" src="https://easyhtmlcss.com/assets/html_logo.png">
```

This is an example of how to use a tag with multiple attributes, in this case, the width, height, and image source. As you can see, it's quite simple - each attribute is in the form of `ATTRIBUTE="VALUE"`, just as we learned in the last section, with spaces to separate them.

What will the code above look like? It's time to...

<div class="try-it">

<ol>
  <li>Open your <code class="language-plaintext highlighter-rouge">my_webpage.html</code> file from before.</li>
  <li>Add the <code class="language-plaintext highlighter-rouge">img</code> code above somewhere in the file, and save it.</li>
  <li>Open the file in your web browser (or refresh the page if you already have it open), and voila!</li>
</ol>

<p>Now, try saving the image to your computer and loading it from your computer instead:</p>

<ol>
  <li>Right-click the image and save it as <code class="language-plaintext highlighter-rouge">html_logo.png</code>. Save it in <strong>the same folder</strong> as your <code class="language-plaintext highlighter-rouge">my_webpage.html</code> file.</li>
  <li>Change your <code class="language-plaintext highlighter-rouge">img</code> tag to the following: <code class="language-plaintext highlighter-rouge">&lt;img width="100" height="100" src="html_logo.png"&gt;</code></li>
  <li>Now refresh the page in your web browser and the image should still show up! Except now it’s using the image file on your computer.</li>
</ol>

</div>

Now you know how to save images from the internet to put them in your website!
