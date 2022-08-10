---
layout: article
title: Olym 8N. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/number-theory/olym-8n/theorems-and-techniques/
---
# Olym 8N. 고등 정수론 I <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/number-theory/">Number Theory</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/number-theory/olym-8n/">Olym 8N</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/number-theory/olym-8n/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

## LTE

## 비에타 점핑

이번에 다룰 주제는 비에타 점핑(Vieta jumping)이다. 무한강하와 비슷한 전략으로, 최소해를 잡은 뒤 비에타 정리를 이용해 더 작은 해를 잡아 모순을 보이는 것이 일반적이다. 
<greenboard><b>Theorem 8.n.</b> $x$에 대한 이차방정식 $x^2-mx+n=0$의 해가 $x=a, b$일 때, $$a+b=m, ab=n$이 성립한다. </greenboard>

비에타 점핑은 다음 예제를 통해 알아보자. 
<skyblueboard><b>Example 8.n.</b> 양의 정수 $a, b$에 대하여 $ab+1$이 $a^2+b^2$을 나눌 때, 다음 식이 완전제곱수임을 보여라. $$\frac{a^2+b^2}{ab+1}$$</skyblueboard>
<i>Proof.</i> $k=\frac{a^2+b^2}{ab+1} \in \mathbb{Z}$라 두고, 고정된 $k$에 대해 $a+b$가 최소가 되는 양의 정수해 $(a, b)$를 잡자. $k$가 완전제곱수가 아니라고 가정하자. $k>0$임은 자명하다.

$a=b$인 경우, $k=\frac{2a^2}{a^2+1}=2-\frac{2}{a^2+1} \in \mathbb{Z}$이므로 $a=1$이 되어 $k=1$로 완전제곱수이다. 따라서 일반성을 잃지 않고 $a>b$라 두자. 

식을 변형하면 이차방정식 $a^2-kb \cdot a + (b^2-k)=0$을 얻을 수 있다. 즉, $x^2-kbx+b^2-k=0$의 한 해는 $a$이고, 다른 한 해는 $a^\prime$이라 두자. 

비에타 정리에 의해 $$a^\prime=kb-a=\frac{b^2-k}{a}$$임을 알 수 있다. $a^\prime=kb-a$로부터 $a^\prime$이 정수임은 자명하다. $k=\frac{(a^\prime)^2+b^2}{a^\prime b+1}>0$이므로 $a^\prime \geq 0$이다. $a^\prime =0$인 경우, $a^\prime =\frac{k^2-b}{a}=0$에서 $k=b^2$으로 완전제곱수가 되므로, $a^\prime>0$인 경우만 보자. 

위에서 $a>b$라 가정했으므로, $a^2>b^2-k$이고, 다시 쓰면 $$0< a^\prime = \frac{b^2-k}{a}< a$$이다. 즉, $0< a^\prime < a$임을 보였다. 

그러면 $$k=\frac{a^2+b^2}{ab+1}=\frac{(a^\prime)^2+b^2}{a^\prime b+1}$$에서 $a^\prime +b < a+b$이므로, $a+b$가 최소라는 가정에 모순이다. 

따라서 $k$는 완전제곱수이다. $\blacksquare$

## Zsigmondy's Theorem
