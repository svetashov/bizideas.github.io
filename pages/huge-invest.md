---
layout: page
permalink: /huge-invest/
title: От 200 тыс. р.
---

<div class="home">

  <h1 class="page-heading">Бизнес с инвестициями от 200 тыс. р.</h1>

  <ul class="post-list">
    {% for post in site.posts %}
      {% if post.invest == "huge" %}
      <li>
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>
          <a href="{{ post.url | prepend: site.baseurl }}">
          <img src="{{ post.postimage }}" class="post-image-on-index">
          <p class="post-description">{{ post.description | truncate: 160 }}</p>
          </a>
      </li>
      {% endif %}
    {% endfor %}
  </ul>

  

</div>
