



«A4» При просмотре страницы на любом устройстве шириной от 320px, не появляется горизонтальная полоса прокрутки.

«A5» Скрипт мобильного меню подключен в HTML отдельным файлом mobile-menu.js.

Разметка
«B1» У всех страниц в блоке <head> есть метатег viewport.

«B2» Все фоновые и контентные растровые изображения - отзывчивые, и поддерживают экраны с плотностью x1 и x2.

«B3» Для отзывчивых контентных изображений использован элемент <img> с атрибутом srcset и дескриптором x.

«B4» Для отзывчивых фоновых изображений использованы медиа-фукцнии min-device-pixel-ratio и min-resolution.

«B5» Выполнена разметка мобильного меню.

Оформление
«C1» При написании стилей использован Mobile First подход и медиа-функция (min-width: ).

«C2» Стили необходимые только в определённом промежутке, закрыты в медиа-запросы (min-width: ) and (max-width: ) или только (max-width: ).

«C3» В медиа-запросах отсутствует лишнее дублирование стилей.

«C4» Вёрстка выполнена относительно трёх точек перелома: 480px, 768px и 1200px.

«C5» Выполнено оформление мобильного меню.




    <header class="page-header">
      <div class="container">
        <button
          class="menu-toggle js-open-menu" aria-expanded="false" aria-controls="mobile-menu" >
          <svg width="24" height="24" fill="currentColor"</svg>
        </button>

        <ul class="menu">
          <li><a href="" class="link">О нас</a></li>
          <li><a href="" class="link">Работы</a></li>
          <li><a href="" class="link">Контакты</a></li>
          <li><a href="" class="link">Карьера</a></li>
        </ul>
      </div>
    </header>

    <main>
      какой-то текст
    </main>

    <div class="menu-container js-menu-container" id="mobile-menu">
      <button class="menu-toggle js-close-menu">
        <svg></svg>
      </button>

      <ul class="mobile-menu">
        <li><a href="" class="link">О нас</a></li>
        <li><a href="" class="link">Работы</a></li>
        <li><a href="" class="link">Контакты</a></li>
        <li><a href="" class="link">Карьера</a></li>
      </ul>
    </div>