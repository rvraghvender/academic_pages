---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if site.author.googlescholar %}
  <div class="wordwrap">You can also find my articles on <a href="{{site.author.googlescholar}}">my Google Scholar profile</a>.</div>
{% endif %}

{% include base_path %}
{% assign counter = 0 %}
<ol>
{% for post in site.publications reversed %}
  {% assign counter = counter | plus: 1 %}
  <li>
    <span style="font-weight: bold; display: inline;">{{ counter }}.</span>
    <span style="display: inline;">{% include archive-single.html %}</span>
  </li>
{% endfor %}
</ol>
