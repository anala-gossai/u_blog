---
title: "On starting a blog"
date: 2017-12-03
author: ""
draft: false
comments: false
image: ""
menu: ""
share: true
slug: "on-starting-a-blog"
tags: ["general"]
aliases: [
    "/2017/12/03/on-starting-a-blog/"
]
---

Having a blog as a way to learn new technical skills and build my personal brand was something I wanted to attempt. Therefore, I spent a weekend building this static website that could host simple markdown documents or HTML outputs. 

Although I have some familiarity with using [Jekyll](https://github.com/jekyll/jekyll) as a static site generator with GitHub Pages, I preferred the default aesthetics of [Hugo](https://gohugo.io/about/) with the [Casper theme](https://github.com/vjeantet/hugo-theme-casper).       

I started following the [Quick Start](http://gohugo.io/getting-started/quick-start/) guide for building and deploying Hugo as a GitHub Pages website. I did, however, make the following adjustments as I proceeded through the guides and help pages:   

+ I called my new blog directory `u_blog` rather than `quickstart` when running `hugo new site quickstart`     
+ Rather than `git submodule add`-ing the Casper theme, I `git clone`-ed it as recommended by the [Casper ReadMe](https://github.com/vjeantet/hugo-theme-casper)      
+ Of course, as the theme I chose was Casper, I updated the config file to include `echo 'theme = "casper"' >> config.toml`   
+ I received the error _"We were unable to load Disqus."_ at the bottom of my blog page, and solved this problem by deleting the `DisqusShortname` from my config file 
+ A non-intuitive edit was to create the `post` folder as `hugo new post/my-first-post.md` rather than `post`**`s`** as was instructed by the [Quick Start](http://gohugo.io/getting-started/quick-start/) guide     
+ As I intended to deploy the website via the `/docs` Folder on the Master Branch, I added `publishDir = "docs"` to the config file
	+ I followed the [instructions](http://gohugo.io/hosting-and-deployment/hosting-on-github/#deployment-via-docs-folder-on-master-branch) to modify the repository settings to allow GitHub to host the site    
	+ Note that I had to add a GitHub repository of the name `u_blog`, and then set the blog code as a new remote using `git remote add origin https://github.com ... .git` as instructed by [GitHub Help](https://help.github.com/articles/adding-a-remote/)        
+ Unfortunately, debugging various relative URLs is still a work in progress      

This blog is the resulting product of my attempt to execute a blog on GitHub Pages, and I hope to maintain this website as an entertaining forum!        
