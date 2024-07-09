# Lampa
Приложение полностью бесплатное и использует публичные ссылки для просмотра информации о фильмах, новинках, популярных фильмов и т.д. Вся доступная информация используется исключительно в познавательных целях. Приложение не использует свои серверы для распространения информации.

#### Устройства
* Samsung Tizen
* MSX (находится в магазине приложений телевизора)
* PC

## Установка для MSX (находится в магазине приложений телевизора)
#### Необходим свой хостинг или локальный веб-сервер.
1. Нажмите на зелёную кнопку (Code), выберите (Download ZIP) и распакуйте загруженный архив.
2. Откройте файл msx/start.json и замените содержимое {domain} на свой домен или IP.
3. Загрузите файлы на хостинг или веб-сервер.
4. Откройте MSX и выполните установку, указав адрес своего сервера.

#### Нет возможности или желания возиться.
* Откройте MSX и выполните установку, указав адрес: https://lampa.lobs.su/

## Запуск в Docker'е
1. Соберите образ `docker build --build-arg domain={domain} -t lampaf . `
2. Запустите контейнер `docker run -p 8080:80 -d --restart unless-stopped -it --name lampa lampaf`

## Запуск на PC
* Открыть ссылку в любом обозревателе: https://lampa.lobs.su/

## Подключение дополнительных модулей
#### Модуль "Кинозал" (просмотр фильмов и сериалов из источников наподобие IVI)
* https://plugs.lobs.su/kinozal.js

#### Модуль "Публичные парсеры" (отображение каталогов поиска пиров для торрентов)
* https://plugs.lobs.su/pubtorr.js

#### Добавляет в меню пункт "Парсер"
* https://plugs.lobs.su/etor.js

#### Золотая Тема
* https://plugs.lobs.su/gold_theme.js
