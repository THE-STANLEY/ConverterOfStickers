# ConverterOfStickers
Online converter of stickers from Telegram

Frontend by https://github.com/THE-STANLEY
Backend by https://github.com/TeM4ik-prog

_________________________________________________________

Это мини веб-приложение на nodejs и react, c помощью которого можно конвертирвать стикеры из Telegramm(.tgs) в gif

ДЛЯ ЗАПУСКА ПРОЕКТА ВАМ ПОНАДОБИТСЯ:

1.установить Docker(https://docs.docker.com/engine/install/)

скачать и настроить mssql
3.откройте папку

cd converter\server

4.Сделайте сборку проекта

docker build -t stickers-converter .

5.Запуститу сборку.
Тут порт 3000. Чтобы все запросы с клиента корректно работали измените файл converter\client\localSitePath.js на тот торт, который вы захотите поставить

docker run -v ${PWD}:/app -p 3000:3000 stickers-converter
