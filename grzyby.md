---
layout: page
title: Grzyby
---

<ul>
{% for item in site.data.mushrooms %}
  <li style="{% if item.isPoisonous %}color: red {% endif %}">
    {{ item.name }} (<em>{{ item.latinName }}</em>)
  </li>
{% endfor %}
</ul>
