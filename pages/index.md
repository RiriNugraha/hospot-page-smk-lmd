---
layout: default
title: Daftar Halaman
---

<h1>Daftar Halaman</h1>

<ul>
{% for file in site.static_files %}
    {% if file.extname == ".html" %}
        <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
{% endfor %}
</ul>