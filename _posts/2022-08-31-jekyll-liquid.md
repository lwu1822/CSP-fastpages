---
toc: true
layout: post
description: Recording my learnings on using Jekyll.
categories: [jekyll-liquid]
title: Jekyll and Liquid
---

<p style="font-size: 5px"><em>this took me hours to research btw</em></p>

While I was setting up my fastpages blog, I noticed this interesting line of code in `index.html`. 

![]({{site.baseurl}}/images/index_html_code.png "code in index.html to insert image")

And I thought, *hey, this is interesting, what does {% raw %} {{site.baseurl}} {% endraw %} do?*

After some [googling](https://www.google.com/), I found that {% raw %} `{{site.baseurl}}` {% endraw %} wasn't something in Markdown. Turns out it's actually Jekyll syntax. 

So what does {% raw %} `{{site.baseurl}}` {% endraw %} do? 

Basically, `baseurl` is the directory under the URL of the website. [^1] So for example, this blog's URL is `lwu1822.github.io`, and the baseurl is `CSP-fastpages`. 

So instead of typing out `![](lwu1822.github.io/CSP-fastpages/images/diagram.png)`, I can instead just do {% raw %} `![]({{site.baseurl}}/images/diagram.png)`. {% endraw %} Saves a lot of typing.

Pretty cool, huh? 😊

**Something else I encountered while making this post** 

{% assign openTag = '{%' %}

To type {% raw %} `{{site.baseurl}}` {% endraw %} in this Markdown file, apparently you have to use the {% raw %} `{% raw %}` {% endraw %} and `{{ openTag }} endraw %}` template. [^2]

For example:
{% raw %}
```
{{ openTag }} raw %} {{site.baseurl}} {{ openTag }} endraw %}
```
{% endraw %}


**Also something I encountered just as I was writing the line above**

Noticed how I was able to write `{{ openTag }} endraw %}` above? Unfortunately, it's not that simple to just type it directly into your IDE, like this

###### Things for me to contemplate on: 

I noticed on the provided [Fastpages Notebook Blog Post](https://lwu1822.github.io/CSP-fastpages/jupyter/2020/02/20/test.html), you can add an image without the baseurl. For example, you can specify an image with `![](images/diagram.png)`. Not sure why that works, but I'm guessing it has something to with Jupyter Notebooks.

# Test
{% assign openTag = '{%' %}
`{{ openTag }} endraw %}`

[^1]: [baseurl](https://mademistakes.com/mastering-jekyll/site-url-baseurl/)

[^2]: [Liquid template language](https://shopify.github.io/liquid/tags/template/)
