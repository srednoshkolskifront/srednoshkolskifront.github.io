---
layout: splash
permalink: /
hidden: true
header:
  overlay_filter: 0.3
  overlay_image: /assets/images/home-page.jpg
  actions:
    - label: "Дознајте повеќе"
      url: "/about/"
excerpt: >
  Здружение на ученици во средните училишта во Македонија<br />
---

<h3 class="archive__subtitle">{{ site.data.ui-text[site.locale].recent_posts | default: "Recent Posts" }}</h3>

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.posts %}
{% endif %}

{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>
