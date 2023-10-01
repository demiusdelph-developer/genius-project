**Шрифт** - це комплект літер певного типу для відображення тексту

Є три типи (сімейства) які можуть використовуватись на сайті

- **serif** - шрифт з засічками
- **sans-serif** - стандартний шрифт без засічок
- **monospace** - моноширинний шрифт, це шрифт літери якого мають однакову шририну

Сімейство шрифтів зазвчиай визначають в css файлі за допомогою правила font-family і вказується основний шрифт та через кому сімейство шрифта яке відповідає макету, якщо в макеті шрифт із засічками то вказується serif якщо без то sans-serif ну і з моношорифтом відповідна історія

**Підключення шрифтів**
- Використання системних шрифтів - у операційних шрифтів є безліч вже вбудованих шрифтів, тому можна використовувати і їх, попередньо можна уточнити наявність потрібного шрифту в самій операційній системі або за допомогою відповідних ресурсів де є вказаний перелік, цей варіант не надійний оскільки у користувачів можуть бути різні редакції операційних систем в яких може бути відсутній шрифт, або користувач можливо сам частину системних ресурсів видалив щоб збільшити об'єм вільно місця на жорсткому диску, тому найкраще підключати шрифти одним з наступних способів
- Використання ресурсу Google Fonts - https://fonts.google.com/ на ньому теж можна знайти безліч шрифтіві так як гугл є одним з основних гігантів у всесвітній павутині він є досить надійним ресурсом який працює безперебійно. При переході за посиланням в рядку пошуку 'Serach fonts' потрібно ввести необхідну назву після чого ресурс запропонує доступні варіанти, наприклад ми можемо ввести Poppins один з відомих шрифтів який часто використовується на веб сайтах, після того як побачимо результат натискаємо на нього і бачимо перелік доступних варіантів даного шрифту, а точніше його жирність, також зверху є поле 'Type here to preview text' в якому можна ввести слово або декілька і поабчити нижче приклад написаний саме за допомогою цього шрифту, якщо ж повернутись до варіантів то тут нам потрібно додати потрібні варіанти для можливості їх використання біля кожного варіанту є кнопка 'Select 'назва варіанту'' при натисканні справа з'являється панель де можна побачити назви обраних варіантів, код (посилання) яке потрібно вставити в html або css файл (link або import) і варіант підключення font-family наприклад у нас Poppins без засічок то для нього відразу пропонується варіант
```css
font-family: 'Poppins', sans-serif;
```
- **Локальне підключення** - професійний підхід оскільки при підключенних локальних шрифтах можна бути впевненим що вони завжди працюватимуть і це пришвидшує роботу сайту оскільки не відбувається завантаження зі сторонніх ресурсів, а ще гірше коли ресурс недоступний і шрифти можуть не працювати, приклад такого підключення
```css
@font-face {
  font-display: swap;
  font-family: 'Poppins';
  font-style: normal;
  font-weight: 400;
  src: url('../fonts/poppins-v20-latin-regular.woff2') format('woff2');
}
```
Ми тут можемо бачити підключення шрифта poppins який знаходиться в папці fonts, такий варіант підключення можна знайти на ресусі https://gwfh.mranftl.com/fonts а разом з кодом і самий шрифт можна завантажити, або ж як варіант взяти цей варіант підключення і переробити під свій шрифт можна

**Оформлення тексту**
- text-decoration - відповідає за підкреслення тексту
- text-align - відповідає за розташування тексту
- text-transform - відповідає за відображення тексту, наприклад можна зробити всі літери великими або малими
- text-shadow - властивість яка дозволяє додати тінь для тексту
- letter-spacing - влвставість яка дозволяє встановити відступ між літерами
- word-spacing - дозволяє вказати відступ між словами
- white-space - властивість яка визначає чи може переноситись контент всередині блоку якщо він не влазить в 1 рядок

**Властивості шрифту**
- font-family - як ми розглядали раніше відповідає за оголошення шрфту
- font-size - за допомогою цієї властивості можна вказати розмір шрифту
- font-weight - властивість яка відповідає за товщину шрифту
- font-style - вказує на стиль шрифту

В головному проекті можна побачити частину задіяних властивостей для офорлмення і основних властивостей шрифту, тема про шрифти є теоретичною і з урахуваможливих можливостей відмінностей не може бути продемонстрована наглядно

