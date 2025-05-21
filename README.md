[![Main Kittygram workflow](https://github.com/Mirogor/kittygram_final/actions/workflows/main.yml/badge.svg)](https://github.com/Mirogor/kittygram_final/actions/workflows/main.yml)

# Kittygram — сервис для любителей котиков

**Kittygram** — это веб-приложение, где пользователи могут публиковать карточки котиков, указывать их характеристики и делиться ими с другими. Вы можете добавлять, редактировать и удалять котиков, фильтровать по породам и многое другое. Проект развёрнут в Docker-контейнерах и использует CI/CD для автоматического деплоя.

## Возможности
- Добавление новых котиков
- Загрузка фото и описание
- Просмотр всех котиков
- Панель администратора
- Авторизация через Django admin

## Технологии

- Python
- Django
- PostgreSQL
- Docker / Docker Compose
- Nginx / Gunicorn
- GitHub Actions (CI/CD)
- Telegram Bot (уведомления о деплое)

## Как развернуть проект локально

1. Клонируйте репозиторий:

```bash
git clone https://github.com/Mirogor/kittygram_final.git
cd kittygram_final
```

2. Создайте файл .env со следующим содержимым:

```
SECRET_KEY=ваш_секретный_ключ
ALLOWED_HOSTS=localhost,127.0.0.1,<ваш_домен>
DB_ENGINE=django.db.backends.postgresql
DB_NAME=postgres
POSTGRES_USER=postgres
POSTGRES_PASSWORD=postgres
DB_HOST=db
DB_PORT=5432
```

3. Запустите проект в Docker:

```bash
docker-compose up --build
```
Сайт будет доступен по адресу http://localhost:9000/

## Автор

- Мирон Толканица
- [GitHub: Mirogor](https://github.com/Mirogor)
