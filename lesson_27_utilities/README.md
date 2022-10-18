# Bootstrap - утиліти

{property}{sides}-{size} для xs;
{property}{sides}-{breakpoint}-{size} для sm, md, lg, и xl.

- Замість {property} необхідно вказати першу літеру назви відступу, тобто m або p (m – для margin, p – для padding).

- Замість {sides} необхідно вказати сторону (t - для завдання відступу тільки зверху, b - знизу, s - ліворуч, e - праворуч) або кілька сторін (x - ліворуч і праворуч, y - зверху та знизу). Якщо {sides} не вказати, тоді відступ буде встановлений для всіх 4 сторін елемента.

- Замість {breakpoint} потрібно вказати контрольну точку (sm, md, lg або xl). Іншими словами, визначити мінімальну ширину viewport, починаючи з якої відступи, що задаються цим класом, будуть діяти.

- Замість {size} необхідно задати величину відступу (за допомогою одного з наступних значень):

0 (рівно 0);
1 (рівно $ spacer _ 0.25);
2 (до $spacer _ 0.5);
3 (рівно $spacer);
4 (рівно $spacer _ 1.5);
5 (рівно $spacer _ 3);
auto (рівно auto) можна використовувати тільки для margin.

.mx-auto для горизонтального вирівнювання блоку відносно блоку контенту фіксованої ширини – тобто контент, якому задані display: block та набір width за допомогою горизонтальних марджинів та auto.

<div class="mx-auto" style="width: 200px;">
    Відцентрований елемент
</div>

Класи називаються у форматі .d-{breakpoint}-{value}

breakpoint (контрольна точка): sm, md, lg та xl
value (значення) – одне з: none, inline, inline-block, block, table, table-cell, table-row, flex, inline-flex

Shadows (Тіні)
Додавайте або видаляйте тіні елементам за допомогою утиліти box-shadow.

<div class="shadow-none p-3 mb-5 bg-light rounded">Без тіней</div>
<div class="shadow-sm p-3 mb-5 bg-white rounded">Маленька тінь</div>
<div class="shadow p-3 mb-5 bg-white rounded">Звичайна тінь</div>
<div class="shadow-lg p-3 mb-5 bg-white rounded">Велика тінь</div>

Text (Текст)
Документація та зразки для звичайних текстових утиліт для керування вирівнюванням, огортанням, вагою і т.д.
Вирівнюйте текст у відповідності з вирівнюванням компонентів за допмогою класів вирівнювання

<p class="text-left">Вирівнювання по лівому краю.</p>
<p class="text-center">Вирівнювання по центру.</p>
<p class="text-right">Вирівнювання по правому краю.</p>

<p class="text-sm-left">Вирівнювання по лівому краю для розміру SM (small) або ширшого.</p>
<p class="text-md-left">Вирівнювання по лівому краю для розміру MD (medium) або ширшого.</p>
<p class="text-lg-left">Вирівнювання по лівому краю для розміру LG (large) або ширшого.</p>
<p class="text-xl-left">Вирівнювання по лівому краю для розміру XL (extra-large) або ширшо

Sizing(Розміри)
Утиліти ширини та висоти генеруються з карти розміру $sizes Sass у \_variables.scss. Включають підтримку по 25%, 50%, 75% и 100% по дефолту. Змінюємо ці значення так, як нам потрібно, щоб створити різні утиліти.

Ширина

<div class="w-25 p-3" style="background-color: #eee;">Ширина 25%</div>
<div class="w-50 p-3" style="background-color: #eee;">Ширина 50%</div>
<div class="w-75 p-3" style="background-color: #eee;">Ширина 75%</div>
<div class="w-100 p-3" style="background-color: #eee;">Ширина 100%</div>
<div class="w-auto p-3" style="background-color: #eee;">Ширина auto</div>

Висота

<div style="height: 100px; background-color: rgba(255,0,0,0.1);">
  <div class="h-25 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Висота 25%</div>
  <div class="h-50 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Висота 50%</div>
  <div class="h-75 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Висота 75%</div>
  <div class="h-100 d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Висота 100%</div>
  <div class="h-auto d-inline-block" style="width: 120px; background-color: rgba(0,0,255,.1)">Висота auto</div>
</div>

Ми також можемо використовувати утиліти, щоб встановити висоту та ширину відносно області перегляду.

<div class="min-vw-100">Мінімальна ширина 100vw</div>
<div class="min-vh-100">Мінімальна висота 100vh</div>
<div class="vw-100">Ширина 100vw</div>
<div class="vh-100">Висота 100vh</div>
