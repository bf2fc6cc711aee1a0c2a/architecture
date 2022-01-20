---
title: ADRs
permalink: /adr/
layout: default
---

<link rel="stylesheet" href="/css/adr.css">

# Architecture Decision Records

If you don't know what an ADR is, look [here](/about/#architecture-decision-records-adr).

# Accepted ADRs

<table>
{% assign adrs = site.adr | sort: "num" %}
{% for adr in adrs %}

  <tr>
    <td>
      <a href="{{ adr.num | escape }}/">ADR-{{ adr.num }}: {{ adr.title }}</a>
      {% for tag in adr.tags %}
      <span class="tag">{{tag}}</span>
      {% endfor %}
    </td>
    <td>
      {{ adr.status }}
    </td>
  </tr>

{% endfor %}
</table>

<!-- # ADRs in elaboration

<table>
{% for adr in site.adrs %}
{% if adr.status == 'Proposed' or adr.status == 'In progress' or adr.status == 'In review' %}
  <tr>
    <td>
      <a href="{{ adr.url }}">ADR-{{ adr.num }}: {{ adr.name }}</a>
    </td>
    <td>
      {{ adr.status }}
    </td>
  </tr>
{% endif} %}
{% endfor %}
</table> -->



