---
layout: article
title: Olym 7G. 이론 및 기술 | Olympiadium
date: 2022-01-01
mathjax: true
lang: ko
permalink: /mathematical-olympiads/geometry/olym-7g/theorems-and-techniques/
---
# Olym 7G. 사영 기하학 <br> <ssup> - 이론 및 기술</ssup>

<ul class="breadcrumb">
	<li><a href="{{ site.url }}">Olympiadium</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/">Mathematical Olympiads</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/geometry/">Geometry</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/geometry/olym-7g/">Olym 7G</a></li> 
	<li><a href="{{ site.url }}mathematical-olympiads/geometry/olym-7g/theorems-and-techniques/">이론 및 기술</a></li>
</ul>

## 조화점열
### 비조화비 Cross Ratios
<yellowboard><b>Definition 10.1. </b>한 직선 위에 네 점 $A, B, X, DY$가 주어졌을 때, $A, B, X, Y$의 <span style="color:blue"><b>비조화비(cross Ratio)</b></span>를 다음과 같이 정의한다: $$(A, B; X, Y)=\frac{XA/XB}{YA/YB}$$ (단, 여기서 선분비는 방향을 가진다. <a href="https://example.com"> 참고</a>) <br>
한 점에서 만나는 네 직선 $a, b, x, y$에 대해서도 $$(a, b; x, y)=\pm \frac{\sin \angle(x, a) / \sin \angle(x, b)}{\sin \angle(y, a) / \sin \angle(y, b)}$$
한 직선 위의 점 $A, B, X, Y$가 각각 한 점 $P$에서 만나는 네 직선 $a, b, x, y$ 위에 있을 때, $$P(A, B; X, Y)=(a, b; x, y)$$</yellowboard>
<i>Diagram.</i>
<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 7G/비조화비.png"  width="60%">
</p>
여기서 $P(A, B; X, Y)$를 <span style="color:blue"><b>선다발(pencil of lines)</b></span>이라고 한다. 
<redborder> <b>비조화비의 부호</b> <br> $(A, B; X, Y)>0 \iff \overline{AB}, \overline{XY}$가 만나지 않거나 한 선분이 다른 선분을 포함함. <br>
  $(a, b; x, y)>0 \iff a$와 $b$로 이루어진 각에 $x$와 $y$가 모두 포함되거나 모두 포함되지 않음. </redborder>

<greenboard><b>Lemma 10.2. </b> $P(A, B; X, Y)$가 pencil of lines이고 $A, B, X, Y$가 한 직선 위에 있으면, $$P(A, B; X, Y)=(A, B; X, Y)$$가 성립한다. </greenboard>
<blueborder><details>
<summary><b><i>Proof</i></b></summary>
우리가 증명해야 하는 것은 $$\frac{\sin \angle(x, a) / \sin \angle(x, b)}{\sin \angle(y, a) / \sin \angle(y, b)}=\frac{XA/XB}{YA/YB}$$와 같다. 삼각형의 넓이 비를 이용하자. 
\begin{align*} \frac{XA/XB}{YA/YB}&=\frac{\triangle XPA / \triangle XPB}{\triangle YPA / \triangle YPB} \\ &=\frac{PX \cdot PA \cdot \sin \angle(x, a) / PX \cdot PB \cdot \sin \angle(x, b)}{PY \cdot PA \cdot \sin \angle(y, a) / PY \cdot PB \cdot \sin \angle(y, a)} \\ &=\frac{\sin \angle(x, a) / \sin \angle(x, b)}{\sin \angle(y, a) / \sin \angle(y, b)} \end{align*} $\blacksquare$
</details></blueborder>
<redborder> 위 Lemma는 $A, B, X, Y, P$가 한 원 위에 있을 때에도 적용할 수 있다. </redborder>
<yellowboard> <b>Proposition 10.3. </b> 아래 두 그림에서
<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 7G/비조화비2.png"  width="49%">
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 7G/비조화비3.png"  width="49%">
</p>
$(A, B; X, Y) = P(A, B; X, Y)=P(A', B'; X', Y')=(A', B'; X', Y')$가 성립하는데, 이를 <span style="color:blue">taking perspectivity at $P$</span>라고 부르며, $$(A, B; X, Y) \overset{P}{=} (A', B'; X', Y')$$로 표기한다. </yellowboard>
<orangeborder><details>
<summary><b><i>Extra. </i></b></summary>
    Coming Soon!
</details></orangeborder>
<orangeboard><b>Proposition 10.4. </b> 임의의 네 점 $A, B, C, D$에 대하여 $$(A, B; X, Y)=(B, A; X, Y)^{-1}=(A, B; Y, X)^{-1}=(X, Y; A, B)$$ 가 성립한다. <br>
    한 직선 상에 서로 다른 세 점 $A, B, X$와 실수 $k$가 주어졌을 때, $(A, B; X, Y)=k$가 되는 점 $Y$가 유일하게 존재함을 보여라. <br>
    $(A, B; X, Y)=1 \iff$ $A$와 $B$가 일치하거나 $X$와 $Y$가 일치한다. </orangeboard>
    
### 조화점열의 정의와 성질
<yellowboard><b>Definition 10.5. </b> $(A, B; X, Y)=-1$을 만족할 때, $(A, B; X, Y)$를 <span style="color:blue">조화점열(harmonic bundle)</span>이라고 하며, <br>
    사각형 $AXBY$가 원에 내접하면 이를 <span style="color:blue">조화사각형(harmonic quadrilateral)</span>이라 한다. <br>
    $(A, B; X, Y)=-1 \implies (A, B; Y, X)=(B, A; X, Y)=-1$이므로 점 $Y$를 $\overline{AB}$에 대한 점 $X$의 <span style="color:blue">harmonic conjugate</span>이라 정의한다. </yellowboard>
<greenboard><b>Lemma 10.6. </b> </greenboard>

## Pole and Polar
### La-Hire's Theorem
### 7점 공선
<greenboard> 원에 내접하는 사각형 $ABCD$에 대해 점들을 다음과 같이 정의하자. 
  
$P_1$은 직선 $AD$와 $BC$의 교점, $P_2$는 점 $A$와 $B$에서 그은 접선의 교점, $P_4$는 선분 $AC$와 $BD$의 교점, $P_5$는 $(ADP_4)$와 $(BCP_4)$의 $P_4$가 아닌 교점, $P_7$은 점 $C$와 $D$에서 그은 접선의 교점. $X$는 직선 $AB$와 $CD$의 교점, $P_3$와 $P_6$는 각각 점 $X$에서 원에 그은 접선의 접점.

이때, 7개의 점 $P_1, P_2, P_3, P_4, P_5, P_6, P_7$이 한 직선 위에 있다. </greenboard>

<i>Diagram.</i> 
<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 7G/칠점공선.png"  width="80%">
</p>

<blueborder><details>
<summary><b><i>Proof</i></b></summary>
<i>Diagram.</i> 
<p align="center">
    <img src="{{ site.url }}{{ site.baseurl }}/images/posts/Olym 7G/칠점공선 증명.png"  width="95%">
</p>
<orangeboard><i>Step1.</i> $P_1, P_2, P_4, P_7$가 일직선</orangeboard>
$AACBBD$에서 파스칼 정리에 의해 $P_1, P_2, P_4$가 일직선, $ACCBDD$에서 파스칼 정리에 의해 $P_1, P_4, P_7$가 일직선.
이 두 사실에 의해 $P_1, P_2, P_4, P_7$가 일직선. $\blacksquare$
<orangeboard><i>Step2.</i> $P_1, P_4, P_5$가 일직선 </orangeboard>
$(ADP_4), (ABCD), (BCP_4)$에서 근축 $AD, BC, P_4P_5$는 한 점 $P_1$에서 만난다. 따라서 $P_1, P_4, P_5$가 일직선. $\blacksquare$
<orangeboard><i>Step3.</i> $(AP_2BP_5O)$가 공원점, $(CP_5ODP_7)$가 공원점 </orangeboard>
$$\angle AP_5B = \angle AP_5P_4 + \angle BP_5P_4 = \angle ADB + \angle ACB = 2\angle ADB = \angle AOB$$
또한, $AP_2, BP_2$가 접선이므로, $$\angle P_2AO = \angle P_2BO = 90^\circ$$ 따라서 $(AP_2BP_5O)$가 공원점. 같은 방법으로, $(CP_5ODP_7)$도 공원점. $\blacksquare$
<orangeboard><i>Step4.</i> $X, P_5, O$가 일직선 </orangeboard>
$(ABP_5O), (CDOP_5), (ABCD)$에서 근축 $AB, CD, OP_5$는 한 점 $X$에서 만난다. 따라서 $X, P_5, O$가 일직선. $\blacksquare$
<orangeboard><i>Step5.</i> $P_3, P_5, P_6$ 일직선 </orangeboard>
방멱 정리에 의해 $$XO \times XP_5 = XA \times XB = XP_3^2$$ 따라서 $\triangle XP_3O \sim \triangle P_3P_5O$<br>
$XP_3$가 접선이므로 $$\angle OP_5P_3 = \angle OP_3X = 90^\circ$$ 같은 방법으로 $\angle OP_5P_6 = 90^\circ$도 보일 수 있다. 
  
따라서 $\angle P_3P_5P_6 = 180^\circ$이므로, $P_3, P_5, P_6$는 일직선. $\blacksquare$<br><br>

Step 1~5의 사실을 종합하면 $P_1, P_2, P_3, P_4, P_5, P_6, P_7$이 한 직선 위에 있다는 것이 증명된다. 
</details></blueborder>
