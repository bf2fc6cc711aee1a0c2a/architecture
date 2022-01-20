---
title: ADRs
permalink: /padr/
layout: default
---

<link rel="stylesheet" href="/css/adr.css">

# Platform Architecture Decision Records

# Accepted Platform ADRs

<table>
{% assign padrs = site.padr | sort: "num" %}
{% for adr in padrs %}

  <tr>
    <td><span class="status-{{ adr.status | downcase }}">
      <a href="{{ adr.num | escape }}/">PADR-{{ adr.num }}: {{ adr.title }}</a>
      {% for tag in adr.tags %}
      <span class="tag tag-{{tag}}">{{tag}}</span>
      {% endfor %}</span>
    </td>
    <td>
      {{ adr.status }}
    </td>
  </tr>

{% endfor %}
</table>

