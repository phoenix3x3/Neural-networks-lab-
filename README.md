# Neural-networks-lab-
### Step Decay
Оранжевый - initial_lr = 0.001, drop = 0.3; Синий - initial_lr = 0.005, drop = 0.4; Красный - initial_lr = 0.0001, drop = 0.5; Голубой - Warm-Up 10 эпох, init_lr 0.001 до 0.01, drop 0.2. 
Cильно выделяется оранжевый: вообще не сошёлся , при этом имеет самый нестабильный характер, в то время как остальные три сошлись по точности уже к 20-25 эпохам идут гладко. Красный и синий сходятся в одно время как по ошибке, так и по точности на валидационной выборке. Получается, что лучшим вариантом будет lr = 0.0001/0.005 и drop = 0.4/0.5
#### Train
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/train1.jpg)
#### Validation
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/validation1.jpg)
#### Learning Rate
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/lr1.png)

### Exponential Decay
Оранжевый - init_lr 0.001, k 0.5, Синий - init_lr 0.01, k 0.4, Красный - init_lr 0.001, k 0.2, Голубой - с Warm-Up на 10 эпох init_lr 0.001 до 0.01, k 0.4
На обучающей выборке на графике точности красный график лучший результат,  голубой и синий имеют точность гораздо хуже остальных. На графике ошибки, лучшие значения опять-таки показывают красный и оранжевый графики. На графике точности валидационноый выборке, все графики имеют схожие по значению выборосы, но заметно что оранжевый график имеет самый маленькие. На а на графике ошибки хуже всего себя показывает голубой, при этом синий показал себя даже чуть лучше, но исходя из всех данных можно сделать вывод, что оптимальным является красный график (init_lr 0.001, k 0.2)
#### Train
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/train2.jpg)
#### Validation
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/validation2.jpg)
#### Learning Rate
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab5/lr2.png)
