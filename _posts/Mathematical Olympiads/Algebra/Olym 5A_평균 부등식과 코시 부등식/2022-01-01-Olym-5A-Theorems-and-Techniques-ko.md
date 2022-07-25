---
layout: article
title: Olym 5A. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/algebra/olym-5a/theorems-and-techniques/
---
# Olym 5A. 평균 부등식과 코시 부등식 <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.baseurl }}/">Olympiadium</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/">Algebra</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/olym-5a/">Olym 5A</a></li> 
	<li><a href="{{ site.baseurl }}/mathematical-olympiads/algebra/olym-5a/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

## 산술 기하 평균 부등식
<greenboard><b>Theorem 5.1.</b> 음이 아닌 실수 $a_1, a_2, \ldots, a_n$에 대하여 다음 부등식이 성립한다. $$\frac{a_1+a_2+ \cdots + a_n}{n} \ge \sqrt[n]{a_1a_2 \cdots a_n}$$</greenboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
증명
</details></blueborder>

### 가중 산술 기하 평균 부등식
<greenboard><b>Theorem 5.2.</b> 음이 아닌 실수 $a_1, a_2, \ldots, a_n$와 양의 실수 $w_1, w_2, \ldots, w_n$에 대하여 $w=w_1+w_2+ \cdots w_n$이라 하면 다음 부등식이 성립한다. $$\frac{w_1a_1+w_2a_2+ \cdots w_na_n}{w} \ge \sqrt[w]{a_1^{w_1}a_2^{w_2} \cdots a_n^{w_n}}$$</greenboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
증명
</details></blueborder>

### 멱평균 부등식
<greenboard><b>Theorem 5.3.</b> 음이 아닌 실수 $a_1, a_2, \ldots a_n$와 $w_1+w_2+ \cdots +w_n=w$인 양의 실수 $w_1, w_2, \ldots, w_n$에 대하여 $$\mathcal{P}(r)=\begin{cases} (\frac{w_1a_1^r+w_2a_2^r+ \cdots +w_na_n^r}{w})^{1/r} \qquad &r \ne 0 \\\\ \sqrt[w]{a_1^{w_1}a_2^{w_2} \cdots a_n^{w_n}} \qquad &r=0 \end{cases}$$로 정의하자. 이때, $r>s$이면 $\mathcal{P}(r) \ge \mathcal{P}(s)$가 성립하고, 등호는 $a_1=a_2=\cdots = a_n$일 때 성립한다. </greenboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
증명
</details></blueborder>
<orangeborder><details>
<summary><b><i>Consequence</i></b></summary>
$P(1) \ge P(0)$는 가중 산술 기하 평균 부등식과 일치하고, $P(1) \ge P(0) \ge P(-1), w_1=w_2=\cdots =w_n=\frac{1}{n}$이면 산술 기하 조화 평균 부등식이 된다. 
</details></orangeborder>

### 평균 부등식의 활용

## 코시 부등식
<greenboard><b>Theorem 5.4.</b> 실수 $a_1, a_2, \ldots, a_n, b_1, b_2, \ldots, b_n$에 대하여 다음 부등식이 성립한다. $$(a_1+a_2+\cdots +a_n)(b_1+b_2+\cdots + b_n) \ge (a_1b_1+a_2b_2+\cdots +a_nb_n)^2$$</greenboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
증명
</details></blueborder>

### 코시 부등식의 응용
<orangeboard><b>Proposition 5.5(Engel Form).</b> 임의의 실수 $a_1, a_2, \ldots, a_n$과 양의 실수 $b_1, b_2, \ldots, b_n$에 대하여 다음 부등식이 성립한다. $$\frac{a_1^2}{b_1}+\frac{a_2^2}{b_2}+ \cdots +\frac{a_n^2}{b_n}$$ </orangeboard>
<orangeboard><b>Proposition 5.6(Nesbitt's Inequality). </b></orangeboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
증명
</details></blueborder>
