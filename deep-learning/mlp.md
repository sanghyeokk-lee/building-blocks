# MLP 🌱

MLP(Multi-Layer Perceptron, 다층 퍼셉트론)는 선형층과 비선형 활성화 함수를 번갈아서 쌓은 neural network다.

**예.** VAE의 decoder는 선형층, $\tanh$, 선형층을 차례로 쌓은 MLP로, $z$를 받아 픽셀 784개의 logit을 낸다. $W_1, W_2$는 가중치 행렬이고 $b_1, b_2$는 bias다.

$$
\text{logits} = W_2 \tanh(W_1 z + b_1) + b_2
$$
