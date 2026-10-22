# Generative process 🌱

Generative process(생성 과정)는 변수들이 나오는 순서를 정하고, 그 순서대로 각 변수를 그보다 먼저 나온 변수를 조건으로 하는 probability distribution에서 sampling하는 과정이다.

**예.** 주머니를 먼저 고른 다음, 그 주머니에서 공을 꺼낸다. 고른 주머니를 $B$, 꺼낸 공의 색을 $R$이라 하면, $P(B)$에서 주머니를 sampling하고 $P(R \mid B)$에서 공의 색을 sampling한다.

$$
\begin{aligned}
b &\sim P(B) \\
r &\sim P(R \mid B = b)
\end{aligned}
$$

그래서 joint distribution도 이 순서대로 쪼개진다.

$$
P(B, R) = P(R \mid B)\, P(B)
$$
