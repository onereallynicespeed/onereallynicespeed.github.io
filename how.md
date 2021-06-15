---
layout: default
permalink: /how
title: "How to singlespeed"
cover_image: "IMG_5815_1x.jpeg"
---

<ul>
			{% for link in site.data.categories %}
			{% if link.url contains 'http' %}
			{% assign domain = '' %}
			{% else %}
			{% assign domain = site.url %}
			{% endif %}
				<li><a href="{{ domain }}{{ link.url }}" {% if link.url contains 'http' %}target="_blank"{% endif %} class="no-bottom">{{ link.title }}</a></li>
			{% endfor %}
	</ul>