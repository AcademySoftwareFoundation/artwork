---
layout: default
title: Academy Software Foundation (ASWF) Logos
permalink: /
---

<section>
  <div class="logos">
    <h2>{{ page.title }}</h2>
    
    <p>{{ site.trademark_text }}</p>

{% for category in site.logo_categories %}
{% assign logo_groups = site.pages | where: "level", category | sort: "project_name" | sort: "order" %}
{% for logo_group in logo_groups %}
{% if forloop.first %}
<h3>{{ category }}</h3>
{% endif %}
<a href="{{ logo_group.dir }}">
<div class="outer-wrapper">
<div class="imagesquare">
<div class="imagecontainer"><img src="{{ logo_group.dir }}{{ logo_group.featured_image }}"></div><div class="imagesquarecta">View Logos »</div></div>
</div>
</a>
{% endfor %}
{% endfor %}

</div>
</section>
