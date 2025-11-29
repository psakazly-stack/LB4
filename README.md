# CRUD веб-додаток для бази даних (Лабораторна робота 4)

# Призначення
Веб-застосунок для керування сутностями бази даних: "клієнти", "автомобілі", "продажі".  
Реалізовано повний набір CRUD-операцій (створення, перегляд списку, редагування, видалення).  
Застосунок побудовано на PHP з використанням PDO, Docker, та розділенням на `public/` і `src/`.

# Структура проекту
db-lab/
app/
public/ - Публічні сторінки (customers.php, cars.php, sales.php)
src/ - DAO-класи
.env - Конфігурація БД
Dockerfile - PHP з pdo_mysql
docker-compose.yml - MySQL, PHP, Nginx
.env.example - Шаблон конфігурації
README.md - Цей файл

# Інструкція запуску
1. Скопіюйте `env.example` у `.env`:
```bash
cp .env.example .env
2. Запустіть середовище:
docker compose up -d
3. Відкрийте у браузері:
http://localhost:8080
