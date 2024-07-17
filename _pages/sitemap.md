---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
cvurl: '/files/CV_Anna.pdf'
---

{% include base_path %}

<h2>Projects</h2>
{% for post in site.portfolio %}
  {% include archive-single.html %}
{% endfor %}

<h2>CV</h2>
You can download my CV using the link below:

[Download CV (PDF)]({{ page.cvurl }})

<!-- <h2>Pages</h2>
{% for post in site.pages %}
  {% include archive-single.html %}
{% endfor %}

<h2>Posts</h2>
{% for post in site.posts %}
  {% include archive-single.html %}
{% endfor %}

{% capture written_label %}'None'{% endcapture %}

{% for collection in site.collections %}
{% unless collection.output == false or collection.label == "posts" %}
  {% capture label %}{{ collection.label }}{% endcapture %}
  {% if label != written_label %}
  <h2>{{ label }}</h2>
  {% capture written_label %}{{ label }}{% endcapture %}
  {% endif %}
{% endunless %}

{% for post in collection.docs %}
  {% unless collection.output == false or collection.label == "posts" %}
  {% include archive-single.html %}
  {% endunless %}
{% endfor %}
{% endfor %}
-->