---
layout: default
title: Algebra | Olympiadium
date: 2021-12-25
mathjax: true
lang: ko
permalink: /mathematical-olympiads/algebra/
---
<h1>Algebra Content</h1>
<a href="{{ site.homeurl }}">Olympiadium</a> > <a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a> > <a href="{{ site.homeurl }}mathematical-olympiads/algebra/">Algebra</a><br><br>
{% for topic in site.data.algebra_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.algebra_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}olym-{{ forloop.index | plus:0 }}a" class="button fit big">Olym {{ forloop.index | plus:0 }}A. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
