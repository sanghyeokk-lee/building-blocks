# Reparameterization trick 🌱

Reparameterization trick(재매개변수화 트릭)은 sampling 과정으로는 gradient가 흐르지 않아 encoder까지 gradient가 가지 못하는 문제를 풀기 위해, 먼저 $\epsilon$을 정규분포에서 sampling한 다음 평균과 $\text{std} \cdot \epsilon$을 통해 gradient가 흐르도록 하는 방법이다.

**예.** VAE의 encoder가 평균 $\mu$와 표준편차 $\sigma$를 내면, $z$를 $q_\phi(z \mid x)$에서 바로 sampling하지 않고 아래처럼 만든다. $\odot$은 원소별 곱이다.

$$
\begin{aligned}
\epsilon &\sim \mathcal{N}(0, I) \\
z &= \mu + \sigma \odot \epsilon
\end{aligned}
$$
