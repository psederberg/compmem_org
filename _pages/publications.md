---
layout: page
permalink: /publications/
title: Publications
description: Publications by categories in reversed chronological order. Generated by jekyll-scholar.
years: ["Submitted", "In Press", 2015, 2014, 2013, 2012, 2011, 2010, 2009, 2008, 2007, 2006, 2003, 1998, 1997]
---

{% for y in page.years %}
  <h3 class="year">{{y}}</h3>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
