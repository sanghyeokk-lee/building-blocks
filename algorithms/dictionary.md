# Dictionary 🌱

% 2026-10-22 씨앗: 사용자가 자기 말로 다시 말한 문장을 형식만 다듬어 심었다.

**신호.** key 값을 이용해 value를 뽑아내야 할 때.

Dictionary(dict)는 key와 value로 담겨 있어서, key 값을 이용해 value를 바로 가져올 수 있다. list로 이런 작업을 하면 순서대로 훑어야 해서 예산을 초과한다.

**예.** 가위는 2, 바위는 0, 보는 5로 적을 때, 상대가 낸 손(key)으로 이기는 손(value)을 바로 꺼낸다.

```python
winning_strategy = {0: 5, 2: 0, 5: 2}  # key: 상대가 낸 손, value: 이기는 손
winning_strategy[2]  # 0
```

## 이럴 때 꺼낸다

- 무엇이 오면 무엇으로 바꿀지 정해진 짝이 있다 → dict로 바꾸기표를 만든다
