---
layout: category
description: These opt-in modules, the goto for custom styling requirements, need only be enabled if they suit your project. Want to style things? You should probably do that here :)
title: Design Patterns
nav: primary
---

<nav>
  <ul class="nav">

    {% for post in site.categories['patterns'] %}
    <li>
      <a class="post-link" href="#{{ post.title | downcase | replace:' ','-' | replace:',','' | strip_html }}">{{ post.title }}</a>
    </li>
    {% endfor %}

  </ul>
  <h1 class="sr-only">Section Menu</h1>
</nav>

{% for post in site.categories['patterns'] %}

{% include page-intro.html %}

{% endfor %}
