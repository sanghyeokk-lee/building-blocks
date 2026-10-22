# Variational posterior 🌱

Variational posterior(변분 사후분포)는 계산할 수 없는 진짜 posterior $p_\theta(z \mid x)$ 대신, 이를 추측하기 위해 우리가 직접 정한 분포 $q_\phi(z \mid x)$다. 우리가 정한 것이기 때문에 계산이 가능하고, parameter $\phi$를 조정하여 진짜 posterior에 가깝게 맞출 수 있다.

**예.** 공정한 동전과 앞면 확률 0.9인 동전 중 하나를 $1/2$씩의 확률로 몰래 골라 던졌더니 앞면 $H$가 나왔다. 어느 동전이었을지에 대한 추측을 "치우친 동전일 확률은 $\phi$"로 정하면 이것이 variational posterior다. 진짜 posterior는 0.643이므로, $\phi$를 0.643에 가깝게 맞추면 된다.

$$
q_\phi(C = \text{치우침} \mid H) = \phi
$$
