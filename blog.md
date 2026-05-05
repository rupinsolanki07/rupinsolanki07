---
layout: page
title: Blog
permalink: /blog/
---

# Blog Posts

All posts in Markdown. Add new post in `_posts/` with filename: `YYYY-MM-DD-title.md`.

{% if site.posts.size > 0 %}
{% for post in site.posts %}
- [{{ post.title }}]({{ post.url | relative_url }}) — {{ post.date | date: "%b %-d, %Y" }}
{% endfor %}
{% else %}
No posts yet.
{% endif %}
