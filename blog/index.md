---
layout: default
work: true
main: true
title: "Blog"
description: 아주 가끔씩 관심 분야의 글을 올려요.
project-header: true
header-img: img/about.jpg
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.blog == true %}

    {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
