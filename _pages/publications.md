---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<h2 style="font-weight:bold;">Preprints</h2>
{% for post in site.publications reversed %}
  {% if post.status == 'preprint' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}

<h2 style="font-weight:bold;"> </h2>
{% for post in site.publications reversed %}
  {% if post.status == 'published' %}
    {% include archive-single.html %}
  {% endif %}
{% endfor %}
