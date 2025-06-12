---
layout: default
title: Blog
permalink: /blog/
pagination:
  enabled: true
---

<h1>Blog 📔</h1>
<!--
<p>Total posts: {{ paginator.posts | size }}</p>
<p>Total pages: {{ paginator.total_pages }}</p>
<p>Current page: {{ paginator.page }}</p>
<p>Previous page? {{ paginator.previous_page }}</p>
<p>Next page? {{ paginator.next_page }}</p>
-->

{% assign listed_posts = site.posts | where_exp:"post", "post.unlisted != true" %}
{% if listed_posts.size > 0 %}
  <ul>
    {% for post in listed_posts %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> - <small>{{ post.date | date: "%B %d, %Y" }}</small>
      </li>
    {% endfor %}
  </ul>

  <!-- Pagination Links -->
  {% if paginator.total_pages > 1 %}
    <nav class="pagination-nav">
      {% if paginator.previous_page %}
        <a class="prev" href="{{ paginator.previous_page_path }}">⬅️ Previous</a>
      {% else %}
        <span></span>
      {% endif %}
      {% if paginator.next_page %}
        <a class="next" href="{{ paginator.next_page_path }}">Next ➡️</a>
      {% else %}
        <span></span>
      {% endif %}
    </nav>
  {% endif %}
{% else %}
  <p>Coming Soon!</p>
{% endif %}