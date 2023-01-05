# Hand Written Digit Recognition. Author: Benson Ruan
# Распознавание рукописной цифры. Автор: Бенсон Руан
 Распознавание рукописной цифры, с использованием javascript-библиотекой tensorflowjs
## Живой демонстрационный пример
**[https://sergeyderyabin.github.io/Hand-Written-Digit-Recognition/]

![handwritten-recognition](https://bensonruan.com/wp-content/uploads/2019/09/handwritten-recognition-5.gif)
 
## Установка
Клонируйте этот репозитарий на свою локальную ПЭВМ
``` bash
git https://github.com/bensonruan/Hand-Written-Digit-Recognition.git
```
Укажите на своем локальном хосту на клонированный корневой каталог

Просмотрите в браузере http://localhost/index.html  

## Start Predicting Hand Written Digit
* Нарисуйте на холсте: мышью на ПЭВМ или пальцем на мобильном устройстве
* Нажмите кнопку "Predict"("Предсказать"), чтобы получить результат предсказания рукописной цифры
* Нажмите кнопку "Clean"("Очистить"), чтобы снова начать рисовать

## Предварительно обученная модель(Pre-trained model) 
Используйте MNIST-набор данных(MNIST dataset) от Keras с CNN(Convolutional Neural Network; Сверточная Нейронная Сеть;СНС)
```python
model = keras.Sequential([
    keras.layers.Conv2D(32, (5, 5), padding="same", input_shape=[28, 28, 1]),
    keras.layers.MaxPool2D((2,2)),
    keras.layers.Conv2D(64, (5, 5), padding="same"),    
    keras.layers.MaxPool2D((2,2)),    
    keras.layers.Flatten(),   
    keras.layers.Dense(1024, activation='relu'),    
    keras.layers.Dropout(0.2),   
    keras.layers.Dense(10, activation='softmax')
])

model.compile(optimizer='adam', loss='categorical_crossentropy', metrics=['accuracy'])
```

## Библиотеки
* [jquery](https://code.jquery.com/jquery-3.3.1.min.js) - JQuery
* [tensorflowjs](https://github.com/tensorflow/tfjs) - JavaScript-библиотека для обучения и развертывания моделей машинного обучения(machine learning models)
* [Chart.js](https://github.com/chartjs/Chart.js) - JavaScript-библиотека для отображения диаграмм( charts)
