---
layout: article
title: Card Game Application | Olympiadium
date: 2021-09-13
mathjax: true
permalink: card-game-application/
---
# 카드 문제의 응용

## Problem
<blueboard>$n$은 자연수이고, 두 학생 $A$와 $B$가 $1$부터 $2n$까지 숫자가 적힌 $2n$장의 카드를 가지고 다음 규칙에 따라 게임을 한다.<br><br>
$2n$장의 카드를 섞어 두 명의 학생에게 임의로 $n$장씩 나누어 준다. $A$부터 시작해 두 학생은 번갈아 가며 자신의 카드를 한 장씩 낸다. 두 학생이 낸 카드에 적힌 모든 숫자의 합이 $2n + 1$의 배수가 될 때, 이 게임은 끝나고, 마지막에 카드를 낸 학생이 승리한다.<br><br>
이때, 이 게임의 필승전략은 누구에게 존재하는가? </blueboard>
[AoPS Link](https://artofproblemsolving.com/community/c6h2507072p21197246){:target="blank"}

<purpleborder><details>
<summary><b>Hint 1</b></summary>
쉽게 예상할 수 있겠지만, 필승전략은 $B$에게 있다. 
</details></purpleborder>

<purpleborder><details>
<summary><b>Hint 2</b></summary>
$A$가 이기지 못하도록 하는 카드를 $B$가 항상 가지고 있음을 보이면 된다.
</details></purpleborder>

<purpleborder><details>
<summary><b>Hint 3</b></summary>
$\bmod (2n+1)$에서 생각을 한다. 
</details></purpleborder>

<purpleborder><details>
<summary><b>Hint 4</b></summary>
$B$가 카드를 내는 순간 $B$가 가지고 있는 카드의 수는 $A$가 가지고 있는 카드의 수보다 $1$개 더 많다. 
</details></purpleborder>

<pinkborder><details>
<summary><b>Solution</b></summary>
필승전략을 $\boxed{B}$에게 있다. 
이제, $A$가 이기지 못하게 하는 카드를 $B$가 항상 가지고 있음을 보이자. <br>
$A$와 $B$가 가지고 있는 카드에 적힌 모든 숫자들은 서로 다르고, $B$가 카드를 내는 차례에, $B$는 $A$보다 카드를 한 장 더 가지고 있다. <br>
$B$ 차례에, $A$가 가지고 있는 카드에 적힌 수들이 $a_1, a_2, \ldots, a_k$이면, $B$가 카드를 냈을 때 $\bmod 2n+1$에서 $-a_1, -a_2, \ldots, -a_k$가 되지 않도록 해야 한다. <br>
$B$는 $A$보다 카드가 한 장 많으므로, $b_1, b_2, \ldots, b_k, b_{k+1}$을 가지고 있다면, 현재까지 낸 모든 숫자의 합을 $s$라 할 때, <br>
$B$는 자신의 차례에 $s+b_1, s+b_2, \ldots, s+b_{k+1}$를 만들 수 있고, 이들은 $\bmod 2n+1$에서 서로 다르다. <br>
즉, $B$가 만들 수 있는 합은 $k+1$가지이고, 만들지 말아야 할 합은 $k$가지 이다. 따라서, 만들지 말아야 할 합을 만들지 않을 수 있다. <br>
$1$부터 $2n$까지의 모든 자연수의 합은 $n(2n+1)$로, $(2n+1)$의 배수이므로, 중간에 승부가 나지 않을 경우, 마지막 카드를 내는 $B$가 결국 승리를 하게 된다. 
</details></pinkborder>
