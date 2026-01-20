---
layout: default
title: Blog
description: "Daily posts about Orlando and Central Florida—why it’s the greatest city to live."
---

# Blog

New posts added regularly.

{% for post in site.posts %}
- **[{{ post.title }}]({{ post.url }})** — <small>{{ post.date | date: "%B %-d, %Y" }}</small>  
  <small>{{ post.excerpt | strip_html | truncate: 160 }}</small>
{% endfor %}
