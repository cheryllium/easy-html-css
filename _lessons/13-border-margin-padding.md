---
title: Border, Margin, and Padding
lesson: 13
layout: default
---

Let's introduce a few more attributes you can use to style the `header`, `content`, and `footer` from the last section. Using CSS, we can give each section a fancy border, a margin, and some padding. 

While you're working through this section, be sure to follow along using the HTML code from the last section to see all of the code in action!

### Border

The `border` CSS attribute looks like this: 

```
#header {
  border: 2px solid #00ff00; // green
}
```

(Remember, `// green` is a **comment** which means everything after the `//` will be ignored.) 

The **value** of the `border` attribute has three parts: 

- `2px` - This is how wide the border is, in pixels. 
- `solid` - This is the style of the border. Solid means it will be a solid line. You can also have `dashed`, for a dashed line, `dotted` for a dotted line, or `inset` for a cool 3D effect. 
- `#0f0#` - This is the color of the border, as a hexadecimal color code. 

<div class="try-it">

<p>Try adding different borders to your header, content, and footer. You can try writing different values for each of the three parts: for example, try writing <code class="language-plaintext highlighter-rouge">10px</code> instead of <code class="language-plaintext highlighter-rouge">2px</code> for the width, try writing <code class="language-plaintext highlighter-rouge">dashed</code> instead of <code class="language-plaintext highlighter-rouge">solid</code>, and try picking a different hexadecimal color!</p>

</div>

### Margin and Padding

Next, let's talk about the margin and padding of an element. First, the margin refers to the space **around** your element. Try adding the following 20-pixel margin to your header and see what happens. We'll also add a border so you can clearly see the borders of the element. 

```html
#header {
  border: 2px solid #00ff00; 
  margin: 20px;
}
```

If you try this out on your page, you'll see the element appear to shrink as it gets 20 pixels of margin around each side. Now, let's see what padding does: 

```html
#header {
  border: 2px solid #00ff00; 
  padding: 20px;
}
```

Try it out! Now, you'll see that the space between the borders and the stuff inside of the header has increased. Padding refers to the space inside an element that's padding out its contents. Here, you can see that there are 20 pixels of space between the border and the text inside. 

<div class="try-it">

<p>If you didn’t follow along with the code above, give it a try now. First, add the line <code class="language-plaintext highlighter-rouge">margin: 20px;</code> to create 20 pixels of margin, and watch what happens. Then, try replacing it with <code class="language-plaintext highlighter-rouge">padding: 20px;</code> to see the difference. Finally, try writing it with both margin AND padding, and try adjusting them from 20 pixels to other amounts - for example, 5px or 50px.</p>

</div>

Note that some HTML elements have a bit of border and margin by default, so they might not behave exactly as you expect. For example, the `h1` tag has some top and bottom margin by default, so you can expect to see a little extra vertical space in this padding example.

### Partial borders, etc

Finally, what if you only want there to be a border on the bottom of the element? Or what if you want to only put margin on the top of an element, or only pad one side? For the `border`, `margin`, and `padding` attributes, you can specify a single side by writing `-top`, `-bottom`, `-left`, or `-right` after the attribute. For example: 

```html
#header {
  border-top: 2px solid #00ff00; 
  margin-bottom: 20px; 
  padding-left: 20px;
}
```

In this example, there will only be a border at the top, a margin on the bottom, and a padding on the left side of the element. 
