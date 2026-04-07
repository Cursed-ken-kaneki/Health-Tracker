Общая информация

Health Tracker — это веб-приложение для отслеживания показателей здоровья пользователя (например: активность, питание, параметры тела и т.д.).

Проект построен на фреймворке Laravel (PHP) и использует стандартную MVC-архитектуру.

Архитектура проекта

Проект следует шаблону MVC (Model–View–Controller):


Models (app/Models) — работа с данными и БД

Controllers (app/Http/Controllers) — бизнес-логика

Views (resources/views) — интерфейс пользователя

Основные директории

app/ — основная логика приложения

routes/ — маршруты (web.php, api.php)

resources/ — шаблоны (Blade), стили, JS

database/ — миграции и сиды

config/ — конфигурация проекта

public/ — точка входа (index.php)

storage/ — кэш, логи, файлы

tests/ — тесты

vendor/ — зависимости (Composer)

Установка и запуск

Установить зависимости:

composer install

npm install

Создать файл окружения:

cp .env.example .env

php artisan key:generate

Настроить базу данных в .env


Выполнить миграции:

php artisan migrate

Запустить сервер:

php artisan serve

Маршруты

Маршруты определены в:

routes/web.php — веб-интерфейс

routes/api.php — API

Основной функционал (типовой)

(на основе структуры проекта)

Регистрация и авторизация пользователей

Отслеживание показателей здоровья

CRUD-операции (создание, просмотр, редактирование, удаление данных)

Работа с базой данных через Eloquent ORM

База данных

Используется миграционная система Laravel:

database/migrations — структура таблиц

database/seeders — тестовые данные

Тестирование

Тесты находятся в папке:

tests/

Запуск:

php artisan test

Зависимости

PHP (Laravel)

Composer (backend)

Node.js + npm (frontend)

Vite (vite.config.js)
Дополнительно

Конфигурация хранится в config/

Переменные окружения — .env

Логи — storage/logs
