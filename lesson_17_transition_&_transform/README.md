#

# Transition -- дозволяє анімувати вихідне значення CSS-властивості на нове значення із плином часу, керуючи швидкістю зміни значень.

Наступні чотири властивості управляють різними параметрами переходу.
-transition-property: <властивість>
-transition-duration: <час>
-transition-timing-function: <функція розподілу часу>
-transition-delay: <затримка>

короткий запис:
transition: [property] [duration] [timing-function] [delay]

==================================================

 # Властивість Transform -- Може змінювати розмір, форму та положення елемента на веб-сторінці.

-translate(x,y)  Зміщує елемент на нове місце (ліворуч чи вгору -)
-scale(x,y)  Масштабує елементи, збільшуючи або зменшуючи їх.Вих зач 1
-rotate(кут)  Обертає елементи на задану кількість градусів 
-skew(x-кут, y-кут)  Використовується для деформації сторін

Допустимі значення:
-matrix() — будь-яке число translate(),
-translateX(), translateY() — одиниці довжини (додаткові та відємні), %
-scale(), scaleX(), scaleY() — будь-яке число
-rotate() — кут (deg, grad, rad или turn)
-skew(), skewX(), skewY() — кут (deg, grad, rad).

==============================================

# Властивості Animation

-animation-name  <назва анімації> (через @keyframes;)
-animation-duration  <як довго триватиме анімація>
-animation-timing-function  <як розраховуються проміжні стани>
-animation-delay  <анімація починається із затримкою>
-animation-iteration-count  <скільки разів має повторитись анімація>
-animation-direction  <чи має анімація працювати в зворотному напрямку>
-animation-fill-mode  <які стилі застосовуються до початку анімації та після неї>

короткий запис:
animation: [name] [duration] [timing-function] [delay] [iteration-count] [direction] [fill-mode] [play-state]

Значення необов'язкових властивостей можна пропустити або поміняти місцями. Виняток становлять властивості duration і delay - значення тривалості анімації завжди повинно зазначатися до затримки.

[куб 3D]https://codepen.io/desandro/pen/bMqZmr