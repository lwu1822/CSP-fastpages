---
toc: true
layout: post
description: Recording my learnings on using Jekyll.
categories: [jekyll-liquid]
title: Jekyll and Liquid
---

While I was setting up my fastpages blog, I noticed this interesting line of code in `index.html`. 

![]({{site.baseurl}}/images/index_html_code.png "code in index.html to insert image")

And I thought, *hey, this is interesting, what does {% raw %} 
{{site.baseurl}} 
{% endraw %} do?*

After some [googling](https://www.google.com/), I found that `{{ site.baseurl }}` wasn't something in Markdown. Turns out it's actually Jekyll syntax. 

So what does `{{ site.baseurl }}` do? 

Basically, `baseurl` is the directory under the URL of the website. So for example, this blog's URL is `lwu1822.github.io`, and the baseurl is `CSP-fastpages`. 

So instead of typing out `![](lwu1822.github.io/CSP-fastpages/images/diagram.png)`, I can instead just do `![]({{site.baseurl}}/images/diagram.png)`. Saves a lot of typing.

Pretty cool, huh? 😊

**Something else I encountered while typing this blog** 


###### Things for me to contemplate on:

I noticed on the provided [Fastpages Notebook Blog Post](https://lwu1822.github.io/CSP-fastpages/jupyter/2020/02/20/test.html), you can add an image without the baseurl. For example, you can specify an image with `![](images/diagram.png)`. Not sure why that works, but I'm guessing it has something to with Jupyter Notebooks.
