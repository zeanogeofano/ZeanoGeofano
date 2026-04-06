---
layout: default
title: "Blog Posts"
---

<ul>
{% for post in site.posts %}
    <li>
        <a href="{{ post.url }}">{{ post.title }}</a> - {{ post.date | date: "%Y-%m-%d" }}<br>
        {{ post.excerpt }}
    </li>
{% endfor %}
</ul>