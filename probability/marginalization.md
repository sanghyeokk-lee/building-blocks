# Marginalization 🌿

Marginalization(주변화)은 joint distribution에서 관심 없는 변수가 가질 수 있는 모든 값에 대해 확률을 더해(연속이면 적분해) 그 변수를 없애는 것이다. Latent variable이 있는 모델에서는, latent variable을 거쳐 관측값에 이르는 모든 경로의 확률을 더하는 것과 같다.

**예.** 공정한 동전과 앞면이 0.9의 확률로 나오는 동전 중 하나를 각각 $1/2$의 확률로 몰래 골라 던진다. 고른 동전 $C$를 모르므로, 두 경우를 모두 더해 앞면 $H$가 나올 확률을 구한다.

$$
P(H) = \sum_{c} P(H,\ C = c) = 0.5 \times 0.5 + 0.5 \times 0.9 = 0.7
$$

**왜.** [Random variable](random-variable.md)은 outcome마다 값을 하나만 주는 함수다. 그래서 $y$가 다르면 $Y = y$인 경우들은 서로 겹치지 않고, 모든 $y$를 모으면 빠지는 outcome이 없다. 따라서 $P(X = x,\ Y = y)$를 모든 $y$에 대해 더하면, $X = x$인 outcome을 빠짐없이 한 번씩 센 것이 되어 $P(X = x)$가 된다.

$$
P(X = x) = \sum_{y} P(X = x,\ Y = y)
$$

**반례.** '$P(X = x \mid Y = y)$를 모든 $y$에 대해 더하면 $P(X = x)$다'라는 주장은 틀렸다. 위의 예에서 동전마다 앞면이 나올 conditional probability를 더하면 1을 넘으므로 확률이 될 수 없다. 동전을 고를 확률이 빠졌기 때문이다. 더하는 것은 고를 확률까지 담긴 joint probability여야 한다.

$$
\begin{aligned}
\sum_{c} P(H \mid C = c) &= 0.5 + 0.9 = 1.4 \\
\sum_{c} P(H,\ C = c) &= 0.25 + 0.45 = 0.7
\end{aligned}
$$
