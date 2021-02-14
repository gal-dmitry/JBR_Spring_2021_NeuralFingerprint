# NeuralFingerprint
**Задание 2**

Результаты в файле `VISUALIZATION_2`

- Python 3.7
- конвертация с помощью 2to3
- `build.convet.py`, функция `softmax`:
замена `return np.exp(X - logsumexp(X, axis=axis, keepdims=True))` 

на `return np.exp(X - np.log(np.sum(np.exp(X), axis=axis)).reshape(-1, 1))`
