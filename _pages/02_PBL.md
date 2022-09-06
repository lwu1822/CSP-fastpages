---
layout: page
title: Weekly Work
permalink: /weekly-work/
---

## Week 0

* [First post](https://lwu1822.github.io/CSP-fastpages/jekyll-liquid/2022/08/31/jekyll-liquid.html)

* [Python](https://lwu1822.github.io/CSP-fastpages/python/2022/09/04/python.html)

## Week 1

* [Bash: Check if tools are installed](https://lwu1822.github.io/CSP-fastpages/bash/2022/09/05/tools.html)



<table>
    <tr>
        <th>Week</th>
        <th>Assignments</th>
    </tr>
    
    
    {% for i in (1..3) %}
    <tr>
        <td>{{ i }}</td>
    {% if i == 1 %}
        <td><a href="https://lwu1822.github.io/CSP-fastpages/jekyll-liquid/2022/08/31/jekyll-liquid.html">First post</a></td>
    {% endif %}
    </tr>
    {% endfor %}
    


</table>

