---
bg: "tag.jpg"
layout: page
permalink: /archive/
title: "Archiv"
crawlertitle: "Blogarchiv"
summary: "Posts about jekyll"
active: active
---

<ul>
    {% for post in site.posts %}
    <li>
        <a href="{{site.baseurl}}{{post.url}}">{{post.title}}</a>
    </li>
    {% endfor %}
</ul>

<!--{% for tag in site.tags %}
  {% assign t = tag | first %}
  {% assign posts = tag | last %}

<h2 class="category-key" id="{{ t | downcase }}">{{ t | capitalize }}</h2>-->

<!--<ul class="year">
  {% for post in site.posts %}
    {% if post.tags contains t %}
      <li>
        {% if post.lastmod %}
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="date">{{ post.lastmod | date: "%d-%m-%Y"  }}</span>
        {% else %}
          <a href="{{ post.url }}">{{ post.title }}</a>
          <span class="date">{{ post.date | date: "%d-%m-%Y"  }}</span>
        {% endif %}
      </li>
    {% endif %}
  {% endfor %}
</ul>-->


<!--{% endfor %}-->
