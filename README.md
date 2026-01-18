<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>
*Ваш потолок – наше вдохновение!** Веб-платформа компании по установке натяжных и подвесных потолков с интеллектуальным калькулятором стоимости, системой заявок и админ-панелью.

> **Наш девиз:** «Качество и скорость»  
> **Наше кредо:** «Доброе имя важнее денег»  
> **Наш стиль:** «Безупречность в работе»

## 📌 Содержание

- [✨ Возможности](#-возможности)
- [🛠 Технологии](#-технологии)
- [🚀 Быстрый старт](#-быстрый-старт)
- [👥 Роли пользователей](#-роли-пользователей)
- [🎯 Ключевые разделы](#-ключевые-разделы)
- [⚡ Команды разработки](#-команды-разработки)
- [🔧 Администрирование](#-администрирование)
- [📖 О Laravel](#-о-laravel)

---

## ✨ Возможности

### 🌐 **Публичная часть**
- **🏠 Лендинг** — информация о компании SkyPro
- **🧮 Калькулятор** — расчёт стоимости потолка с выбором параметров
- **📝 Регистрация/Вход** — создание личного кабинета
- **ℹ️ О компании** — подробная информация о философии качества

### 👤 **Личный кабинет клиента**
- **📋 Профиль** — личные данные (имя, email, телефон)
- **📊 Мои заявки** — история расчётов и их статусы
- **💬 Отзывы** — написание отзывов о работе
- **🚪 Выход** — завершение сессии

### ⚙️ **Панель администратора**
- **📈 Дашборд** — статистика по заявкам, отзывам и проектам
- **📋 Управление заявками** — просмотр, фильтрация, изменение статусов
- **⭐ Модерация отзывов** — одобрение/отклонение клиентских отзывов
- **🖼️ Управление проектами** — портфолио выполненных работ
- **🔔 Уведомления** — настройка оповещений

---

## 🛠 Технологии

### **Backend**
- **PHP 8.1+** с **Laravel 10/11**
- **MySQL 8.0** — база данных
- **Docker & Docker Compose** — контейнеризация

### **Frontend**
- **Bootstrap 5** — CSS-фреймворк
- **JavaScript (ES6+)** — интерактивность
- **Vite** — сборка ассетов
- **Blade Templates** — шаблонизация

### **Инструменты**
- **Composer** — менеджер PHP-зависимостей
- **NPM** — менеджер фронтенд-зависимостей
- **Artisan CLI** — командная строка Laravel

---

## 🚀 Быстрый старт

### 📦 **1. Клонирование репозитория**
```bash
git clone https://github.com/your-username/skypro-potolki.git
cd skypro-potolki

⚙️ 2. Настройка окружения
cp .env.example .env
# При необходимости отредактируйте файл .env

 ###🐳 3. Запуск Docker контейнеров
# Используйте любую из команд:
docker compose up -d
# или
docker-compose up -d

🔧 4. Настройка приложения

# Установка PHP зависимостей
docker compose exec app composer install

# Генерация ключа приложения
docker compose exec app php artisan key:generate

# Запуск миграций базы данных
docker compose exec app php artisan migrate

# Установка фронтенд зависимостей
docker compose exec app npm install
docker compose exec app npm run build

✅ 5. Проверка запуска
# Проверка статуса контейнеров
docker compose ps
# Должно быть: up или running

🌐 6. Доступ к приложению
Сайт:http://localhost:8000/
Админка: admin@admin.com / password

👥 Роли пользователей
Роль	Иконка	Описание	Доступ
Гость	👤	Посетитель сайта	Калькулятор, регистрация, вход, "О нас"
Клиент	👨‍💼	Зарегистрированный пользователь	Личный кабинет, история заявок, отзывы
Администратор	⚙️	Управляющий системой	Полный доступ + админ-панель

🎯 Ключевые разделы
🧮 Калькулятор стоимости
Интерактивный инструмент для расчёта стоимости натяжного потолка:
Параметры расчета:
  - 📏 Геометрия:
    • Длина и ширина комнаты
    • Количество углов
    • Количество труб
    
  - 🏗️ Материалы:
    • Пластиковый профиль
    • Алюминиевый профиль
    • Теневой профиль
    
  - 💡 Дополнительно:
    • Монтаж люстр
    • Монтаж светильников
    • Карнизы (3 типа)

⚙️ Панель администратора
📊 Дашборд — общая статистика
📋 Заявки — управление клиентскими запросами
⭐ Отзывы — модерация клиентских отзывов
🖼️ Проекты — управление портфолио работ

👤 Личный кабинет
Приветствие с именем пользователя
Контактные данные (email, телефон)
История всех отправленных заявок
Форма для написания отзывов

⚡ Команды разработки
🐳 Для Docker-окружения
# Запуск миграций
docker compose exec app php artisan migrate

# Запуск сидов (тестовые данные)
docker compose exec app php artisan db:seed

# Создание контроллера
docker compose exec app php artisan make:controller Api/CalculatorController

# Режим разработки фронтенда
docker compose exec app npm run dev

# Просмотр логов
docker compose logs -f app

⚡ Управление контейнерами
# Запуск проекта
docker compose up -d

# Остановка проекта
docker compose down

# Перезапуск
docker compose restart

# Просмотр логов
docker compose logs -f

🔧 Утилиты Laravel
# Очистка кэша
docker compose exec app php artisan optimize:clear

# Просмотр маршрутов
docker compose exec app php artisan route:list

# Запуск тестов
docker compose exec app php artisan test

🔧 Администрирование
👑 Создание суперпользователя (админа)
Для создания суперпользователя выполните:
docker compose exec app php artisan createsuperuser

Следуйте инструкциям в консоли (введите имя, логин, email, пароль).

🔐 Ручное создание администратора (если не работает)
Если не удалось зайти в админку (admin@admin.com / password):

1.Подключение к MySQL:
docker compose exec mysql mysql -uroot -prootroot sky-pro
2.Проверка существующих пользователей:
SELECT id, login, email, is_superuser FROM users;
3.Добавление администратора:
INSERT INTO users (name, surname, email, login, phone, password, is_superuser, created_at, updated_at)
VALUES (
  'Admin',
  'Administrator',
  'admin@admin.com',
  'admin',
  '+70000000000',
  '$2y$10$92IXUNpkjO0rOQ5byMi.Ye4oKoEa3Ro9llC/.og/at2.uheWG/igi',
  1,
  NOW(),
  NOW()
);
4.Проверка добавления:
SELECT id, login, email, is_superuser FROM users WHERE login = 'admin';
5.Выход:
EXIT;
🔧 Решение проблем
# Если ошибка 500 или "Permission denied"
docker compose exec app chmod -R 775 storage bootstrap/cache

# Сброс и перезапуск миграций
docker compose exec app php artisan migrate:fresh --seed

📖 О Laravel
Laravel — это фреймворк для веб-приложений с выразительным, элегантным синтаксисом. Мы считаем, что разработка должна быть приятным и творческим процессом.

Ключевые возможности Laravel:
Простой и быстрый движок маршрутизации

Мощный контейнер внедрения зависимостей

Несколько бэкендов для хранения сессий и кэша

Выразительная, интуитивно понятная ORM для баз данных

Агностические миграции схем БД

Надежная обработка фоновых заданий

Трансляция событий в реальном времени

Обучение Laravel
Laravel имеет самую обширную и тщательную документацию и библиотеку видеоуроков среди всех современных фреймворков веб-приложений.

Вы также можете попробовать Laravel Bootcamp, где вас проведут через создание современного Laravel-приложения с нуля.

Если не хотите читать, вам поможет Laracasts. Laracasts содержит тысячи видеоуроков по таким темам, как Laravel, современный PHP, модульное тестирование и JavaScript.

Лицензия
Фреймворк Laravel является открытым программным обеспечением, лицензированным по лицензии MIT.

📞 Контакты
📧 Email: support@skypro-potolki.ru

🌐 Сайт: skypro-potolki.ru

📱 Телефон: +7 (XXX) XXX-XX-XX

💼 Компания: ООО "SkyPro"

<div align="center">
🏢 Качество и скорость — наш стандарт в каждом проекте!
Доброе имя важнее денег • Безупречность в работе

Создавая уют в Вашем доме и оставляя частичку душевного тепла в ваших сердцах

</div> ```
Этот README.md:

Сохраняет оригинальную структуру Laravel с логотипом и бейджами

Добавляет информацию о вашем проекте SkyPro

Объединяет все ваши инструкции по запуску и администрированию

Профессионально оформлен с иконками, таблицами и цветовым кодированием

Содержит подробные инструкции для разработчиков и администраторов

Имеет чёткую навигацию по разделам

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

-   [Simple, fast routing engine](https://laravel.com/docs/routing).
-   [Powerful dependency injection container](https://laravel.com/docs/container).
-   Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
-   Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
-   Database agnostic [schema migrations](https://laravel.com/docs/migrations).
-   [Robust background job processing](https://laravel.com/docs/queues).
-   [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

You may also try the [Laravel Bootcamp](https://bootcamp.laravel.com), where you will be guided through building a modern Laravel application from scratch.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

-   **[Vehikl](https://vehikl.com)**
-   **[Tighten Co.](https://tighten.co)**
-   **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
-   **[64 Robots](https://64robots.com)**
-   **[Curotec](https://www.curotec.com/services/technologies/laravel)**
-   **[DevSquad](https://devsquad.com/hire-laravel-developers)**
-   **[Redberry](https://redberry.international/laravel-development)**
-   **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Создание суперюзера (админа)

Для создания суперпользователя (аналог django createsuperuser) выполните в терминале из корня проекта:

```
php artisan createsuperuser
```

Далее следуйте инструкциям в консоли (введите имя, логин, email, пароль и т.д.).

Пользователь будет создан с правами суперюзера (`is_superuser = true`).

## запуск

docker compose или docker-compose
если первая команда без тире не работает, юзай вторую везде

все команды выполнять из корневой папки проекта
то есть, из папки myapp

1. docker compose up -d
   установка образов

2. docker compose ps
   проверка на запуск, должно быть up либо running

3. docker compose exec app php artisan migrate
   инициазизация бд

docker compose up -d - запуск проекта
docker compose down - остановка проекта

попробуй зайти в админский профиль, если не получится, смотри действия ниже

mail: admin@admin.com
Пароль: password

эти команды если не получилось зайти на админку:

docker compose exec mysql mysql -uroot -prootroot sky-pro
после этого должно выводиться:
mysql>

SELECT id, login, email, is_superuser FROM users;
проверка таблицы юзеры

INSERT INTO users (name, surname, email, login, phone, password, is_superuser, created_at, updated_at)
VALUES (
'Admin',
'Administrator',
'admin@admin.com',
'admin',
'+70000000000',
'$2y$10$92IXUNpkjO0rOQ5byMi.Ye4oKoEa3Ro9llC/.og/at2.uheWG/igi',
1,
NOW(),
NOW()
);
добавление админа

SELECT id, login, email, is_superuser FROM users WHERE login = 'admin';
проверка добавления админа

EXIT;
выход из mysql

Если сайт показывает ошибку 500 или "Permission denied", выполни в терминале:
docker compose exec app chmod -R 777 storage bootstrap/cache
