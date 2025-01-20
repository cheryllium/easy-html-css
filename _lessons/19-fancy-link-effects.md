---
title: Fancy Link Effects
lesson: 19
layout: default
---

This project is coming along nicely; we have finished our layout and chosen some colors to give it some personality. The next thing we'll do is customize the sidebar links. 

### Linking with Style

Let's customize our links by: 

- Removing the underline
- Adding font and background colors
- Spacing them out and padding the contents
- Add a decorative partial border

#### Remove the Default Underline

Links are underlined by default, but this can be removed with CSS. Normally, underline is controlled by the `text-decoration` property, which sets decorative lines on text. You can actually control a lot with this property, but we will focus on these three possible values: 

- `text-decoration: underline;` specifies that the text should be underlined.
- `text-decoration: line-through;` specifies that the text should have a line through it: ~~like this~~
- `text-decoration: none;` specifies that the text should not be underlined. 

In your CSS, find the code that selects `#sidebar a`, in other words, every `a` tag that's in the `#sidebar`. You should already have some code here setting these links to `display: block;` from a previous lesson. Go ahead and add the rule: `text-decoration: none;`

#### Add Font and Background Colors

Next, we can add `background-color` and `color` properties. Recall that the `color` property, although it is just named "color", controls the font color. 

Try using what you learned in the last section to choose link colors with the inspector. Remember: right-click on the link and choose "Inspect" (or "Inspect Element") to bring up the inspector. Make sure that one of your `a` tags is selected in the HTML panel, and then add your rules in the CSS panel.

I will give my links white text and a teal background:

```
color: #ffffff;
background-color: #257c8a; 
```

#### Add Margin and Padding

Finally, let's space out our links a little by adding some margin. The `margin` property will add margin to all sides of the link, but we don't need it on every side. If we just want to space them out vertically, we can do so by adding margin to the **bottom** of every link, with the `margin-bottom` property. 

```
margin-bottom: 10px;
```

Next, let's add some padding, which will add space between the link text and the border of the link. This will look like there is more space to see the background color. 

```
padding: 5px; 
```

#### Add a Decorative Partial Border

One easy trick to make your web design more interesting is to give an element a partial border, instead of a complete border on all sides. Sometimes, it looks cooler to just do one or two sides. 

Recall that for margin and padding, you can specify it for a single side by adding `-left`, `-right`, `-top`, or `-bottom`. You can do the same thing with the `border` property. Let's try adding a thick white border to the left side: 

```
border-left: 5px solid #ffffff; 
```

If you like, you can add the same border on the right side as well:

```
border-left: 5px solid #ffffff; 
border-right: 5px solid #ffffff; 
```

It's okay to have more than one property that starts with `border-`. You can put completely different borders on each side as well!

### Adding Hover Effects

CSS doesn't just allow us to style links, but it even has a feature where we can put different CSS on the link **in different states**, including when the link is being hovered over. 

To style a hovered link, we simple write `a:hover` instead of `a` in our CSS. The `:hover` here is called a "pseudo-class" and it's a magical way of saying "select an `a` tag only when it is hovered". 

To test this out, let's add a rule that puts a line through the link when it is hovered over, using the `text-decoration` property. 

```
#sidebar a:hover {
  text-decoration: line-through; 
}
```

The selector `#sidebar a:hover` means: "select every `a` tag that is being hovered over, and is in the `#sidebar` element".

Now, refresh the page and try hovering over the link. There will now be a line through it. However, notice that all of the CSS we wrote for the `a` tag still applies. That's because the link is still using an `a` tag. The browser will apply all of that first, and then add the styles for `a:hover` over top of that. 

It will use the `a:hover` rules for any properties they both have. For example, we already `text-decoration: none;` on our `a` tag. Our `a:hover` rule changes this for hovered links, but everything else stays the same. 

<div class="screenshot">
  <img src="/assets/ch19_1.png" />
</div>

The tweaks we made on this page are just some ideas for what you can do. This is your webpage, so don't be afraid to experiment! For example, what if you changed the background or border colors on hover instead? 

You can download the code so far [here](), and view a live example [here](/project/index-4.html).
