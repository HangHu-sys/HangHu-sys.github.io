---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
{% include base_path %}

{% assign publications = site.publications | sort: 'date' | reverse %}
{% for post in publications %}
<article class="archive__item">
  <h2 class="archive__item-title"><a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a></h2>
  <div class="archive__item-excerpt">
    {{ post.authors | markdownify }}
    <p><em>{{ post.venue }}</em>, {{ post.volume }}({{ post.issue }}): {{ post.pages }}, {{ post.date | date: '%Y' }}.</p>
    <p><a href="{{ post.paperurl }}">Paper</a> &middot; <a href="{{ post.codeurl }}">Code</a> &middot; <a href="{{ post.doiurl }}">DOI</a></p>
  </div>
</article>
{% endfor %}
