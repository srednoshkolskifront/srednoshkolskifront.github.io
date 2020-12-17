---
layout: splash
permalink: /
hidden: true
header:
  overlay_image: https://i.imgur.com/Lt4ZTpF.png
  overlay_filter: 0.5
  teaser: /assets/images/500x300.png
  og_image: /assets/images/500x300.png
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
