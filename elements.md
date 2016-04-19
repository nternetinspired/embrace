---
layout: category
description: The baseline css styles provided by Embrace. These low-level styles are applied only to named html elements, keeping specificity low.
title: Element Styles
nav: primary
---

<nav>
  <ul class="nav">

    {% for post in site.categories['elements'] %}
    <li>
      <a class="post-link" href="#{{ post.title | downcase | replace:' ','-' | replace:',','' | strip_html }}">{{ post.title }}</a>
    </li>
    {% endfor %}

  </ul>
  <h1 class="sr-only">Section Menu</h1>
</nav>

{% for post in site.categories['elements'] %}

{% include page-intro.html %}

{% endfor %}
