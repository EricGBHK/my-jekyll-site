---
layout: default
title: Home
---

{% assign preview_count = 5 %}
{% for cat in site.data.items %}
  {% assign name = cat[0] %}
  {% assign list = cat[1] %}
  <section class="section overview {{ name }}">
    <h2>
      <a href="{{ '/' | append: name | append: '/' | relative_url }}">
        {{ name | capitalize }} →
      </a>
    </h2>

    {% if name == "photos" or name == "drawings" %}
      <div class="grid-images">
        {% for img in list limit:preview_count %}
          <a href="{{ img.url }}">
            <img src="{{ img.src }}" alt="">
          </a>
        {% endfor %}
      </div>
    {% else %}
      <div class="two-col">
        <ul class="titles">
          {% for item in list limit:preview_count %}
            <li><a href="{{ item.url }}">{{ item.title }}</a></li>
          {% endfor %}
        </ul>
        <ul class="dates">
          {% for item in list limit:preview_count %}
            <li>{{ item.date }}</li>
          {% endfor %}
        </ul>
      </div>
    {% endif %}
  </section>
{% endfor %}
