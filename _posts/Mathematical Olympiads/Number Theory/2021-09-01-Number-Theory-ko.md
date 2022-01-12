---
layout: default
title: Number Theory | Olympiadium
date: 2021-09-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/number-theory/
---
<h1>Number Theory Content</h1>
<a href="{{ site.homeurl }}">Olympiadium</a> > <a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a> > <a href="{{ site.homeurl }}mathematical-olympiads/number-theory/">Number Theory</a><br><br>
{% for topic in site.data.number-theory_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.number-theory_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}olym-{{ forloop.index | plus:0 }}n" class="button fit big">Olym {{ forloop.index | plus:0 }}N. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
