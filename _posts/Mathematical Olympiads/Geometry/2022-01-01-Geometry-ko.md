---
layout: default
title: Geometry | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/geometry/
---
<h1>Geometry Content</h1>
<a href="{{ site.homeurl }}">Olympiadium</a> > <a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a> > <a href="{{ site.homeurl }}mathematical-olympiads/geometry/">Geometry</a><br><br>
{% for topic in site.data.geometry_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.geometry_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}olym-{{ forloop.index | plus:0 }}g" class="button fit big">Olym {{ forloop.index | plus:0 }}G. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
