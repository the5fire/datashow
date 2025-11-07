---
layout: default
title: "Stock Files Index"
---

<h2>Stock 目录下的文件列表</h2>
<ul>
  {% for file in site.static_files %}
    {% if file.path contains 'stock' and file.extname == '.html' %}
      <li><a href="{{ file.path | relative_url }}">{{ file.name }}</a></li>
    {% endif %}
  {% endfor %}
</ul>
