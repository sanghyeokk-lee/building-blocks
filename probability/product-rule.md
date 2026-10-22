# Product rule 🌱

Product rule(곱셈정리)은 joint probability를 한 변수의 확률과, 그 변수가 주어졌을 때 다른 변수의 conditional probability의 곱으로 나타내는 규칙이다. [Conditional probability](conditional-probability.md)의 정의에서 바로 유도되고, 두 변수의 자리를 바꿔도 성립한다.

$$
\begin{aligned}
P(X, Y) &= P(Y \mid X)\, P(X) \\
&= P(X \mid Y)\, P(Y)
\end{aligned}
$$

**예.** 주사위의 눈을 $Y$, 짝수인지 홀수인지를 $X$라 하면, 6이 나오면서 짝수일 확률은 두 순서 중 어느 쪽으로 쪼개도 같다.

$$
\begin{aligned}
P(Y = 6,\ X = \text{짝수}) &= P(Y = 6 \mid X = \text{짝수})\, P(X = \text{짝수}) = \frac{1}{3} \times \frac{1}{2} = \frac{1}{6} \\
P(Y = 6,\ X = \text{짝수}) &= P(X = \text{짝수} \mid Y = 6)\, P(Y = 6) = 1 \times \frac{1}{6} = \frac{1}{6}
\end{aligned}
$$
