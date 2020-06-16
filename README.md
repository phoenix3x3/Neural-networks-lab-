Лабораторная работа №3
Здесь графики обученной модели сети VGG16.

1 конфигурация. lr= 0.0000004, batch_size = 8.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/lr%204*10-7%20.png)

2 конфигурация. lr= 0.0000008, batch_size = 8.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/lr%208*10-7.png)

3 конфигурация. lr = 0.000001, batch_size = 8.
![Image alt](https://github.com/MaximGil/SMOMI/blob/Lab3/lab3%20new/lr%201*10-6.png)

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


