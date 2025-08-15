---
layout: default
title: Technosymbiosis Journal
---

<h1>{{ site.title }}</h1>
<p>{{ site.description }}</p>

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
      <span> — {{ post.date | date: "%d/%m/%Y" }}</span>
    </li>
  {% endfor %}
</ul>
