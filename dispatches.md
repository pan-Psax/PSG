---
layout: page
title: Dispatches
permalink: /dispatches/
---

Are you looking for skeptical takes on Czech religious power grabs, political absurdities, and esoteric nonsense? This is where I vent. I mean, write.

These articles were originally written for the *Atropos Blog* – the official outlet of a small but stubborn skeptical society. Science, reason, and a dash of sarcasm.

---

<ul class="post-list" style="list-style-type: none; padding-left: 0;">
{% assign sorted_dispatches = site.dispatches | sort: "date" | reverse %}
{% for post in sorted_dispatches %}
  <li style="margin-bottom: 1.5rem;">
    <span style="color: #666; font-size: 0.9rem;">{{ post.date | date: "%Y-%m-%d" }}</span>
    <h3 style="margin-top: 0.2rem; margin-bottom: 0.2rem;">
      <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    </h3>
  </li>
{% endfor %}
</ul>
