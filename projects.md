---
layout: single
title: Projects
permalink: /projects/
---

# Projects

{% assign project_posts = site.categories.projects %}
{% if project_posts.size > 0 %}
{% for post in project_posts %}
## [{{ post.title }}]({{ post.url }})
<small>{{ post.date | date: "%B %d, %Y" }}</small>

{{ post.excerpt }}
{% endfor %}
{% else %}
No project posts yet.
{% endif %}
