---
layout: page
title: Publications
permalink: publications
order: 3
---

{% assign years = site.data.publications | group_by: "year" %}

{% for year in years %}
    {% assign publications = year.items %}
    {% include publications.html %}
{% endfor %}