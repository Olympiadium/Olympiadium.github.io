---
layout: article
title: Olym 1G. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/geometry/olym-1g/theorems-and-techniques/
---
# Olym 1G. 각 돌리기 <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.homeurl }}">Olympiadium</a></li> 
	<li><a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.homeurl }}mathematical-olympiads/geometry/">Geometry</a></li> 
	<li><a href="{{ site.homeurl }}mathematical-olympiads/geometry/olym-1g/">Olym 1G</a></li> 
	<li><a href="{{ site.homeurl }}mathematical-olympiads/geometry/olym-1g/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

## 각의 표현
### 방향각(Directed Angle)
<yellowboard><b>Definition 1.1.</b> 평행하지 않은 두 직선 $\ell, m$에 대해서 방향각 $\measuredangle(\ell, m)$은 $\ell$에서 $m$까지 <span style="color:red">반시계 방향</span>으로 측정된 각도를 의미한다. </yellowboard>
<center>
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 1G/Directed Angle.svg"  width="30%">
</center>
<redborder>방향각 기호는 표준이 아니므로, 서술 시에는 정의를 해주는 것이 좋다. </redborder>

그리고, 방향각에서 한 가지 더 주목해야 할 점은 모든 각에 $\bmod 180^\circ$를 취한다는 것이다. 즉, 
<p>$$-70^\circ=110^\circ=290^\circ=\ldots$$</p>
라 할 수 있다. 

<orangeboard><b>Proposition 1.2.</b> 임의의 두 직선 $\ell, m$에 대하여 $\measuredangle(\ell, m)=-\measuredangle(m, \ell)$이다. </orangeboard>

<yellowboard><b>Definition 1.3.</b> 세 점 $A, O, B$에 대하여 $$\measuredangle AOB \overset{\rm def}= \measuredangle(\overleftrightarrow{AO}, \overleftrightarrow{BO})$$로 정의한다. </yellowboard>

<orangeboard><b>Proposition 1.4.</b> 한 평면 위 임의의 네 점 $A, B, C, P$에 대하여 다음 명제들이 성립한다. <ul class="inbox">
<li><i>Anti-Reflexivity.</i> $\measuredangle ABC = - \measuredangle CBA$. </li>
<li><i>Angle Addition.</i> $\measuredangle APB + \measuredangle BPC = \measuredangle APC$. </li>
<li><i>Triangle Sum.</i> $\measuredangle ABC + \measuredangle BCA + \measuredangle CAB = 0$. </li>
<li><i>Parallel Lines.</i> $\overline{AB} \parallel \overline{CD}$이면 $\measuredangle ABC + \measuredangle BCD =0$.</li>
<li><i>Collinearity.</i> $A, B, C$ 일직선 $\iff$ $\measuredangle PBA = \measuredangle PBC$.</li>
<li><i>Perpendicular Lines.</i> $\ell \perp m$이면 $\measuredangle (\ell, m) = \measuredangle (m, \ell) = 90^\circ$.</li>
</ul>
</orangeboard>

<redborder>방향각은 $\bmod 180^\circ$를 취했으므로, $2\measuredangle ABC = 2\measuredangle XYZ$라고 해서 양변을 2로 나눈 $\measuredangle ABC = \measuredangle XYZ$가 성립하지는 않는다. </redborder>

<!--
#### 엇각, 동위각
#### 각의 이등분선 정리
-->

## 원에서 각 돌리기
#### 원주각, 내대각
<greenboard><b>Theorem 1.5.</b> 어떠한 세 점도 한 직선 위에 놓이지 않는 네 점 $A, B, X, Y$에 대하여 $A, B, X, Y$가 공원점일 필요충분조건은 다음과 같다. $$\measuredangle XAY = \measuredangle XBY$$</greenboard>


#### 중심각, 접현각
<greenboard><b>Theorem 1.6.</b> 삼각형 $ABC$와 외심 $O$에 대하여 다음이 성립한다. $$\measuredangle AOB = 2 \measuredangle ACB$$ </greenboard>

<greenboard><b>Theorem 1.7.</b> 삼각형 $ABC$의 외심이 $O$일 때, 임의의 점 $P$에 대하여 다음 명제들이 서로 동치이다. <ul class="inbox">
	<li>$\overline{PA}$가 $(ABC)$에 접한다. </li>
	<li>$\overline{OA} \perp \overline{AP}$.</li>
	<li>$\measuredangle PAB = \measuredangle ACB$.</li>
</ul></greenboard>

### 오심에서 각 돌리기
<greenboard><b>Theorem 1.8.</b>삼각형 $ABC$의 내심을 $I$, 외심을 $O$라고 할 때, 다음이 성립한다. 
<ul class="inbox">
<li>$\angle BIC = 90^\circ + \frac{1}{2}\angle A$</li>
<li>$\angle BOC = 2 \angle A$</li>
<li>$\angle OBC = 90^\circ - \angle A$</li>
<li></li>
</ul></greenboard>

#### 수심에서 각 돌리기
<yellowboard><b>Definition 1.9.</b>삼각형 $ABC$의 세 꼭지점에서 마주보는 변에 내린 수선의 발을 각각 $D, E, F$라고 할 때, 삼각형 $DEF$는 삼각형 $ABC$의 수심삼각형(orthic triangle)이다. </yellowboard>
<greenborder>삼각형 $ABC$의 수심을 $H$라고 할 때, 다음이 성립한다.
<ul class="inbox">
<li>$(A, F, H, E), (B, D, H, F), (C, E, H, D), (A, B, D, E), (B, C, E, F), (C, A, F, D)$가 공원점</li>
<li>$H$는 삼각형 $DEF$의 내심이다. </li></ul>


#### 방심에서 각 돌리기
<greenboard><b>Theorem 1.10.</b> 삼각형 $ABC$에서 방심을 $I_A, I_B, I_C$라고 할 때, 다음이 성립한다. 
<ul class="inbox"><li>$(A, B, I_A, I_B)$가 공원점이다.</li>
<li>$(A, I_C, B, I)$가 공원점이고 $II_C$가 지름이다.</li>
<li>$I_AI_BI_C$의 수심은 $I$이다. </li>
</ul>
</greenboard>

### 멘션 정리
<greenboard><b>Theorem 1.11.</b> 삼각형 $ABC$의 내심을 $I$, 각 $A$에 대한 방심을 $I_A$라 하자. 호 $BC$의 중점을 $M$이라 할 때, $\overline{MI}=\overline{MB}=\overline{MC}=\overline{MI_A}$가 성립한다. </greenboard>


### 외심과 수심
<skyblueboard><b>Example 1.12.</b> 삼각형 $ABC$의 외심을 $O$, 수심을 $H$라고 할 때, 다음을 보여라. $$\angle BAO = \angle CAH$$</skyblueboard>

### H-Reflections
<greenboard><b>Theorem 1.13.</b> 삼각형 $ABC$의 수심을 $H$, 외심을 $O$라 하자. 이때, $H$를 변 $BC$에 대해 대칭시킨 점을 $X$, $H$를 변 $BC$의 중점 $M$에 대해 대칭시킨 점을 $Y$라 하면, $X, Y$는 삼각형 $ABC$의 외접원 위에 있고, $A, O, Y$는 일직선이다. </greenboard>

### 세르보어 정리
<greenboard><b>Theorem 1.14.</b> 삼각형 $ABC$의 수심을 $H$, 외심을 $H$라 하고, 변 $BC$의 중점을 $M$이라 할 때, $\overline{AH}=\overline{OM}$이 성립한다. </greenboard>

### 직선이 이루는 각
<greenboard><b>Theorem 1.15.</b> 평면 위의 임의의 네 직선 $a, b, c, d$에 대하여 다음이 성립한다. $$\measuredangle(a, b)+\measuredangle (c, d)=\measuredangle (a, d) + \measuredangle (c, b)$$</greenboard>

### Reim's Theorem
<greenboard><b>Theorem 1.16.</b> 원에 내접하는 사각형 $ABCD$에서 $P$와 $Q$는 각각 직선 $AB, CD$ 위의 점이다. 이때, $A, B, P, Q$가 공원점일 필요충분조건은 $\overline{CD} \parallel \overline{PQ}$이다. </greenboard>
<center>
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 1G/Reim's Theorem.svg"  width="50%">
</center>

### 심슨 정리
<greenboard><b>Theorem 1.17.</b> 삼각형 $ABC$의 외접원 위의 임의의 점 $P$에 대하여 $P$에서 변 $BC, CA, AB$에 내린 수선의 발을 각각 $X, Y, Z$라 하면 세 점 $X, Y, Z$는 한 직선 위에 있다. </greenboard>

#### 심슨 정리의 응용

### Phantom Point

## 대표 Configurations
#### Three Tangents
#### Right Angles on Incircle Chord
### Steiner-Lehmus Theorem
#### $60^\circ$ 삼각형