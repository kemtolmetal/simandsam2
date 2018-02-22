---
layout: page-portfolio
title: Photoworks
permalink: /photoworks/
page-cat: photoworks
tags:
- commercial
- fashion
- product
---

<div class="posts">
  {% for post in site.categories.photoworks %}
    <article class="post photoworks {% for tags in post.tags %}{{ tags }} {% endfor %}">
      <h2><a href="{{ site.baseurl }}{{ post.url }}">
        {{ post.title }}
        </a></h2>
      {{ post.content }}
    </article>
  {% endfor %}
</div>
