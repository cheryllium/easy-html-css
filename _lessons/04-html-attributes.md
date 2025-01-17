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

Now, you can try it!

<div class="try-it">

In the last section, you saved an HTML file <code class="language-plaintext highlighter-rouge">my_webpage.html</code> to your computer. Now, save a new file called <code class="language-plaintext highlighter-rouge">about_me.html</code> with the following contents:</p>

<div class="language-html highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;h1&gt;</span>About me<span class="nt">&lt;/h1&gt;</span>
<span class="nt">&lt;p&gt;</span>I'm learning HTML and CSS!<span class="nt">&lt;/p&gt;</span>
</code></pre></div></div>

<p>Make sure to save <code class="language-plaintext highlighter-rouge">about_me.html</code> in the <strong>same folder</strong> as where you have <code class="language-plaintext highlighter-rouge">my_webpage.html</code>.</p>

<p>Now, let’s learn how to link to your new page. In <code class="language-plaintext highlighter-rouge">my_webpage.html</code>, add a new line somewhere in the file that says:</p>

<div class="language-html highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="nt">&lt;a</span> <span class="na">href=</span><span class="s">"about_me.html"</span><span class="nt">&gt;</span>About Me<span class="nt">&lt;/a&gt;</span>
</code></pre></div></div>

<p>Save it and open <code class="language-plaintext highlighter-rouge">my_webpage.html</code> in your web browser. Now, if you click the link, it will take you to your new about page.</p>

<p><strong>NOTE:</strong> The value of the <code class="language-plaintext highlighter-rouge">href</code> in this example is <code class="language-plaintext highlighter-rouge">about_me.html</code>, a <strong>relative path</strong>. Instead of containing the full URL, relative paths are relative to whatever folder you are currently in. In this case, it will look for an about_me.html file in the same folder. So this allows you to link to a different HTML file in the same folder.</p>

</div>

Don't worry if this is still a little confusing. We will go over attributes a little more in the next section, which should make it clearer.
