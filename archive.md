---
layout: default
title: Archive
permalink: /archive/
---

<h1 class="post-title">Archive</h1>
<ul class="post-list archive-list">
  {% for post in site.posts %}
  <li>
    <span class="pl-date">{{ post.date | date: "%-d %b %Y" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    {% if post.teaser %}<span class="pl-teaser">{{ post.teaser }}</span>{% endif %}
  </li>
  {% endfor %}
</ul>
