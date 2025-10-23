---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

{% assign conferences = site.publications | where: "pub_type", "conference" | sort: "date" | reverse %}
{% assign journals = site.publications | where: "pub_type", "journal" | sort: "date" | reverse %}
{% assign workshops = site.publications | where: "pub_type", "workshop" | sort: "date" | reverse %}
{% assign book_chapters = site.publications | where: "pub_type", "book" | sort: "date" | reverse %}
{% assign misc = site.publications | where: "pub_type", "misc" | sort: "date" | reverse %}

{% if conferences != empty %}
<div class="pub-section pub-section--conference">
  <h2 class="pub-section__heading">Conference Papers</h2>
  {% for post in conferences %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}

{% if journals != empty %}
<div class="pub-section pub-section--journal">
  <h2 class="pub-section__heading">Journal Articles</h2>
  {% for post in journals %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}

{% if workshops != empty %}
<div class="pub-section pub-section--workshop">
  <h2 class="pub-section__heading">Workshops &amp; Symposia</h2>
  {% for post in workshops %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}

{% if book_chapters != empty %}
<div class="pub-section pub-section--book">
  <h2 class="pub-section__heading">Book Chapters</h2>
  {% for post in book_chapters %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}

{% if misc != empty %}
<div class="pub-section pub-section--misc">
  <h2 class="pub-section__heading">Miscellaneous</h2>
  {% for post in misc %}
    {% include archive-single.html %}
  {% endfor %}
</div>
{% endif %}
