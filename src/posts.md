---
layout: page
title: Posts
---

<ul>
  {% if collections.posts.resources | size == 0 %}
    <li>Coming Soon!</li>
  {% else %}
    {% for post in collections.posts.resources %}
      <li>
        <a href="{{ post.relative_url }}">{{ post.data.title }}</a>
      </li>
    {% endfor %}
  {% endif %}
</ul>

{% comment %}
If you have a lot of posts, you may want to consider adding [pagination](https://www.bridgetownrb.com/docs/content/pagination)!
{% endcomment %}