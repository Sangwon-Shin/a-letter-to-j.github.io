---
layout: single
title: "EMF and potential"
categories: physics
tag: [EMF, potential, faraday's law, 패러데이, 퍼텐셜]
toc: true
author_profile: false
use_math: true
---
## 한 줄 요약
알짜 전하가 없고 자기장 변화에 의해 유도되는 전기장만 있는 경우, 퍼텐셜은 모든 공간에서 같다.

## 패러데이 법칙과 퍼텐셜

고교 물리에서 패러데이의 법칙은 다음의 식으로 기술된다.

\\[ V_emf = -\frac{\Delta \Phi}{\Delta t} \\]

$V_emf$(유도 기전력)는 퍼텐셜로 오해하기 쉽다. 그러나 이 값은 퍼텐셜이 아니다. 원형 고리의 안쪽에 자기장의 변화를 주어 고리에 전류가 흐르게 하면, 퍼텐셜은 어떻게 될까? 이 유도 기전력이 퍼텐셜이라고 한다면 모순이 발생한다. 유도 기전력이 퍼텐셜이라고 가정하면, 고리 위의 한 점에서 전류 방향으로 고리를 따라 이동하면 퍼텐셜이 감소해야 한다. 그렇게 한바퀴를 돌아 왔을 때 시작점에서의 퍼텐셜과는 $V_emp$만큼 차이가 나게 된다. 결론만 말하면, 퍼텐셜은 고리 위의 모든 점에서 같다. 자기장이 시간에 따라 변하지 않을 때는 전기장에 의한 기여분만 고려하여 퍼텐셜을 구해도 된다. 고교 물리에서는 이런 경우에만 퍼텐셜을 다룬다. 하지만 자기장이 시간에 따라 변하는 경우에는 퍼텐셜을 계산할 때 자기장 변화에 의한 기여분도 고려해야 한다.
전자기장이 시간에 따라 변하는 일반적인 상황에서 미분 형태의 패러데이 법칙은 아래와 같다.($\mathbf{A}$는 벡터 퍼텐셜)

\\[ \nabla\times\mathbf{E} = -\frac{\partial\mathbf{B}}{\partial t} = -\nabla\times\frac{\partial\mathbf{A}}{\partial t} \\]
\\[ \nabla\times\left(\mathbf{E}+\frac{\partial\mathbf{A}}{\partial t}\right) \\]

그러므로 $\mathbf{E}$만으로는 시간에 불변인 퍼텐셜 $V$를 만들 수 없고 $\frac{\partial\mathbf{A}}{\partial t}$를 포함한 양이어야 퍼텐셜 $V$를 정의할 수 있다.

\\[ \mathbf{E} + \frac{\partial\mathbf{A}}{\partial t} = -\nabla V \\]

고교 물리에서 패러데이의 법칙에서의 $V_E$는 전기장의 선적분인 emf를 의미한다(Griffiths 3ed Eq.7.13). 닫힌 곡선 전체에 대한 선적분이 아니라 임의의 곡선에 대해 선적분을 해보면 다음과 같다.

\\[ \int_a^b \mathbf{E}\cdot d\mathbf{l} + \int_a^b \frac{\partial\mathbf{A}}{\partial t}\cdot d\mathbf{l} = -[V(b) - V(a)] \\]

자기장 $\mathbf{B}$가 공간적으로 균일하고 시간에 따라서는 $z$ 방향으로 커지는 상황에서의 패러데이 법칙을 생각해보자.

\\[ \mathbf{B} = kt\hat{z} \quad\to\quad \mathbf{A} = \frac{1}{2}kst\hat{\theta} \\]

$k$는 0보다 큰 상수, $s$는 원통좌표계에서의 반지름이다. 패러데이 법칙의 미분 형태를 이용해서 전기장을 계산하면 다음과 같다.

\\[ \mathbf{E} = -\frac{1}{2}ks\hat{\theta} \\]

전기장과 벡터 퍼텐셜의 방향이 반대이다. 그러므로 전기장과 벡터 퍼텐셜의 시간 미분을 원형 궤도 위의 호에 대해 선적분해보면 크기가 같고 부호가 반대가 되어 상쇄된다. 따라서 원위의 모든 지점에서 퍼텐셜 $V$값은 같다.

\\[ V(a) = V(b) \\]

## 유도 기전력의 일반적 상황: $\rho=0 \quad\to\quad \nabla\cdot\mathbf{E}=0 $

자기장의 변화에 의해서만 전기장이 유도되는 상황에서, Coulomb gauge를 적용하자. 그러면 다음이 성립한다.

\\[ \nabla\cdot\left(\mathbf{E}+\frac{\partial\mathbf{A}}{\partial t}\right) = 0 \\]

그리고 패러데이의 법칙으로부터

\\[ \nabla\times\left(\mathbf{E}+\frac{\partial\mathbf{A}}{\partial t}\right) = 0 \\]

이다. 헬름홀츠 정리에 의하면 divergence와 curl이 모두 0이고, 무한히 먼 곳에서 $1/r^2$보다 빠르게 감소하는 벡터장은 항등적으로 0이다. 그러므로

\\[ \mathbf{E}+\frac{\partial\mathbf{A}}{\partial t} = 0 \\]

이다. 그러면 자기장의 변화에 의해 유도된 전기장만 있을 때의 퍼텐셜은 모든 공간에서 일정하다.

\\[ \int_a^b\mathbf{E}\cdot d\mathbf{l} + \int_a^b\frac{\partial\mathbf{A}}{\partial t}\cdot d\mathbf{l} = 0 = -[V(b) - V(a)] \\]
\\[ \therefore~ V(a) = V(b) \\]
