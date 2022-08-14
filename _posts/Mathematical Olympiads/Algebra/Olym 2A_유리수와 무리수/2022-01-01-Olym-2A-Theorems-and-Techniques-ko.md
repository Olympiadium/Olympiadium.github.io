---
layout: article
title: Olym 2A. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/algebra/olym-2a/theorems-and-techniques/
---
# Olym 2A. 유리수와 무리수 <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/">Algebra</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/olym-2a/">Olym 2A</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/olym-2a/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

### Dirichlet's Approximation Theorem

$\lVert z \rVert$는 $z$에서 $z$와 가장 가까운 정수의 차이를 의미한다. 엄밀하게는 $$\lVert z \rVert = \begin{cases} \{z\} &if \{z\}<0.5 \\ 1-\{z\} &otherwise$$

<greenboard><b>Theorem 2.1.</b> 임의의 양의 정수 $N>1$과 실수 $\alpha$에 대하여 다음을 만족하는 정수 $1 \leq q \leq N$이 존재한다. $$\lVert q\alpha \rVert \leq \frac{1}{N+1}$$</greenboard>
<i>Proof.</i> 
