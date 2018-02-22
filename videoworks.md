---
layout: page-portfolio
title: Videoworks
permalink: /videoworks/
page-cat: videoworks
tags:
- commercial
- series
- video content
- corporate
- documentary
- music
---

<div class="posts">
  {% for post in site.categories.videoworks %}
    <article class="post {% for tags in post.tags %}{{ tags }} {% endfor %}">
      <a href="{{ site.baseurl }}{{ post.url }}">
        <img src="http://i.ytimg.com/vi/{{ post.videoid }}/maxresdefault.jpg" />
        <span>{{ post.title }}</span>
      </a>
    </article>
  {% endfor %}
</div>
