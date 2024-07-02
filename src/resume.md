---
layout: page
title: Resume
---

<h2>Resume Goes Here...</h2>
<ul>
  {% for post in collections.posts.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
    </li>
  {% endfor %}
</ul>

