---
title: "HTML Tags: An Introduction"
lesson: 2
layout: default
---

If you've ever seen HTML before, you know there are a lot of things that go in between < and > signs. These things are called **tags**. There are two types of tags in HTML, but we're going to just worry about one to begin with. The first type of tag is the **opening and closing tag**. Here is an example:

```html
<em>supernova</em> explosion
```

There are a couple of things to note about this example. Let's not worry about what `em` means, and just focus on the basic syntax. First, **notice how there is a forward slash in the second `em` tag**. That indicates that it is a **closing tag**. The first `em` tag is an **opening tag**. Everything **in between the opening and closing tags** is affected by the tag.

Thus, in this example, the word *supernova* will be affected by the `em` tags, but the word *explosion* will not be affected (it is outside the tags). Pretty simple so far, right?

You can place these tags inside of each other. This is called **nesting tags** in programmer speak. For example:

```html
<em>supernova <strong>explosion</strong></em>
```

Here, the word *supernova* is affected by only the `em` tag, but the word *explosion* is affected by both the `em` and `strong` tags. This is illustrated by the diagram below: 

<div style="text-align:center">
    <img src="/assets/ch02_diagram.png" style="width:600px;max-width:100%;border:1px solid #eee" />
</div>

In this diagram, everything in between the `em` tags is underlined in green, and everything in between the `strong` tags is underlined in pink. The word *supernova* is affected by only the `em` tag, but the word *explosion* has both a pink and green underline, and is affected by both tags. 

Now that we have these out of the way, let's talk about what these tags actually mean and do - and learn some more while we're at it.
