---
layout: page
title: Field Notes
permalink: /field-notes/
---

Observations, phenology, and nature field notes from Central Bohemia.

---

<ul class="post-list" style="list-style-type: none; padding-left: 0;">
{% for post in site.categories.field-notes %}
  <li style="margin-bottom: 1.5rem;">
    <span style="color: #666; font-size: 0.9rem;">{{ post.date | date: "%Y-%m-%d" }}</span>
    <h3 style="margin-top: 0.2rem; margin-bottom: 0.2rem;">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
  </li>
{% endfor %}
</ul>
