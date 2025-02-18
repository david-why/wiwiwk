---
title: "What I Wish I Would've Known"
---

This is a website

## Speakers

{% for post in site.posts %}
  - [{{ post.title }}]({{ post.url | prepend: site.baseurl }})
{% endfor %}
