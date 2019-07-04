---
layout: page
title: titles.terms
parent: titles.about
permalink: /terms-and-conditions/
nav_order: 2
---

{% if site.ga_tracking != nil %}
<script>gtag('config', '{{ site.ga_tracking }}', {'page_path': window.location.pathname})</script>
{% endif %}

{% tf about/terms.md %}