# Conditional probability 🌿

Conditional probability(조건부 확률)는 조건 $x$가 주어졌을 때 $y$가 나올 확률, 또는 그때 $y$가 따르는 probability distribution이다.

**예.** 주사위를 던졌는데, 먼저 본 친구가 짝수라고 알려 주었다. 주사위의 눈을 $Y$, 짝수인지 홀수인지를 $X$라 하면, 6이 나왔을 확률은 conditional probability로 구하면 다음과 같다.

$$
P(Y = 6 \mid X = \text{짝수}) = \frac{P(Y = 6,\ X = \text{짝수})}{P(X = \text{짝수})} = \frac{1/6}{1/2} = \frac{1}{3}
$$

**왜.** $X = x$라는 것을 알면 가능한 outcome이 $X = x$인 것들로 줄어들고, conditional probability는 그 안에서 $Y = y$인 것이 차지하는 비율이다. 그래서 줄어든 범위 전체의 확률 $P(X = x)$로 나눈다. 이렇게 나누면 줄어든 범위 안의 확률을 모두 더한 값이 다시 1이 된다. 0으로는 나눌 수 없으므로 이 식은 $P(X = x) > 0$일 때만 쓸 수 있다.

$$
\sum_{y} P(Y = y \mid X = x) = \frac{\sum_{y} P(Y = y,\ X = x)}{P(X = x)} = \frac{P(X = x)}{P(X = x)} = 1
$$

두 번째 등호에서 [Marginalization](marginalization.md)을 썼다.

**반례.** '$P(Y \mid X) = P(X \mid Y)$'라는 주장은 틀렸다. 트럼프 카드 52장에서 한 장을 뽑을 때, 빨간색이라는 조건에서 하트일 확률은 $1/2$이지만 하트라는 조건에서 빨간색일 확률은 $1$이다. 분자 $P(\text{하트},\ \text{빨강}) = 1/4$는 같고, 무엇으로 나누느냐(조건)만 다르다.

$$
\begin{aligned}
P(\text{하트} \mid \text{빨강}) &= \frac{1/4}{1/2} = \frac{1}{2} \\
P(\text{빨강} \mid \text{하트}) &= \frac{1/4}{1/4} = 1
\end{aligned}
$$
