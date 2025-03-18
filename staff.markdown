---
layout: default
title: Team
permalink: /team/
---

<h1 class="staff-h1">Our Team</h1>

<div class="staff-list">
  {% assign team = site.team | sort: 'order' %}
  {% for member in team %}
    <div class="item">
      <a class="staff-link" href="{{ site.baseurl }}{{ member.url }}">
        <!--<div class="staff-image">
          {% if member.image %} <img src="{{member.image}}">
          {% endif %}
        </div>-->
        <div class="staff-name-section">
          <div class="staff-name">{{ member.display_name  }}</div>
          <div class="staff-position">{{ member.position }}</div>
        </div>
      </a>
    </div>
  {%- endfor -%}
</div>

---

<h1 class="staff-h1">Past Members</h1>
- Sumukh Prasad
- Pratham Sri Vasisht