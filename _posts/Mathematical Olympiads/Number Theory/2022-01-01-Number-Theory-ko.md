---
layout: default
title: Number Theory | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/number-theory/
---
<h1>Number Theory Content</h1>
<ul class="breadcrumb">
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/number-theory/">Number Theory</a></li>
</ul>
{% for topic in site.data.number-theory_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.number-theory_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}olym-{{ forloop.index | plus:0 }}n" class="button fit big">Olym {{ forloop.index | plus:0 }}N. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
