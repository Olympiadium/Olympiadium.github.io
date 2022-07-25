---
layout: article
title: Olym 5N. 연습문제 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/number-theory/olym-5n/exercise-problems/
---
# Olym 5N. 이차잉여와 원시근 <br> <ssup> - 연습문제</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.url }}">Olympiadium</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/number-theory/">Number Theory</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/number-theory/olym-5n/">Olym 5N</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/number-theory/olym-5n/exercise-problems/">연습문제</a></li>
</ul>

### Example n. Title Here
<skyblueboard> Problem Here </skyblueboard>
[Source Here](Link Here){:target="blank"}
<pinkborder><details>
<summary><b>Solution</b></summary>
Solution Here. 
</details></pinkborder>

### Exercise n. A Great Exercise For Orders
<skyblueboard> 다음 조건을 모두 만족하는 소수의 순서쌍 $(p, q, r)$을 모두 구하여라. $$p \mid q^r+1, \ q \mid r^p+1, \ r \mid p^q+1$$ </skyblueboard>
[USA TST 2003/3](https://artofproblemsolving.com/community/c6h58445p357351){:target="blank"}
<purpleborder><details>
<summary><b>Walkthrough</b></summary>
<purpleborder><details>
<summary><b>Part (a)</b></summary>
$p, q, r$ 중 같은 두 수가 존재하는 경우와, $p, q, r$ 중 $2$가 존재하는 경우를 먼저 살펴본다. <ssbr/>
일반성을 잃지 않고 $p, q, r$ 중 $p$가 최소라고 할 수 있다. 
</details></purpleborder>
<purpleborder><details>
<summary><b>Part (b)</b></summary>
$q^r \equiv -1 \pmod{p}$에서 $q^{2r} \equiv 1 \pmod{p}$이므로, $$\mathrm{ord}_q(p) \mid 2r$$를 얻는다. 
</details></purpleborder>
<purpleborder><details>
<summary><b>Part (c)</b></summary>
Hint Here. 
</details></purpleborder>
</details></purpleborder>
<pinkborder><details>
<summary><b>Solution</b></summary>
우선, $p, q, r$ 중 같은 두 수가 존재하는 경우, $p=q$이면 $p \mid p^r+1 \implies p \mid 1$ 가 되어 모순이다. <ssbr/>

먼저, $p, q, r$이 모두 홀수인 경우를 보자. 
$q^r \equiv -1 \pmod{p}$에서 $q^{2r} \equiv 1 \pmod{p}$이므로, $$\mathrm{ord}_q(p) \mid 2r$$을 얻는다. 
$r$은 소수이므로, $\mathrm{ord}_q(p) = 1, 2, r, 2r$이 되고, 각 경우를 살펴보자. <ssbr/>

<ul>
  <li> $\mathrm{ord}_q(p)=1$인 경우: $q \equiv 1 \pmod{p}, \ q^r \equiv 1 \equiv -1 \pmod{p}$에서 $p=2$로 가정에 모순이다.  <ssbr/></li>
  <li> $\mathrm{ord}_q(p)=r$인 경우: $q^r \equiv 1 \equiv -1 \pmod{p}$에서 $p=2$로 가정에 모순이다. <ssbr/></li>
  <li> $\mathrm{ord}_q(p)=2r$인 경우: $2r \mid p-1 \implies r \mid p-1$.<br> 따라서, $p \equiv 1 \pmod{r}$이고, $p^q \equiv -1 \pmod{r}$에 대입하면 $1 \equiv -1 \pmod{r} \implies r=2$로 가정에 모순이다. <ssbr/></li>
  <li> $\mathrm{ord}_q(p)=2$인 경우: $q^2 \equiv 1 \pmod{p}$에서 $p \mid q^2-1 = (q-1)(q+1) \implies p \mid q+1$.<br> 같은 방법으로, $\mathrm{ord}_p(r)=2, \mathrm{ord}_r(q)=2$이고, $q \mid r+1, r \mid p+1$까지 얻을 수 있다.<br> $p, q, r$이 홀수이므로, $p \mid \frac{q+1}{2}, q \mid \frac{r+1}{2}, r \mid \frac{p+1}{2}$인데, 크기비교를 통해 $$p \le \frac{q+1}{2} \le \frac{r+3}{4} \le \frac{p+7}{8}$$가 되어, $p \le 1$로 모순이다. <ssbr/></li>
</ul>
따라서 $p, q, r$이 홀수인 경우는 해가 없다. <ssbr/>

이제 $p, q, r$ 중 2가 있는 경우를 살펴보면, (일반성을 잃지 않고 $p=2; q, r>2$라 가정하자.) <br>
문제 조건은 $q \mid r^2+1, r \mid 2^q+1$로 쓸 수 있고, $2^q \equiv -1 \pmod{r}$에서 $\mathrm{ord}_2(r)=1, 2, r, 2r$이 된다. <br>
<ul>
  <li> $\mathrm{ord}_2(r)=1$인 경우: $2 \equiv 1 \pmod{r}$에서 $r=1$이 되어 모순이다. <ssbr/></li>
  <li> $\mathrm{ord}_2(r)=2$인 경우: $4 \equiv 1 \pmod{r}$에서 $r=3$이고, $q \mid r^2+1=10$에서 $q=5$. 따라서 순서쌍 $(p, q, r)=(2, 5, 3)$이 조건을 만족한다. <ssbr/></li>
  <li> $\mathrm{ord}_2(r)=q$인 경우: $2^q \equiv 1 \equiv -1 \pmod{r}$에서 $r=2$가 되어 모순이다. <ssbr/></li>
  <li> $\mathrm{ord}_2(r)=2q$인 경우: $2q \mid r-1 \implies q \mid r-1 \implies r^2 \equiv 1 \equiv -1 \pmod{q}$에서 $q=2$가 되어 모순이다. <ssbr/></li>
</ul>
따라서 $(p, q, r)=(2, 5, 3)$은 조건에 대입시 성립하고, 같은 방법으로 $q=2$와 $r=2$인 경우 $(p, q, r)=(3, 2, 5), (5, 3, 2)$를 얻어, 답은 $\boxed{(p, q, r)=(2, 5, 3), (3, 2, 5), (5, 3, 2)}$가 된다. 
</details></pinkborder>
