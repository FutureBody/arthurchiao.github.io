---
layout: default
title: Articles
---

<div id="articles">
  <h1>Articles</h1>
  <ul class="posts noList">
    {% for post in site.posts %}
      {% if post.url contains "-zh" %}
        <li>
          <span class="date">{{ post.date | date: "%Y-%m-%d" }}</span>
          <h4><a href="{{ post.url }}">{{ post.title }}</a></h4>
        </li>
      {% endif %}
    {% endfor %}
  </ul>
</div>