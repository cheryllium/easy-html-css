---
title: Coding with Style
lesson: 8
layout: default
---

Let's say you have a bit of code like the following:

```html
beautiful <strong>constellations</strong>
```

If that's all you have (no CSS), it will look something like this: beautiful **constellations**. By default, the `strong` tag simply bolds the text. But let's say we want to make it fancier. Using CSS, we can change the way the `strong` tag affects the text. We can make all `strong` text purple, or underlined, or bigger, for example.

Your CSS code has to go in between `style` tags. The style tag should have an attribute `type` with the value "text/css", to tell it that we're using CSS. Inside of these style tags, we can **style** things by putting the name of what we want to style in front of curly braces, and putting our styles inside of the curly braces. 

That probably sounded a little confusing, but it should make more sense with an example:

```html
<style type="text/css">
    strong {
      color: #eeeeee;
    }
</style>
```

Notice how we have `strong` right in front of the curly braces. This tells us that we're changing the way the `strong` tag affects the text. In technical terms, this is called a **selector**, and we say that our CSS is *selecting* the `strong` tag.  

Inside of the curly braces, we can list our **CSS properties** in the format `property: value;`, like this: 

```
selector {
  property: value;
}
```

Make sure you put the colon and semicolon in the right spots. In the example above, the **property** is `color` and the **value** is `#eeeeee`. 

<div style="border:1px solid #666;border-radius:5px;padding:20px;">
    <p><b>Quick note:</b> The value <code>#eeeeee</code> represents a color in a special way that computers can understand. The format is a hashtag symbol (<code>#</code>) followed by six numbers or letters. The technical term for it is a <b>hexadecimal color code</b>. You can use the color picker below to find out the <b>color code</b> for any color, to use it in your CSS.</p>
    <div style="display:flex;align-items:center;">
    <input type="color" id="color-picker" value='#eeeeee'>
    &nbsp;&nbsp;Color code: &nbsp;<code id="color-code">#eeeeee</code>
    <script type="text/javascript">
    const colorPicker = document.querySelector('#color-picker');
    colorPicker.addEventListener("change", (event) => {
      const colorCode = document.querySelector('#color-code');
      colorCode.innerHTML = event.target.value;
    }, false); 
    </script>
    </div>
    <p style='margin-top:20px;'>If you are curious about how these codes work, I wrote a brief explanation in the appendix of this tutorial. But you don't need to understand them to use them; you just need to know how to find the code for the color you want, by using a <b>hexadecimal color picker</b> like the one above.</p>
</div>

### Text color and background color

In this example, we are setting the color to a color code, #eee, or light gray. Now, if we use the same HTML, we get a different result: beautiful <span style="color: #eee;">constellations</span>

Well, we can't see that very well. Luckily, there's another property we can change that might make that text easier to see. The `background-color` attribute will change the background color of whatever you are styling. Let's add a line for background-color, changing it to `#000000`, or black:

```html
<style type="text/css">
strong {
	color: #eeeeee;
	background-color: #000000;
}
</style>
```

Now, our HTML will render like this: beautiful <span style="color: #eee; background-color: #000">constellations</span>
