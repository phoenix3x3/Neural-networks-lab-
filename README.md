# Lab_2

Во всех случаях модель обучалась: опитмизатор - сигмоида, ошибка - категориальная кроссэнтропия, метрика - категориальная точность.

Batch_size = 50.
epoch = 50.

1 Этап - Исходный файл; 

        tf.keras.layers.Input(shape=(224,224,3)),
        tf.keras.layers.Conv2D(filters=8, kernel_size=3),
        tf.keras.layers.MaxPool2D(),
        tf.keras.layers.Conv2D(filters=16, kernel_size=3),
        tf.keras.layers.MaxPool2D(),
        tf.keras.layers.Conv2D(filters=32, kernel_size=3),
        tf.keras.layers.MaxPool2D(),
        tf.keras.layers.Flatten(),
        tf.keras.layers.Dense(NUM_CLASSES, activation=tf.keras.activations.softmax)
        
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab2/images/0.1.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab2/images/0.2.jpg)

2 Этап - Меняем параметры
  2.1 Оранжевый - Добавили ещё один полносвязный слой с filters=32  и kernel_size=3
  2.2 Синий - Добавили ещё один полносвязный слой с filters=64  и kernel_size=3
  2.3 Красный - Меняем параметр из 2.2 filters с 64 на 16
  2.4 Голубой - Убираем с конца слои, оставляя 2 полносвязных слоя с filters = 8 и 16

![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab2/images/1.1.jpg)
![Image alt](https://github.com/phoenix3x3/Neural-networks-lab-/raw/lab2/images/1.2.jpg)
