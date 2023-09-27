---
title: Changing the Font
lesson: 11
layout: default
---

One other thing you might want to change is the font used on the page. The CSS **property** for font is called `font-family`. You can give it the name of a font in quotes, for example: 

```
body {
  font-family: 'Arial';
}
```

And it will use that font if it's on the computer of whoever is visiting your website. You can also give it a type of font (a generic family of fonts):

```
body {
  font-family: sans-serif; 
}
```

And the browser will pick a font in that family. The font families you can choose from are: 

- <span style="font-family:serif">serif</span> - fonts with serifs (the little lines on the ends of letters), such as Times New Roman.
- <span style="font-family:sans-serif">sans-serif</span> - fonts without serifs, such as Arial
- <span style="font-family:cursive">cursive</span> - a "script" font where letters look a bit like handwriting
- <span style="font-family:monospace">monospace</span> - a font where every letter has the same width (great for code!)

Finally, you can give the `font-family` property a list of fonts separated by commas. When you do this, it will try every font down the list. If the browser doesn't have the first font, then it will move to the next one. For example: 

```
body {
  font-family: 'Courier New', monospace;
}
```

What this does is tell the browser to first look for the Courier New font. But if your website visitor's computer doesn't have the Courier New font, then it moves on to the next font family in the list, "monospace" - and simply picks a monospace font. 

**Helpful Tip** This list of fonts is called a **font stack**. The website [Modern Font Stacks](https://modernfontstacks.com/) has a whole bunch of good font stacks for you to choose from. Simply copy and paste one of their font stacks and you're all set!

Try it yourself: Try adding a font to your `my_webpage.html` by adding `font-family` CSS to the `body` tag. You can use a font stack from Modern Font Stacks, or make up your own!

### Font size

One last thing before we move on: changing the font size! This is really simple: the property is simply called `font-size` and it can be specified in a number of ways, including pixels or points. For example, if you wanted 12 point font: 

```
body {
  font-size: 12pt;
}
```

And that's it!
