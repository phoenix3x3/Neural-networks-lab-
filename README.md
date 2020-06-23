# Лабораторная работа №3
Здесь графики обученной модели сети VGG16.
1 Этап
1 конфигурация. lr= 0.000001.
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/1_train.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/1_test.jpg)



2 конфигурация. lr= 0.00001.
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/1_train.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/1_test.jpg)

2 Этап
Использована предобученная на image.net сеть VGG16. В данной сети были заморожены свёрточные слои и производилось обучение классификатора с последующим сохранением весовых коэффициентов. Графики для замороженной сети:

Оранжевый lr= 0.00001.
Голубой lr= 0.0001
Красный lr= 0.000001
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/2_train.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/2_test.jpg)

3 Этап c размороженной сетью и предобученным классификатором
lr= 0.000001
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/3_train.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab3/images/3_test.jpg)






