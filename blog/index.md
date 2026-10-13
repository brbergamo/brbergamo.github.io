---
layout: blog
title: Blog
---

Notes on the methods I use every day in bioinformatics, one step of the ladder at a time.

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <span class="date">{{ post.date | date: "%B %-d, %Y" }}</span>
    {% if post.description %}<p class="excerpt">{{ post.description }}</p>{% endif %}
  </li>
{% endfor %}
</ul>

{% if site.posts.size == 0 %}
The first post is coming soon.
{% endif %}
