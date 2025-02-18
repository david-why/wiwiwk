---
title: "What I Wish I Would've Known"
---

This is a website

## Speakers

{% assign speakers = site.posts | where_exp: "item", "item.categories contains 'Speaker'" %}

{% for post in speakers %}
  - [{{ post.title }}]({{ post.url | prepend: site.baseurl }})
{% endfor %}
{% if speakers.size == 0 %}
  No speakers yet
{% endif %}
