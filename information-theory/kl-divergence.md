# KL divergence 🌱

KL divergence(KL 발산)는 두 분포의 차이를 정량화한 것이다. [cross-entropy](cross-entropy.md)에서 [entropy](entropy.md)를 빼서 구한다.

$$
\mathrm{KL}(q \Vert p) = H(q, p) - H(q)
$$

**예.** $p$와 $q$가 같으면 $H(q, p) = H(q, q) = H(q)$가 되므로 KL은 0이 된다.

$$
\mathrm{KL}(q \Vert q) = H(q) - H(q) = 0
$$
