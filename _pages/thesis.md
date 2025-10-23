---
layout: archive
title: "Theses"
permalink: /theses/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% assign theses = site.theses | sort: "date" | reverse %}

{% assign thesis_count = theses | size %}

{% if thesis_count > 0 %}
<div class="pub-section pub-section--thesis">
  <h2 class="pub-section__heading">
    {% if thesis_count > 1 %}
      Theses
    {% else %}
      Master's Thesis
    {% endif %}
  </h2>
  {% for post in theses %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}
