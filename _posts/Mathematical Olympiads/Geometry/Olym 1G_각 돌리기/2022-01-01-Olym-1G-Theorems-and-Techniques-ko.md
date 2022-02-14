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
#### 내심에서 각 돌리기
<greenborder>$\angle BIC = 90^\circ + \frac{1}{2}\angle A$가 성립한다. </greenborder>

#### 외심에서 각 돌리기
<greenborder>$\angle BOC = 2 \angle A$가 성립한다. <br> $\angle BOC = 90^\circ - \angle A$가 성립한다. </greenborder>

#### 수심에서 각 돌리기
<yellowboard><b>Definition 1.n.</b>삼각형 $ABC$의 세 꼭지점에서 마주보는 변에 내린 수선의 발을 각각 $D, E, F$라고 할 때, 삼각형 $DEF$는 삼각형 $ABC$의 수심삼각형(orthic triangle)이다. </yellowboard>
<greenborder>수심으로부터 우리는 6개의 공원점을 얻을 수 있다. $$(A, F, H, E), (B, D, H, F), (C, E, H, D), (A, B, D, E), (B, C, E, F), (C, A, F, D)$$
위 공원점들은 수심에서 각을 돌릴 때 매우 유용하게 사용된다. 
</greenborder>
<skyblueborder>$H$는 삼각형 $DEF$의 내심이다. </skyblueborder>

#### 무게중심에서 각 돌리기 같은 건 없다. 

#### 방심에서 각 돌리기
<greenborder>$(A, B, I_A, I_B)$가 공원점이다. <br>
$(A, I_C, B, I)$가 공원점이고 $II_C$가 지름이다. <br>
$I_AI_BI_C$의 수심은 $I$, 수심삼각형은 $ABC$이다. 
</greenborder>


### 외심과 수심
<skyblueborder>$\angle BAO = \angle CAH$가 성립한다. </skyblueborder>

4강에서 다시 언급하겠지만, $O$와 $H$는 등각켤레점이다. 

### 세르보어 정리
<greenboard><b>Theorem 1.n.</b> $O$에서 $BC$에 내린 수선의 발을 $M$이라 하면 $AH=2OM$</greenboard>

### 멘션 정리
### 직선이 이루는 각

### Reim's Theorem
<greenboard><b>Theorem 1.n.</b> 원에 내접하는 사각형 $ABCD$에서 $P$와 $Q$는 각각 직선 $AB, CD$ 위의 점이다. 이때, $A, B, P, Q$가 공원점일 필요충분조건은 $\overline{CD} \parallel \overline{PQ}$이다. </greenboard>
<center>
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 1G/Reim's Theorem.svg"  width="50%">
</center>

### 심슨 정리

### Phantom Point

## 대표 Configurations
#### Three Tangents
#### Right Angles on Incircle Chord
### Steiner-Lehmus Theorem
#### $60^\circ 삼각형
