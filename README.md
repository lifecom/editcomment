EditComment
===========

Плагин <strong>EditComment</strong> предназначен для включения возможности редактирования сделанных  комментариев.<cut>

Плагин использует нативную для LS 1.0.1 систему комментирования, не требует хаков  темплейтов и, в то же время, обладает гибкостью настройки. Работает с визуальным редактором.

<strong>EditComment</strong> может хранить "историю" редактирования комментариев заданной вложенности, что может помочь модераторам при рассмотрении жалоб.

Плагин имеет несколько опций, позволяющих ограничивать пользователей в использовании функционала редактирования комментариев:

- ограничение по рейтингу
- ограничение по количеству раз редактирования
- ограничение по времени, прошедшим с момента последнего редактирования
- ограничение на редактирование комментариев, на которые уже есть ответ

Так же могут быть легко добавлены какие-то другие ограничения.

Плагин может добавлять к тексту комментария надпись, сообщающую о дате последнего редактирования.

Имеется возможность задать список пользователей, имеющих право игнорировать ограничения на редактирование комментариев.

Плагин распространяется по лицензии <a href="http://creativecommons.org/licenses/by-sa/3.0/deed.ru">Attribution-ShareAlike 3.0 Unported (CC BY-SA 3.0)</a>
Обязательным условием использования плагина является наличие активной ссылки спонсора оригинальной версии плагина. При модификации плагина запрещается изменять содержание ссылки, а так же помещать ее в невидимые блоки или каким-то образом скрывать ее от людей и роботов поисковиков. Отключить ссылку можно за донейт на сайте <a href="http://livestreetcms.ru/profile/kerby/donate/">http://livestreetcms.ru/profile/kerby/donate/</a>.


Список изменений версий:

1.0.1 - исправлен баг с проверкой возможности редактирования топика при AJAX

1.0.2 - введены новые опции по использованию истории комментариев и добавлена кнопка отмены редактирования для ясности
Обновление: сохранить свой config/config.php, переписать файлы плагина "поверх", скопировать из нового файла config/config.php в старый файл опции 

// Показывать ли кнопку истории редактирования комментария.
// 0 - не показывать никому
// 1 - показывать всем
// 2 - показывать только списку редакторов
// 3 - показывать только админу
$config['show_history_button']=1;

// Показывать ли кнопку отмены редактирования комментария. Можно использовать для "экономии" места под кнопки
$config['show_cancel_button']=true;

и переписать в папку конфига. Сбросить кэш.