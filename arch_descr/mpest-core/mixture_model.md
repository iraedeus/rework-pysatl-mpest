# MixtureModel

Класс смеси распределений.



### Атрибуты

#### + components: list[Distribution]

Компоненты смеси.



#### + weights: ndarray

Веса компонент.



#### - logits: ndarray

Логиты. Необходимы для численной стабильности и соблюдения инварианта для весов. Можно оптимизировать их напрямую, хз правда понадобится ли.



### Методы

#### + pdf(X: ndarray): ndarray

Функция плотности.



#### + lpdf(X: ndarray): ndarray

Логарифм функции плотности.



#### + loglikelihood(X: ndarray): ndarray

Логарифм правдоподобия.



#### + q_function(X: ndarray, W: ndarray): ndarray

Q-функция.



#### + generate(size: int): ndarray

Сэмплирование выборки размера `size`.
