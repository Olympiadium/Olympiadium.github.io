---
layout: default
title: MS Earth Science | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /science-olympiads/lecture-notes/megastudy-earth-science/
---
<h1>Megastudy Earth Science</h1>
<ul class="breadcrumb">
	<li><a href="{{ site.homeurl }}">Olympiadium</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/">Science Olympiads</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/lecture-notes/">Lecture Notes</a></li> 
	<li><a href="{{ site.homeurl }}science-olympiads/lecture-notes/megastudy-earth-science/">MS Earth Science</a></li>
</ul>

{% for topic in site.data.ms_earth-science_topic_list %}
{% capture topic_name %}{{ topic | first }}{% endcapture %}
{% assign page_topic = site.data.ms_earth-science_topic_list[topic_name] %}
  <ul class="actions fit big">
  <li><a href="{{ site.baseurl }}{{ page.permalink}}chapter-{{ forloop.index | plus:0 }}" class="button fit big">{{ forloop.index | plus:0 }}강. {{ page_topic.name }}</a></li>
  </ul>
{% endfor %}
