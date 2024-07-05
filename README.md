# Lampa

Приложение полностью бесплатное и использует публичные ссылки для просмотра информации о фильмах, новинках, популярных фильмов и т.д. Вся доступная информация используется исключительно в познавательных целях. Приложение не использует свои серверы для распространения информации.

#### Устройства
* Samsung Tizen
* MSX

## Установка для MSX
### Необходим свой хостинг или локальный веб-сервер. 
1. Нажмите на зелёную кнопку (Code), выберите (Download ZIP) и распакуйте загруженный архив.
2. Откройте файл msx/start.json и замените содержимое {domain} на свой домен или IP.
3. Загрузите файлы на хостинг или веб-сервер.
4. Откройте MSX и выполните установку.

## Запуск в Docker'е
1. Соберите образ `docker build --build-arg domain={domain} -t lampa . `
2. Запустите контейнер `docker run -p 8080:80 -d --restart unless-stopped -it --name lampa lampa`
3. Готовое решение: https://lampa.lobs.su/

## Подключение дополнительных модулей
#### Модуль "Кинозал" (просмотр фильмов и сериалов из источников наподобие IVI)
1. https://lampa.lobs.su/kinozal.js
2. http://192.168.../kinozal.js
