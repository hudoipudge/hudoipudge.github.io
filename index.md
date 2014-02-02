---
layout: page
title: Start page
tagline: for urls
---
{% include JB/setup %}

<div class="blog-index">
{% assign post = site.posts.first %}
{% assign content = post.content %}
{% include post_detail.html %}
</div>

Read [Jekyll Quick Start](http://jekyllbootstrap.com/usage/jekyll-quick-start.html)

Complete usage and documentation available at: [Jekyll Bootstrap](http://jekyllbootstrap.com)


## Sample Posts

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



