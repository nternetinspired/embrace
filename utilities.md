---
layout: category
description: One-trick ponies, these are lightweight and single-purpose utility classes designed to trump any existing styles.
title: Utility Classes
nav: primary
---

<nav>
  <ul class="nav">

    {% for post in site.categories['utilities'] %}
    <li>
      <a class="post-link" href="#{{ post.title | downcase | replace:' ','-' | replace:',','' | strip_html }}">{{ post.title }}</a>
    </li>
    {% endfor %}

  </ul>
  <h1 class="sr-only">Section Menu</h1>
</nav>

{% for post in site.categories['utilities'] %}

{% include page-intro.html %}

{% endfor %}
