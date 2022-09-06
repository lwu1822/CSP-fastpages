---
layout: page
title: Weekly Work
permalink: /weekly-work/
---


<table>
    <tr>
        <th>Week</th>
        <th>Assignments</th>
    </tr>
    
    
    {% for i in (0..2) %}
    <tr>
        <td>{{ i }}</td>
        {% if i == 0 %}
            <td><a href="https://lwu1822.github.io/CSP-fastpages/jekyll-liquid/2022/08/31/jekyll-liquid.html">First post</a> <br> <a href="https://lwu1822.github.io/CSP-fastpages/python/2022/09/04/python.html">Python</a></td>
        {% endif %}

        {% if i == 1 %}
            <td> <a href="https://lwu1822.github.io/CSP-fastpages/bash/2022/09/05/tools.html">Bash: Check if tools are installed</a></td>
        {% endif %}

        
        {% if i == 2 %}
            <td><a href="https://lwu1822.github.io/CSP-fastpages/python/2022/09/05/w2-dictionary.html">Dictionary</a> <br> <a href="https://lwu1822.github.io/CSP-fastpages/html/2022/09/05/2_html-css.html">HTML and CSS</a></td>
        {% endif %}

    </tr>
    {% endfor %}
    


</table>

