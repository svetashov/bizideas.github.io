---
layout: page
permalink: /service/
title: Услуги
---

<div class="home">


  <ul class="post-list">
    {% for post in site.posts %}
      {% if post.type == "service" %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
          <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.postimage }}" class="post-image-on-index">
          <p class="post-description">{{ post.description | truncate: 200 }}</p>
          </a>
      </li>
      {% endif %}
    {% endfor %}
  </ul>

  

</div>
