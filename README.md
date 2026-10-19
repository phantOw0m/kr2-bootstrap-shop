# MonoLEED — Интернет-магазин моноколёс

## Контрольная работа №2
**Тема:** «CSS-фреймворки: разработка интерфейса на Bootstrap или альтернативном CSS-фреймворке».
**Студент:** Самошкина Майя Кирилловна
**Группа:** ЭФБО-03-25

## Краткое описание проекта
Сайт интернет-магазина по продаже моноколёс. Проект выполнен с использованием CSS-фреймворка Bootstrap. Реализован единый визуальный стиль (жёлто-чёрная гамма), адаптивная вёрстка, интерактивные элементы (модальное окно, аккордеон, выпадающие списки).

## Используемый фреймворк и способ подключения
- **Фреймворк:** Bootstrap 5.
- **Способ подключения:** Локальный (без CDN). 
- Файлы фреймворка размещены в папке `vendor/bootstrap/`. 
- Используются:
  - `vendor/bootstrap/css/bootstrap.min.css`
  - `vendor/bootstrap/js/bootstrap.bundle.min.js`
- Собственный файл стилей `css/custom.css` подключён после Bootstrap для переопределения стандартных стилей.

## Структура проекта
```text
kr2-bootstrap-shop/
├── index.html
├── catalog.html
├── product.html
├── order.html
├── contacts.html
├── css/
│   └── custom.css
├── images/
├── vendor/
│   └── bootstrap/
│       ├── css/
│       │   └── bootstrap.min.css
│       └── js/
│           └── bootstrap.bundle.min.js
├── README.md
└── .gitignore

Реализованные Bootstrap-компоненты:

Сетка: container, row, col-* (адаптивные классы col-md-*, col-lg-*), отступы g-4.

Навигация: navbar, navbar-expand-lg, nav-link.

Карточки: card, card-body, card-title, card-img-top.

Кнопки: btn, btn-warning, btn-outline-dark, btn-light.

Значки: badge, bg-warning, bg-success, rounded-pill.

Сообщения: alert, alert-warning, alert-dismissible.

Формы: form-control, form-label, form-select, input-group, form-check.

Модальное окно: modal, modal-dialog, modal-content.

Дополнительный компонент: accordion (для вывода характеристик на странице товара).

Самостоятельные доработки:

Кастомная стилизация: В custom.css переопределены цвета ссылок в футере и настроены эффекты при наведении на кнопки (плавные переходы).

Кастомизация изображений: Настроено единообразное отображение картинок в карточках товаров с помощью свойства object-fit.

Фильтры: В каталог добавлен выпадающий список (form-select) для фильтрации товаров.

Дополнительная страница: Реализована страница contacts.html с оформлением контактных данных в виде карточек.