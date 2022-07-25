---
layout: article
title: Olym 1C. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/combinatorics/olym-1c/theorems-and-techniques/
---
# Olym 1C. 귀납법과 알고리즘 <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.url }}">Olympiadium</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/combinatorics/">Combinatorics</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/combinatorics/olym-1c/">Olym 1C</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/combinatorics/olym-1c/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

## Greedy Algorithm
<skyblueboard><b>Example 1.1.</b>[(Source Here)](Link Here){:target="blank"} In a graph $G$ with $n$ vertices, no vertex has degree greater than $\delta$. Show that one can color the vertices using at most $\delta+1$ colors, such that no two neighboring vertices are the same color.</skyblueboard>
<b>Solution. </b> We use the following greedy algorithm: arrange the vertices in an arbitrary order. Let the colors be $1, 2, 3, \ldots$ Color the first vertex with color $1$. Then in each stage, take the next vertex in the order and color it with the smallest color that has not yet been used on any of its neighbors. Clearly this algorithm ensures that two adjacent vertices won’t be the same color. It also ensures that at most $\delta+1$ colors are used: each vertex has at most $\delta$ neighbors, so when coloring a particular vertex $v$, at most $\delta$ colors have been used by its neighbors, so at least one color in the set $\{1, 2, 3, …, \delta+1\}$ has not been used. The minimum such color will be used for the vertex $v$. Hence all vertices are colored using colors in the set $\{1, 2, 3,…, \delta+1\}$ and the problem is solved. $\blacksquare$