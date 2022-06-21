---
layout: page
title: Blog
permalink: /blog/
---

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <p> {{ post.content | markdownify | strip_html | truncatewords: 80, " (...)" }}</p>
    </li>
  {% endfor %}
</ul>
