---
layout: article
title: Olym 1G. 이론 및 기술 | Olympiadium
date: 2021-09-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/geometry/olym-1g/theorems-and-techniques/
---
# Olym 1G. 각 돌리기 <br> <ssup> - 이론 및 기술</ssup>

<a href="{{ site.homeurl }}">Olympiadium</a> > <a href="{{ site.homeurl }}mathematical-olympiads/">Mathematical Olympiads</a> > <a href="{{ site.homeurl }}mathematical-olympiads/geometry/">Geometry</a> > <a href="{{ site.homeurl }}mathematical-olympiads/geometry/olym-1g/">Olym 1G</a> > <a href="{{ site.homeurl }}mathematical-olympiads/geometry/olym-1g/theorems-and-techniques/">이론 및 기술</a>

## 각의 표현
### 방향각(Directed Angle)
<yellowboard><b>Definition 1.1.</b> 평행하지 않은 두 직선 $l, m$에 대해서 방향각 $\measuredangle(l, m)$은 $l$에서 $m$까지 <span style="color:red">반시계 방향</span>으로 측정된 각도를 의미한다. </yellowboard>
<redborder>방향각 기호는 표준이 아니므로, 서술 시에는 정의를 해주는 것이 좋다. </redborder>

그리고, 방향각에서 한 가지 더 주목해야 할 점은 모든 각에 $\bmod 180^\circ$를 취한다는 것이다. 즉, 
<p>$$-79^\circ=110^\circ=290^\circ=\ldots$$</p>
라 할 수 있다. 

<orangeboard><b>Proposition 1.2.</b> 임의의 두 직선 $l, m$에 대하여 $\measuredangle(l, m)=-\measuredangle(m, l)$이다. </orangeboard>

<yellowboard><b>Definition 1.3.</b> 세 점 $A, O, B$에 대하여 $$\measuredangle AOB \overset{\rm def}= \measuredangle(\overleftrightarrow{AO}, \overleftrightarrow{BO})$$로 정의한다. </yellowboard>

<orangeboard><b>Proposition 1.4.</b> 한 평면 위 임의의 네 점 $A, B, C, P$에 대하여 다음 명제들이 성립한다. <ul class="inbox">
<li><i>Anti-Reflexivity.</i> $\measuredangle ABC = - \measuredangle CBA$. </li>
<li><i>Angle Addition.</i> $\measuredangle APB + \measuredangle BPC = \measuredangle APC$. </li>
<li><i>Triangle Sum.</i> $\measuredangle ABC + \measuredangle BCA + \measuredangle CAB = 0$. </li>
<li><i>Parallel Lines.</i> $\overline{AB} \parallel \overline{CD}$이면 $\measuredangle ABC + \measuredangle BCD =0$.</li>
<li><i>Collinearity.</i> $A, B, C$ 일직선 $\iff$ $\measuredangle PBA = \measuredangle PBC$.</li>
<li><i>Perpendicular Lines.</i> $l \perp m$이면 $\measuredangle (l, m) = \measuredangle (m, l) = 90^\circ$.</li>
</ul>
</orangeboard>

<redborder>방향각은 $\bmod 180^\circ$를 취했으므로, $2\measuredangle ABC = 2\measuredangle XYZ$라고 해서 양변을 2로 나눈 $\measuredangle ABC = \measuredangle XYZ$가 성립하지는 않는다. </redborder>

#### 엇각, 동위각
#### 각의 이등분선 정리

## 원에서 각 돌리기
#### 원주각, 내대각
<greenboard><b>Theorem 1.5.</b> 어떠한 세 점도 한 직선 위에 놓이지 않는 네 점 $A, B, X, Y$에 대하여 $A, B, X, Y$가 공원점일 필요충분조건은 다음과 같다. $$\measuredangle XAY = \measuredangle XBY$$</greenboard>
#### 중심각, 접현각
<greenboard><b>Theorem 1.6.</b> 삼각형 $ABC$와 외심 $O$에 대하여 다음이 성립한다. $$\measuredangle AOB = \measuredangle ACB$$ </greenboard>
<greenboard><b>Theorem 1.7.</b> 삼각형 $ABC$의 외심이 $O$일 때, 임의의 점 $P$에 대하여 다음 명제들이 서로 동치이다. <ul class="inbox">
	<li>$\overline{PA}$가 $(ABC)$에 접한다. </li>
	<li>$\overline{OA} \perp \overline{AP}$.</li>
	<li>$\measuredangle PAB = \measuredangle ACB$.</li>
</ul></greenboard>

### 오심에서 각 돌리기
#### 내심에서 각 돌리기
#### 외심에서 각 돌리기
#### 수심에서 각 돌리기
수심 공원점
#### 무게중심에서 각 돌리기
#### 방심에서 각 돌리기

### 외심과 수심
### 세르보어 정리와 H-reflections

### 멘션 정리
### 직선이 이루는 각

### Reim's Theorem
<greenboard><b>Theorem 1.n.</b> 원에 내접하는 사각형 $ABCD$에서 $P$와 $Q$는 각각 직선 $AB, CD$ 위의 점이다. 이때, $A, B, P, Q$가 공원점일 필요충분조건은 $\overline{CD} \parallel \overline{PQ}$이다. 
### 심슨 정리

## 대표 Configurations
#### Three Tangents
#### Right Angles on Incircle Chord
### Steiner-Lehmus Theorem