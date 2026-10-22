# Prior & posterior 🌱

Prior(사전분포)는 기준으로 삼는 관측을 보기 전, 드러나지 않은 [latent variable](latent-variable.md)에 대해 가진 probability distribution이다. 그 관측을 보고 난 후의 분포는 posterior(사후분포)라고 한다. 관심의 대상은 둘 다 기준으로 삼는 관측이 아니라 latent variable이다.

**예.** 주머니 두 개 중 하나를 $1/2$씩의 확률로 몰래 골라 공을 하나 꺼냈더니 빨간 공이 나왔다. 고른 주머니를 $B$, 빨간 공이 나온 것을 $R$이라 하면, prior는 특정 주머니를 고를 확률이고 posterior는 빨간 공이 나왔을 때 그 주머니를 골랐을 확률이다.

$$
\begin{aligned}
\text{prior} &= P(B) \\
\text{posterior} &= P(B \mid R)
\end{aligned}
$$
