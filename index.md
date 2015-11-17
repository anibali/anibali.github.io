---
layout: page
title: Welcome
tagline:
---
{% include JB/setup %}

## About me

Hello, my name is Aiden and this is my little corner of the Internet. I'm a
programmer and electronic engineer from Victoria, Australia with a passion
for open source software. Some of my past works can be found on the
[portfolio page](/portfolio.html).

<ul style="list-style-type: none;">
  <li>{% include icons/email %} <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a></li>
  <li>{% include icons/github %} github.com/<a href="https://github.com/{{ site.author.github }}">{{ site.author.github }}</a></li>
  <li>{% include icons/linkedin %} linkedin.com/in/<a href="http://www.linkedin.com/in/{{ site.author.github }}">{{ site.author.linkedin }}</a></li>
</ul>

## Latest posts

<ul class="posts">
  {% for post in site.posts limit:5 %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
  <a href="{{ site.JB.archive_path }}">More...</a>
</ul>
