# ELBO 🌱

ELBO(evidence lower bound)는 evidence $\log p_\theta(x)$의 하한이다. $q_\phi$는 [variational posterior](variational-posterior.md)다. 아래 등식이 성립하는데 KL divergence가 0 이상이기 때문이다. $\log p_\theta(x)$는 $\phi$와 상관없이 고정이므로, ELBO만 키우면 KL이 저절로 줄어든다.

$$
\log p_\theta(x) = \underbrace{\mathbb{E}_{q_\phi(z \mid x)}\left[\log \frac{p_\theta(x, z)}{q_\phi(z \mid x)}\right]}_{\text{ELBO}} + \mathrm{KL}\big(q_\phi(z \mid x) \,\Vert\, p_\theta(z \mid x)\big)
$$

**예.** 공정한 동전과 앞면 확률 0.9인 동전 중 하나를 $1/2$씩의 확률로 몰래 골라 던졌더니 앞면 $H$가 나왔다. evidence는 $P(H) = 0.7$이고, 진짜 posterior는 치우친 동전일 확률 0.643이다. 추측 $q_\phi(\text{치우침} \mid H) = \phi$를 바꿔 가며 계산하면 ELBO와 KL의 합은 늘 $\log 0.7 = -0.357$이고, 추측이 진짜 posterior에 닿으면 KL이 0이 되어 ELBO가 evidence와 같아진다.

| $\phi$ | ELBO | KL | 합 |
|---|---|---|---|
| 0.5 | −0.399 | 0.043 | −0.357 |
| 0.8 | −0.416 | 0.059 | −0.357 |
| 0.643 | −0.357 | 0 | −0.357 |
