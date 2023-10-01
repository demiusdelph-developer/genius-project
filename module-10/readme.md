**SVG**
В цьому модулі ми отримаємо розуміння про векторну та растрову графіку, основну увагу приділимо векторній графіці оскільки при роботі з нею ми працюємо з іконками і важливими елементами у вебі

- Растрова графіка - це графіка, в якій зображення являють собою набір пікселів. Кожен піксель має певний колір і не підлягає редагуванню це є статичне зображення яке можна змінити тільки за розмірами і положенням, відображається у файлах зображень. 
  Основні формати:
  - JPEG – стиснення даних з погіршенням якості, використовується для зберігання фотографій
  - GIF – стиснення без втрати даних, підтримує анімацію та прозорість, використовується для анімованих ілюстрацій
  - PNG – стиснення без втрати даних, підтримує прозорість
- Векторна графіка SVG (Scalable Vector Graphics) - формат графіки і мова для опису векторних зображень. Переваги над растровою графікою:
  - масштабування - не втрачає якість при зміні розміру
  - розмір файлу - важать набагато менше, якщо використовуються для іконок
  - динамічність - можна змінювати через CSS і JavaScript (наприклад, колір)

Розглянемо детальніше про svg
SVG-документ - це текстовий файл з розширенням .svg, в ньому містяться такі значення як viewbox та viewport

SVG-viewport - область перегляду SVG-документа, що задається за
допомогою атрибутів width і height
SVG-viewBox - «вікно перегляду», через яке можна переглядати певну
частину SVG-документа

Ми візуально бачимо тільки viewport

Тепер розглянемо варіанти підключення

Існує декілька способів використання векторної графіки на сторінці:
- елемент <img>
- властивість background-image
- вбудований SVG
- спрайт

елемент <imv> - працює як і у растровій графіці і не дає можливість змінювати зображення svg
властивість background-image - аналогічний варіант до <img> мається на увазі що також можна під'жднати svg за допомогою стилів і це зображення теж не буде керованим
вбудований svg - якщо відкрити будь яке зображення svg воно має формат звичайного коду, тобто за допомогою коду саме зображення і формується, його і можна додати в наш html документ та редагувати за потребою код
SVG-спрайт - це графічний файл, у якому містяться SVG-зображення.
Основні переваги:
- один файл для всіх SVG-зображень/іконок
- не кешується браузером, тобто файл не буде завантажений під час
повторних запитів
- зображення є динамічними, їм можна змінювати стилі через CSS

