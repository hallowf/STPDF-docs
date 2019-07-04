---
layout: page
title: titles.privacy
parent: titles.about
permalink: /license/
nav_order: 1
---

{% if site.ga_tracking != nil %}
<script>gtag('config', '{{ site.ga_tracking }}', {'page_path': window.location.pathname})</script>
{% endif %}

{% tf about/privacy.md %}