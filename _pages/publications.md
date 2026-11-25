---
layout: archive
title: "Selected Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<div class="pub-toolbar">
  <p class="pub-note">* Equal contribution. The full list is on <a href="{{ site.author.googlescholar }}">Google Scholar</a>.</p>
  <button type="button" class="pub-toggle-all" aria-pressed="false">Expand all</button>
</div>

{% comment %}Drop compact=true (and the toolbar button and script) for the full card view.{% endcomment %}
{% include publication-sections.html compact=true %}

<script>
  (function () {
    var button = document.querySelector(".pub-toggle-all");
    if (!button) return;
    button.addEventListener("click", function () {
      var open = button.getAttribute("aria-pressed") !== "true";
      document.querySelectorAll(".pub-compact__details").forEach(function (d) { d.open = open; });
      button.setAttribute("aria-pressed", open ? "true" : "false");
      button.textContent = open ? "Collapse all" : "Expand all";
    });
  })();
</script>
