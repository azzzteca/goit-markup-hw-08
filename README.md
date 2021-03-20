



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



.advantages {
  padding-top: 94px;
  padding-bottom: 94px;
}
  
.advantages__list {
  display: flex;
  
  margin-left: -30px;
}
  
.advantages__power {
  flex-basis: calc( 100% / 4 - 30px);
  margin-left: 30px;
}
  
.advantages__item {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 30px;
  
  width: 270px;
  height: 120px;
  background-color: $buttons-color;
}
  
.advantages__title {
  margin-top: 0;
  margin-bottom: 9.01px;
  color: $main-color;
  text-transform: uppercase;
  font-size: 14px;
  font-weight: 700;
  line-height: 1.2;
}
  
.advantages__text {
  margin-top: 0;
  margin-bottom: 0;
  
  color: $secondary-color;
  font-size: 14px;
  font-weight: 400;
  line-height: 1.7;
}