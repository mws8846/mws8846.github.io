---
layout: default
work: true
main: true
title: Book recommendation
description: 좋은 책 지식 공유!
post-header: true
header-img: "img/book.jpg"
---

<div class="catalogue">
{% assign sorted = site.pages | sort: 'order' | reverse %}
{% for page in sorted %}
{% if page.book == true %}

     {% include post-list.html %}

{% endif %}
{% endfor %}
</div>
