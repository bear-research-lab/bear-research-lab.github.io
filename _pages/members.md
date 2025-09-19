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
<!-- Graduate Students: compact 4-column grid -->
<div class="member-grid member-grid--grads">
  {% for person in block.people %}
    {% assign detail = nil %}
    {% if person.slug %}
      {% assign detail = site.people | where: "slug", person.slug | first %}
    {% endif %}
    <div class="member-card member-card--compact">
      <div class="member-photo">
        {% if person.website %}
          <a href="{{ person.website }}" target="_blank" rel="noopener">
            <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
          </a>
        {% else %}
          <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
        {% endif %}
      </div>
      <div class="member-info">
        <div class="member-name">
          {% if person.website %}
            <a href="{{ person.website }}" target="_blank" rel="noopener">{{ person.name }}</a>
          {% else %}
            {{ person.name }}
          {% endif %}
        </div>
        <div class="member-links">
          {% if person.website %}
            <a class="btn" href="{{ person.website }}" target="_blank" rel="noopener">Website</a>
          {% endif %}
          {% if detail %}
            <a class="btn" href="{{ detail.url | relative_url }}">More info</a>
          {% endif %}
        </div>
      </div>
    </div>
  {% endfor %}
</div>


  {% else %}
  <!-- PI and any other groups: FULL layout -->
  <div class="member-grid">
    {% for person in block.people %}
      {% assign detail = nil %}
      {% if person.slug %}
        {% assign detail = site.people | where: "slug", person.slug | first %}
      {% endif %}
      <div class="member-card">
        <div class="member-photo">
          {% if person.website %}
            <a href="{{ person.website }}" target="_blank" rel="noopener">
              <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
            </a>
          {% else %}
            <img src="{{ person.img | relative_url }}" alt="{{ person.name }}">
          {% endif %}
        </div>
        <div class="member-info">
          <div class="member-name">
            {% if person.website %}
              <a href="{{ person.website }}" target="_blank" rel="noopener">{{ person.name }}</a>
            {% else %}
              {{ person.name }}
            {% endif %}
          </div>
          {% if person.role %}<div class="member-role">{{ person.role }}</div>{% endif %}
          {% if person.affiliation %}<div class="member-affiliation">{{ person.affiliation }}</div>{% endif %}
          {% if person.office %}<div class="member-office"><span class="label">Office:</span> {{ person.office }}</div>{% endif %}
          {% if person.phone %}<div class="member-phone"><span class="label">Phone:</span> {{ person.phone }}</div>{% endif %}
          {% if person.email %}<div class="member-email"><span class="label">Email:</span> {{ person.email }}</div>{% endif %}
          <div class="member-links">
            {% if person.website %}<a href="{{ person.website }}" target="_blank" rel="noopener">Website</a>{% endif %}
            {% if person.linkedin %}<a href="{{ person.linkedin }}" target="_blank" rel="noopener">LinkedIn</a>{% endif %}
            {% if person.scholar %}<a href="{{ person.scholar }}" target="_blank" rel="noopener">Scholar</a>{% endif %}
            {% if detail %}
              <a class="btn" href="{{ detail.url | relative_url }}">More info</a>
            {% endif %}
          </div>
        </div>
      </div>
    {% endfor %}
  </div>

{% endcase %}
{% endfor %}
