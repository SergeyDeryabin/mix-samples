# Artistic neural style transfer. Author: Benson Ruan
# Нейронная передача художественного стиля. Автор: Бенсон Руан
  
Нейронная передача художественного стиля(Artistic neural style transfer) - 
оптимизационная технология, обрабатывающая исходное  
изображение на основе изображения шаблона стиля(такого как картина известного живописца), 
т.е смешающая изображения вместе, и таким образом, выходное изображение похоже на исходное изображение, 
но "нарисовано" в стиле изображения шаблона стиля.

  
## Живой демонстрационный пример
 Нейронная передача художественного стиля. Выполняется  в браузере вашего устройства. 
  * Кнопка “Загрузите своё фото” позволяет на вашем устройстве выбрать исходное фото.
  * Кнопка “Загрузите свой стиль” позволяет на вашем устройстве выбрать фото шаблона стиля(фото картины художника).
  * Кнопка “Запустить процесс смешения и передачи стиля” позволяет на вашем устройстве запустись процесс смешения фото и передачи стиля.
  * Процесс занимает много времени. Зависит от мощности вашего устройства. Лучше демо-приложение запустить в браузере ПЭВМ.
    Итоговое фото(на нижней панели, пока белой/пустой) будет похоже на исходное изображение, но "нарисовано" в стиле фото шаблона стиля.

 				
**[https://sergeyderyabin.github.io/Neural-Style-Transfer/]
 ![style-transfer](https://bensonruan.com/wp-content/uploads/2019/09/art_style_transfer.jpg)

## Установка
Клонируйте этот репозитарий на свою локальную ПЭВМ
``` bash
git https://github.com/bensonruan/Neural-Style-Transfer.git
```
Свой локальный хост localhost укажите на клонированный корневой каталог

Просмотрите в браузере http://localhost/index.html  


## Библиотеки
* [jquery](https://code.jquery.com/jquery-3.3.1.min.js) - JQuery
* [jQuery.Keyframes](https://github.com/Keyframes/jQuery.Keyframes) - This library allows dynamic generation of CSS keyframes with callback events and other niceness.
* [magenta.js](https://github.com/tensorflow/magenta-js/tree/master/image) - JavaScript implementation of Magenta's image models uses TensorFlow.js for GPU-accelerated inference
