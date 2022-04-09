---
layout: default
title:  "Learning to use Jekyll"
categories: Blog
---

# Publishing a blog post
Turns out, creating a new markdown file is not enough.

Publishing my [first post]({% post_url 2022-04-09-setting-up-a-blog %}) yielded a bare minimum html document,
with none of the thematic styling portrayed on the blog's landing site.

![screenshot of basic html rendering of blog post](/assets/images/screenshots/vanilla-html-blog-post.jpg)

## How to resolve
Doing a quick search online yielded [this post](https://github.community/t/page-not-showing-the-theme/10340/3)
found in the Github Community.

As can be seen in the [source code](https://github.com/shmolf/shmolf.github.io/blob/c443a134b7b5ff2cb1af4b61005e29a49267731a/_posts/2022-04-09-setting-up-a-blog.md?plain=1#L2)
of the blog post, I referenced `layout: post`, when in fact, I should be referencing `layout: default`.

This post is a test, to be sure it works. I'll commit an update with the results of said test.
