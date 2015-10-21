---
layout: page
title: Home Page
tagline: footprint...
---
{% include JB/setup %}

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)

## Latest article lists

<!-- This loops through the paginated posts -->

{% for post in site.posts %}
  <h1><a href="{{post.url}}">{{post.title}}</a></h1>
  <p class="info">
    <span class="info-item date">published on <a href="{{post.url}}">{{post.date | date: "%Y %m %d"}}</a></span>
    <!-- <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li> -->
  </p>
{% endfor %}


