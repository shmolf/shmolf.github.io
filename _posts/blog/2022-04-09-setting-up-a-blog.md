---
layout: default
title:  "Setting up this blog"
categories: Blog
---

# Considerations

### Who's the purpose of the blog?
I sometimes find I need notes written in my own words, to reference in the future.
A google search, or a bookmarked page may suffice, but I appreciate my `tldr;` style.

Since I'm not selling anything, and I don't like reading long strings of text, I try to keep things concise.


### Who's the consumer of the blog?
Me. I'm writting these notes for myself.
I may reference them when I'm trying to help someone else understand something I've already struggled with.

### What capabilities do I expect from the blog?
I'm not looking to have a fanbase, so
- ~comments~
- ~polls~
- ~user management~ - big win here

So, what do I expect? I enjoy writting in Markdown syntax, and since most of my notes already exist
in this form, I'm expecting static information presented in a clean format, that support syntax highlighting.

## Actions
### Blog Domain
I could use the typical `shmolf.github.io`, but if I ever migrate away from Github, I don't want there
to be a migration issue for any users. Therefor, it's best for me to wrap this URL with a custom domain.

These notes are for me, but I thought `nicholas-browning-notes.blog` is a little ego-centric.

I hope these notes will benefit other developers beyond myself. So I settled on `dev-notes.blog`.

I registered the URL through <a href="https://domains.google.com" target="_blank">Google Domains</a>.
(Google makes it tough to de-Google one's self)

### Blog Content Management
I opted for Github Pages, since I'm already familiar with Github, and the feature seems to support my expectations.

Reading through
<a href="https://pages.github.com/" target="_blank">their summary</a>, and
<a href="https://docs.github.com/en/pages/quickstart" target="_blank">documentation</a>, it's pretty simple.

1. <a href="https://github.com/new" target="_blank">Create a new repo</a>
2. Name the repo something like `shmolf.github.io` where `shmolf` is replaced by your Github username.
3. Go to the Pages settings. For my blog, it was: `https://github.com/shmolf/shmolf.github.io/settings/pages`
4. Choose a theme
5. Provide the custom domain.
   1. It was here, that I got an error, which lead me to
      <a href="https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site" target="_blank">
        further documentation
      </a>
      about setting up the DNS records.
   2. I was interested in the
      <a href="https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site#configuring-an-apex-domain" target="_blank">
        Apex instructions
      </a>
   3. Specifically, I needed to create an `A` record with
      - the host pointed to `shmolf.github.io`
      - four IP addresses set up for the record data. (_Note: these IP addresses may change since this blog post_)
         - `185.199.108.153`
         - `185.199.109.153`
         - `185.199.110.153`
         - `185.199.111.153`
6. Enable https enforcement

## Begin writing
I am now writing this post, as a means to track what I did to set up this blog.
