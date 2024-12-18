# Система онлайн-бронирования билетов в кинотеатр

## Описание проекта

Данный проект представляет собой полнофункциональную веб-платформу для онлайн-бронирования билетов в кинотеатр, включающую систему администрирования для управления залами, сеансами и предварительным бронированием.

## Информация о проекте

- **Автор:** Никита Сероштнов
- **Технологический стек:** 
  - Фреймворк: Laravel 10.44.0
  - Версия PHP: 8.3.12

## Инструкция по развертыванию

1. Клонировать репозиторий:
   ```
   git clone https://github.com/NikitaKST/cinema
   ```
2. Переименовать `.env.example` в `.env`.
3. В файле `.env` указать абсолютный путь к базе данных SQLite:
   ```
   DB_DATABASE=/path/to/your/project/database/database.sqlite
   ```
4. Убедиться в наличии установленного Composer.
5. Установить зависимости Laravel в директории проекта.
6. Выполнить установку и сборку frontend-зависимостей:
   ```
   npm install
   npm run build
   ```
7. Сгенерировать ключ приложения:
   ```
   php artisan key:generate
   ```
8. Запустить локальный сервер разработки:
   ```
   php artisan serve
   ```

## Доступ к панели администратора

- URL: `http://127.0.0.1:8000/admin`
- Учетные данные:
  - Email: administrator@mail.ru
  - Пароль: netology

## Дополнительная информация

База данных SQLite с предварительно заполненной сеткой сеансов находится в директории `database` проекта.
В случае еслине отображаются логотипы для фильмов, убедитесь, что вы создали символическую ссылку:
- php artisan storage:link