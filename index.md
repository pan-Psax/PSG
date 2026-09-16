---
layout: default
title: "Home"
---

Welcome to the personal archive of field notes, essays, and observations.

---

### Field Notes & Articles

<ul class="post-list">
{% for post in site.posts %}
  <li>
    <span class="post-meta">{{ post.date | date: "%Y-%m-%d" }}</span>
    <h3>
      <a class="post-link" href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
  </li>
{% endfor %}
</ul>
