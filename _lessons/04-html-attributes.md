---
title: HTML Attributes
lesson: 4
layout: default
---

Next, let's talk about the `a` (or **anchor**) tag. With this tag, we introduce something called HTML attributes, which are certain traits that a tag can have. HTML attributes go **inside of the opening tag** and always have the syntax of `ATTRIBUTE="VALUE"`, where the value is **always in quotes**. This will make more sense if we look at an example.

The anchor tag is what we use for links. It has an attribute called `href`, or *hyper reference* - the URL of the page that the link goes to. For example, take a look at the following code:

```
<a href="http://easyhtmlcss.com">Click Here</a>
```

What this will render is a link that says "Click Here". If you click the link, you'll be taken to whatever URL is the value of `href` - in this case, the home page of this tutorial!

Now, you can try it. In the last section, you saved an HTML file `my_webpage.html` to your computer. Now, save a new file called `about_me.html` with the following contents: 

```html
<h1>About me</h1>
<p>I'm learning HTML and CSS!</p>
```

Make sure to save `about_me.html` in the **same folder** as where you have `my_webpage.html`. 

Now, let's learn how to link to your new page. In `my_webpage.html`, add a new line somewhere in the file that says: 

```html
<a href="about_me.html">About Me</a>
```

Save it and open `my_webpage.html` in your web browser. Now, if you click the link, it will take you to your new about page. 

**NOTE:** The value of the `href` in this example is `about_me.html`, a **relative path**. Instead of containing the full URL, relative paths are relative to whatever folder you are currently in. In this case, it will look for an about_me.html file in the same folder. So this allows you to link to a different HTML file in the same folder. 

Don't worry if this is still a little confusing. We will go over attributes a little more in the next section, which should make it clearer.
