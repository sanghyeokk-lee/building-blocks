# Likelihood 🌱

Likelihood(우도)는 관측된 데이터를 고정한 채, parameter 값마다 그 parameter일 때 이 데이터가 나올 확률(또는 probability density)을 매긴 점수다. 이 점수를 가장 크게 만드는 parameter가 데이터를 가장 잘 설명하는 parameter다.

**예.** 동전을 10번 던져 앞면 7번, 뒷면 3번이 어떤 순서로 나왔다. 앞면이 나올 확률을 $\theta$라 하면, 바로 그 순서가 나올 확률은 $\theta$의 함수다.

$$
L(\theta) = \theta^7 (1 - \theta)^3
$$

| $\theta$ | 0.5 | 0.7 | 0.9 |
|---|---|---|---|
| $L(\theta)$ | 0.00098 | 0.00222 | 0.00048 |

$L(\theta)$는 $\theta = 0.7$에서 가장 크다. 한편 $L(\theta)$를 $\theta$에 대해 0부터 1까지 적분하면 약 0.00076이어서, likelihood는 $\theta$의 probability distribution이 아니다.
