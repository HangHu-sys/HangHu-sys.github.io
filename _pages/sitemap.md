---
layout: archive
title: "Sitemap"
permalink: /sitemap/
author_profile: true
---

{% include base_path %}

A list of the pages on this site. An [XML sitemap]({{ base_path }}/sitemap.xml) is also available.

<h2>Pages</h2>
<ul>
  {% for entry in site.pages %}
    {% unless entry.sitemap == false or entry.redirect_to or entry.url == page.url %}
      {% if entry.url == '/' %}
  <li><a href="{{ base_path }}{{ entry.url }}">Home</a></li>
      {% elsif entry.title and entry.title != '' %}
  <li><a href="{{ base_path }}{{ entry.url }}">{{ entry.title }}</a></li>
      {% endif %}
    {% endunless %}
  {% endfor %}
  <li><a href="{{ base_path }}/files/CV_HangHu.pdf">CV (PDF)</a></li>
</ul>

{% for collection in site.collections %}
  {% assign entries = collection.docs | where_exp: 'entry', 'entry.published != false' | sort: 'date' | reverse %}
  {% if collection.output and entries.size > 0 %}
<h2>{{ collection.label | capitalize }}</h2>
<ul>
    {% for entry in entries %}
  <li><a href="{{ base_path }}{{ entry.url }}">{{ entry.title }}</a></li>
    {% endfor %}
</ul>
  {% endif %}
{% endfor %}
