# Marginalization 🌱

Marginalization(주변화)은 joint distribution에서 관심 없는 변수가 가질 수 있는 모든 값에 대해 확률을 더해(연속이면 적분해) 그 변수를 없애는 것이다. Latent variable이 있는 모델에서는, latent variable을 거쳐 관측값에 이르는 모든 경로의 확률을 더하는 것과 같다.

**예.** 공정한 동전과 앞면이 0.9의 확률로 나오는 동전 중 하나를 각각 $1/2$의 확률로 몰래 골라 던진다. 고른 동전 $C$를 모르므로, 두 경우를 모두 더해 앞면 $H$가 나올 확률을 구한다.

$$
P(H) = \sum_{c} P(H,\ C = c) = 0.5 \times 0.5 + 0.5 \times 0.9 = 0.7
$$
