---
layout: post
title: Archive
permalink: /archive/
---

{% comment %} Order of sections on this page. Add a name here when you create a new category. {% endcomment %}
{% assign order = "current-events,markets,data,opinion" | split: "," %}

{% for name in order %}
{% assign posts = site.categories[name] %}
{% if posts %}
## {{ name | replace: "-", " " | capitalize }}

{% for post in posts %}
- {{ post.date | date: "%b %-d, %Y" }}: [{{ post.title }}]({{ post.url | relative_url }})
{% endfor %}
{% endif %}
{% endfor %}
