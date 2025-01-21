---
title: Using Multiple Files
lesson: 20
layout: default
---

Now that our links look so good, it's time to make them functional by learning how to add a new, separate page to our website. But before we do that, we need a way for both pages to use the same CSS. 

Right now, our CSS is inside of our HTML file. But if we created a second HTML file, we'd have to copy and paste our CSS code into that file. Then, if we want to make changes to our CSS, we'd have to change both files. 

There is an easier way. We can move our CSS into a file with a `.css` extension, and use that on both of our HTML pages. Then, when we need to update our CSS, we can simply edit the CSS file and it will update on both webpages. 

### Using A CSS File

In your editor, create a new file named `styles.css`. You can actually name it anything you like, but it needs to end with a `.css` file extension. 

Now, open your HTML file and copy everything in between the `<style type="text/css">` and `</style>` tags. **Do not include the style tags; only copy what is in between them.** Go ahead and paste that into your CSS file, and save it in the **same folder** as your HTML file. 

Next, go ahead and delete the CSS from your HTML file. Delete the entire style tag and everything in it. Now, the `<head>` of your HTML file should be totally empty: 

```
<head>
</head>
```

The `style` tag allowed you to write CSS into your document. A different tag is used to link a CSS file. This is the `link` tag. Not to be confused with links on your page, which use the `a` tag, the `link` tag is used to link your HTML file to an external file. 

To link our CSS file, we need to use two attributes: 

- `rel` defines what the relationship is between the HTML file and the external file. Since our external file is a CSS file, the value for this will be "stylesheet".
- `href` defines the location of the external file. We can write the location **relative to** where the HTML file is. This is called a **relative path** to the file. Since it's in the same folder, we can simply specify "styles.css". 

The link tag always goes inside of the document's `<head>`, since it's not meant to be visible on the page. 

```
<head>
  <link rel="stylesheet" href="styles.css">
</head>
```

Go ahead and load your HTML file in your browser. You'll see that your layout, colors and link effects are still there because it's now loading the CSS from your CSS file!

### Creating a New Page

At last, it's time to learn how to expand your website to multiple pages! Let's create an "About" page, a very common page for websites to have. Go ahead and create a new file named `about.html`. Copy the code from your `index.html` file (or whatever you named the file you've been working in) into this file. We are copying the code because we want to use the same layout, so all of the divs should be the same. 

The general layout will be the same, but we'll change the content. Below, I've changed the text in the title, subtitle, and content of the page: 

```
<!DOCTYPE html>
<html>
  <head>
      <link rel="stylesheet" href="styles.css">
  </head>
  <body>
    <div id="header">
      <h1>About</h1>
      <h2>All About Me and My Website</h2>
    </div>
    <div id="container">
      <div id="sidebar">
         <a href="#">Link One</a>
         <a href="#">Link Two</a>
         <a href="#">Link Three</a>
      </div>
      <div id="content">
        <p>Welcome to the About Page!</p>
      </div>
    </div>
    <div id="footer">
      &copy; 2025 | All Rights Reserved
    </div>
  </body>
</html>
```

You can open `about.html` in your browser to make sure it is working correctly. 

### Linking to the New Page

Open your first HTML file in your editor again, and find the `#sidebar` element that contains your placeholder links. It's time to replace these placeholders with a real link!

Just like the `link` tag that we used for our CSS file above, the `a` tag also works with relative paths. Since the `about.html` is in the same folder, we can simply use "about.html" as the path.

```
<div id="sidebar">
  <a href="about.html">About</a>
</div>
```

Here, I updated the link to go to `about.html`, by specifying it in the `href` attribute. I also updated the text of the link to just say "About". 

Finally, let's edit the About page so that its sidebar has a link back to the home page. Open `about.html` in your editor, and replace the placeholder links like this: 

```
<div id="sidebar">
  <a href="index.html">Home</a>
</div>
```

Here, I changed the link `href` to go back to our `index.html` file. If you named your file something different, be sure to use your actual file name here. I also updated the link text to "Home". 

And.... voila! With multiple pages, this is now a true web*site*, not just a web*page* anymore... and we've reached the end of our project. You can view my finished project example [here](), and download the final files [here](). 
