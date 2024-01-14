# goit-markup-repeat-hw-02

Repeat html, css. "Barbershop" (2частина)

-скопійовано перший проект;

==== ПРЕПРОЦЕСОР SASS ===; (плагин Live Sass Compiler)

- налаштування: створено папку .vscode, в ній файл settins.json (налаштування вкладено в цей файл);

- створено папку sass, в ній файл main.scss;
- в папці sass створено папки: base, components, layout, utils (в ці папки розподілено весь
  написаний css(1 частина));
- в main.scss @import (підключити розподіленний css);

-- стилі підключено через <link rel="stylesheet" href="./css/main.min.css" />;

= властивості, що повторюються замінено на mixin (font);

==== змінні($), плейсхолдер(% - @extend), міксин (@mixin - @include) =======

- змінні css практичніше;
- плейсхолдер (шаблон властивостей елемента), наприклад для дісплей флекс та елайн ітем;
- МІКСИН ('примеси') (@mixin name {властивості} - @include) - можливо динамічно налаштовувати, та
  передавати значення. Можна задати значення по замовченню: @mixin font
  ($fs:14px, $fw:400,
  $lh:1.36) { font-size:
  $fs;
  font-weight: $fw;
  line-height: $lh;
  };
  виклик @include font ();
  або @include font ($fw:700);
  /_переназначення_/ також, можна вписати формулу line-height: $lh/$fs ======= 1 частина ========

# goit-markup-repeat-hw-01

Repeat html, css. "Barbershop"

-створено репозиторій, разом із .gitignore, README.md;

-добалено: .prettierrc.json;

- фото оптимізовано в https://squoosh.app/ (поріг якості в оптимізаціїї 75%);

-підключено: шрифти (https://fonts.google.com/), стилі (в кінці head), modern-normalize.min
(https://cdnjs.com/libraries/modern-normalize) після шрифтів та перед стилями;

- усі іконки розміщено в svg-спрайті (використано сервіс https://icomoon.io/), svg-спрайт
  оптимізовано (https://jakearchibald.github.io/svgomg/);

-логотипу додана анімаця, для цього підключено бібліотеку (так як і нормалайз) перед style.css
(https://animate.style/#documentation), обираємо анімацію і задаємо її логотипу як клас;

.visually-hidden { position: absolute !important; clip: rect(1px 1px 1px 1px); /_ IE6, IE7 _/ clip:
rect(1px, 1px, 1px, 1px); padding: 0 !important; border: 0 !important; height: 1px !important;
width: 1px !important; overflow: hidden; }
