---
layout: default
title: Staff
permalink: /staff/
---

<h1>Our Staff</h1>

<div class="staff-list">
  {% for member in site.staff %}
    <div class="item">
      <a class="staff-link" href="{{ site.baseurl }}{{ member.url }}">
        <div class="staff-image">
          {% if member.image %} <img src="{{member.image}}">
          {% endif %}
        </div>
        <div class="staff-name-section">
          <div class="staff-name">{{ member.display_name  }}</div>
          <div class="staff-position">{{ member.position }}</div>
        </div>
      </a>
    </div>
  {%- endfor -%}
</div>
