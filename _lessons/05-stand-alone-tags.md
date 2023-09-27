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

What will the code above look like? Try it yourself! 

1. Open your `my_webpage.html` file from before.
2. Add the `img` code above somewhere in the file, and save it.
3. Open the file in your web browser (or refresh the page if you already have it open), and voila!

Now, try saving the image to your computer and loading it from your computer instead: 

1. Right-click the image and save it as `html_logo.png`. Save it in **the same folder** as your `my_webpage.html` file. 
2. Change your `img` tag to the following: `<img width="100" height="100" src="html_logo.png">`
3. Now refresh the page in your web browser and the image should still show up! Except now it's using the image file on your computer. 

Now you know how to save images from the internet to put them in your website. 
