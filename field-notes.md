---
layout: page
title: Field Notes
permalink: /field-notes/
---

I live in a village near a forest in Central Bohemia. I walk, watch, and record nature – birds, bugs, plants, the sky. These are my field notes: part citizen science, part diary.

You'll find: butterfly & moth observations (Lepidoptera mapping), seasonal plant records, weather & Moon phase notes, random bird encounters, and simple joy. The world outside is amazing. Let's not miss it.

---

<ul class="post-list" style="list-style-type: none; padding-left: 0;">
{% assign sorted_notes = site.field_notes | sort: "date" | reverse %}
{% for post in sorted_notes %}
  <li style="margin-bottom: 1.5rem;">
    <span style="color: #666; font-size: 0.9rem;">{{ post.date | date: "%Y-%m-%d" }}</span>
    <h3 style="margin-top: 0.2rem; margin-bottom: 0.2rem;">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
  </li>
{% endfor %}
</ul>
