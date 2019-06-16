---
layout: default
work: true
main: true
title: Selected Projects
description: 프로젝트
project-header: true
header-img: "img/"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.projects == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>