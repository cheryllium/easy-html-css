---
title: A Smattering of Tags
lesson: 3
layout: default
---

Tags get more fun once you have a couple to play with. Here are some basic tags that you should know about as a novice HTML coder. Remember that these are all opening and closing tags - they affect the text that they enclose. We'll talk about the second type of tag soon.

- `em` - This stands for **emphasis** and is used when you want to emphasize text. By default, this will render as italic.
- `strong` - This is used for text that is **strongly important**. By default, this renders as bold.
- `h1` - This stands for **header 1** and is the largest type of header, or page title. There are also tags `h2` through `h6`. They get progressively smaller, and are used for subheaders or subtitles. By default, this will render as bold, large text on its own line.
- `p` - This stands for **paragraph** and should be used to enclose paragraphs of text. By default, this will have the effect of pressing enter on your keyboard twice before the paragraph.
- `ol` and `ul` - These are **ordered list** and **unordered lists**, in other words: **numbered lists** and **bulleted lists**. Inside the list, each item should be within an `li` (**list item**) tag. 
- `div` - This stands for **division**, in other words, a **section** of the page. This is a versatile tag used to organize more complex HTML into sections. We will use this one more in the CSS section.

For example, check out the following code. Can you guess what it will look like?

```html
<h1>Page Title</h1>

<p>Lorem ipsum <strong>dolor</strong> sit <em>amet</em></p>

<ol>
  <li>Item number one</li>
  <li>Item number two</li>
  <li>Item number three</li>
</ol>
```

You can run this code yourself to find out: 

1. Create a file named `my_webpage.html`. You can actually name it anything you want, but make sure it ends in `.html`!
2. Copy the above example into the file, and save the file.
3. Open the file in a web browser to see your HTML in action!

Once you have this file, you can make changes to it and then refresh the page in your browser to see your changes. Try it: 

1. Add `<h2>Page Subtitle</h2>` on a new line after the `h1` code. 
2. Save the file. 
3. Refresh the page in your web browser to see what your new line of code does!

*A quick note on editing HTML files:* The best way to edit HTML files is with a **text editor** such as [Notepad++](https://notepad-plus-plus.org/) (if on Windows) or [Sublime Text](https://www.sublimetext.com/). You have to use a text editor instead of something like Microsoft Word, because an HTML file is just text, without special formatting. You can use a simple program like Notepad, but I recommend something with more features such as the ability to display different parts of your code in different colors to help you read it (called *syntax highlighting*).
