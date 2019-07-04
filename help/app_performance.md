---
layout: page
title: titles.performance
parent: titles.help
permalink: /help/app-performance/
nav_order: 3
---

<!-- Tag page view -->
{% if site.ga_tracking != nil %}
<script>gtag('config', '{{ site.ga_tracking }}', {'page_path': window.location.pathname})</script>
{% endif %}

{% tf help/app_performance.md %}