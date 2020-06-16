# Лабораторная работа №3
Здесь графики обученной модели сети VGG16.

1 конфигурация. lr= 0.000001, batch_size = 16.
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/1.1.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/1.2.jpg)



2 конфигурация. lr= 0.00001, batch_size = 16.
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/2.1.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/2.2.jpg)


3 конфигурация. lr = 0.00001, batch_size = 32.
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/3.1.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/Lab3/3.2.jpg)


В файле train_freeze.py использована предобученная на image.net сеть VGG16. В данной сети были заморожены свёрточные слои и производилось обучение классификатора с последующим сохранением весовых коэффициентов. Графики для замороженной сети:

Тут за основу взял, конфигурацию 2 , то есть lr= 0.0000008, batch_size = 8.
Использовал train_freeze.py
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/Freeze%20-%20unfreeze8*10-7/freeze%20lr%208*10-8.png)

Так как на размороженной нужно уменьшить темп обучения, то я остановился на 8*10^(-12)
lr = 8*10^(-12), batch_size = 8. Использовал train_unfreeze.py
График размороженной сети 
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/Freeze%20-%20unfreeze8*10-7/unfreeze%20lr%208*10-12.png)
 
Еще один вариант, но уже взял за основу конфигурацию 3. lr = 0.000001, batch_size = 8.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/freeze-unfreeze1*10-7/freeze%20lr%3D10-7.png)

График размороженной lr = 1*10^(-11), batch_size = 8.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/freeze-unfreeze1*10-7/lr%2010-11.png)


