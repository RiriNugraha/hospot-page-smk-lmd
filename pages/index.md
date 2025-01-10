---
layout: default
title: Daftar File
---

<h1>Daftar File</h1>

<ul>
{% for file in site.static_files %}
    <li><a href="{{ file.path }}">{{ file.name }}</a></li>
{% endfor %}
</ul>