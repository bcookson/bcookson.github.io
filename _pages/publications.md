---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% include base_path %}


<h2><u>Papers</u></h2>

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
