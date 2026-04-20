---
layout: page
title: Members
permalink: /members/
---

{% for block in site.data.members %}
### {{ block.group }}

{% assign group_name = block.group | default: "" | strip | downcase %}

{% case group_name %}

{% when "graduate students" %}
<div class="member-grid member-grid--grads">
  {% for person in block.people %}
    <div class="member-card member-card--compact">
      <div class="member-photo">
        <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
      </div>
      <div class="member-info">
        <div class="member-name">{{ person.name }}</div>
      </div>
    </div>
  {% endfor %}
</div>

{% when "undergraduate researchers" %}
<div class="member-list-simple">
  <ul style="list-style-type: none; padding-left: 0; display: flex; flex-wrap: wrap; gap: 15px;">
    {% for person in block.people %}
      <li class="member-name-only" style="font-size: 1.1em; font-weight: 500;">
        {% if person.website %}
          <a href="{{ person.website }}" target="_blank" rel="noopener">{{ person.name }}</a>
        {% else %}
          {{ person.name }}
        {% endif %}
      </li>
      {% unless forloop.last %} <span style="color: #ccc;">|</span> {% endunless %}
    {% endfor %}
  </ul>
</div>

{% else %}
<div class="member-grid">
  {% for person in block.people %}
    <div class="member-card">
      <div class="member-photo">
        <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
      </div>
      <div class="member-info">
        <div class="member-name">{{ person.name }}</div>
        {% if person.role %}<div class="member-role">{{ person.role }}</div>{% endif %}
        <div class="member-links">
          {% if person.website %}<a href="{{ person.website }}">Website</a>{% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>

{% endcase %}
{% endfor %}