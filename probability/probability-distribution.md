# Probability distribution 🌱

Probability distribution(확률분포)은 random variable이 가질 수 있는 값에 수를 매기는 규칙이다. Random variable이 이산이면 그 수는 값마다의 확률이고, 연속이면 probability density(확률밀도)다. 연속일 때는 값 하나가 나올 확률이 0이므로, 확률은 probability density를 구간에서 적분해서 얻는다.

**예.** 공정한 주사위의 눈을 random variable $X$라 하면, $X$는 1부터 6까지의 이산값을 가지고 각 값의 확률은 모두 같다.

$$
P(X = k) = \frac{1}{6} \qquad (k = 1, 2, \dots, 6)
$$

대한민국 남성의 키를 random variable $H$라 하면 $H$는 연속값을 가지므로, 키가 정확히 180cm일 확률 $P(H = 180)$은 0이다. 대신 178cm에서 182cm 사이일 확률은 probability density $p(h)$를 그 구간에서 적분해서 구한다.

$$
P(178 \le H \le 182) = \int_{178}^{182} p(h)\, dh
$$
