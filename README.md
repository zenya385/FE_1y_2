# FE_1y_2

<!-- =====================CALC================= -->

<!--
.element {
 flex-basis: calc((100% - кол-во маржинов в строке * значение маржина) / кол-во элементов в строке);
};
 -->

==============Респонсивні зображення=============

Найпростіший спосіб реалізувати респонсивність - це використовувати одне зображення для всіх пристроїв, задавши йому певний набір CSS-властивостей.

img {
display: block;
max-width: 100%;
height: auto;
}

=========Масштабовані зображення==========

img {
display: block;
width: 100%;
max-width: 100%;
}

==========Приховати секцію===================

.visually-hidden {
position: absolute;
width: 1px;
height: 1px;
margin: -1px;
padding: 0;
overflow: hidden;
border: 0;
clip: rect(0 0 0 0);
}
