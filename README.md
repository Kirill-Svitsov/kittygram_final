![GitHub Actions Status](https://github.com/Kirill-Svitsov/kittygram_final/tree/main/.github/workflows/badge.svg)

# Kittygram: Финальное задание

Этот репозиторий содержит финальное задание "Kittygram".
Kittygram - это проект для обмена фотографиями котиков, где пользователи могут загружать
и просматривать фотографии котиков. Проект построен на Django и предоставляет функциональность загрузки,
просмотра и комментирования фотографий.

## Стек

- Django
- Docker
- PostgreSQL
- HTML/CSS
- JavaScript
- GitHub Actions

## Развертывание проекта

Для развертывания проекта, выполните следующие шаги:

Клонируйте репозиторий:

```bash
git clone https://github.com/Kirill-Svitsov/kittygram_final.git
cd kittygram_final
```

1. Установите Docker, если он не установлен.

2. Создайте файл `.env` в корне проекта и заполните его данными:

```env
SECRET_KEY=your_secret_key
DEBUG=True
DB_NAME=your_database_name
DB_USER=your_database_user
DB_PASSWORD=your_database_password
DB_HOST=db
DB_PORT=5432
```
3. Соберите и запустите контейнеры:

```bash
docker-compose up --build
```

4. Примените миграции:

```bash
docker-compose exec backend python manage.py migrate
```

5. Создайте суперпользователя:

```bash
docker-compose exec backend python manage.py createsuperuser

```

Автор
Этот проект был создан Кириллом Свицовым.
