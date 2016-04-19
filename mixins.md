---
layout: category
description: Mixins; this is where the magic happens! Good typography, with Sass, involves a bit of maths :)
title: Mixins and Functions
nav: primary
---

<nav>
  <ul class="nav">

    {% for post in site.categories['mixins'] %}
    <li>
      <a class="post-link" href="#{{ post.title | downcase | replace:' ','-' | replace:',','' | strip_html }}">{{ post.title }}</a>
    </li>
    {% endfor %}

  </ul>
  <h1 class="sr-only">Section Menu</h1>
</nav>

{% for post in site.categories['mixins'] %}

{% include page-intro.html %}

{% endfor %}
