# Expectation 🌱

Expectation(기댓값)은 어떤 함수 $f$에 대해서든, 그 값을 확률분포로 가중해 평균 낸 것이다. 그 함수가 확률변수 자체일 때의 기댓값 $\mathbb{E}[X]$를 mean(평균)이라 한다.

$$
\mathbb{E}_{p(x)}[f(x)] = \sum_{x} p(x)\, f(x)
$$

**예.** 앞면이 나오면 1, 뒷면이 나오면 0인 동전이 있고, 앞면이 나올 확률은 0.7이다. 이 값의 기댓값은 0.7이다. 동전을 10번 던져 앞면이 6번 나왔다면 sample mean $\bar{x}$는 0.6으로, 기댓값과 다르다.

$$
\begin{aligned}
\mathbb{E}[X] &= 1 \times 0.7 + 0 \times 0.3 = 0.7 \\
\bar{x} &= \frac{6}{10} = 0.6
\end{aligned}
$$
