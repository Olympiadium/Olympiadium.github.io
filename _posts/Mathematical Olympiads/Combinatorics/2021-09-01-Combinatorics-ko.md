---
layout: default
title: Combinatorics | Olympiadium
date: 2021-09-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/combinatorics/
---
<h1>Combinatorics Content</h1>
<a href="{{ site.homeurl }}">Olympiadium</a> > <a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a> > <a href="{{ site.homeurl }}mathematical-olympiads/combinatorics/">Combinatorics</a><br><br>
{% for topic in site.data.combinatorics_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.combinatorics_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}olym-{{ forloop.index | plus:0 }}c" class="button fit big">Olym {{ forloop.index | plus:0 }}C. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
