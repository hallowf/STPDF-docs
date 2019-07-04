---
layout: about
title: titles.about
has_children: true
permalink: /about/
nav_order: 4
---

{% if site.ga_tracking != nil %}
<script>gtag('config', '{{ site.ga_tracking }}', {'page_path': window.location.pathname})</script>
{% endif %}

{% tf about/about.md %}