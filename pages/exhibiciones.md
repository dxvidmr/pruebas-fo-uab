---
layout: page
permalink: /exhibiciones/
title: Exhibiciones
---

{% assign exhibits = site.exhibits | where: 'layout','exhibit' %}
<ul>
  {% for exhibit in exhibits %}
    <li>
      <a href='{{ exhibit.url | relative_url }}'>
        {{ exhibit.title }}
      </a>
    </li>
  {% endfor %}
</ul>
