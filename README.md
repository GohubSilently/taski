# Task API — REST сервис управления задачами на Django REST Framework.

[![Python](https://img.shields.io/badge/-Python_3.12-3771a1?style=flat&logo=Python&logoColor=ffffff)](https://www.python.org/)
[![Django](https://img.shields.io/badge/-Django-092E20?style=flat&logo=django&logoColor=ffffff)](https://www.djangoproject.com/)
[![DRF](https://img.shields.io/badge/-Django_REST_Framework-red?style=flat&logo=django&logoColor=ffffff)](https://www.django-rest-framework.org/)

Автор — [Халин Вадим](https://t.me/gohub1)

---

## Оглавление
- [Описание](#описание)
- [Функционал](#функционал)
- [Основные технологии](#основные-технологии)
- [API Endpoints](#api-endpoints)
- [Запуск проекта (локально)](#запуск-проекта-локально)

---

## Описание
Task API — это REST-сервис для управления задачами (To-Do List), 
реализованный на базе **Django** и **Django REST Framework**.

---

## Функционал
- Создание задачи
- Получение списка задач
- Просмотр отдельной задачи
- Обновление задачи
- Удаление задачи

---

## Основные технологии
- Python
- Django, DRF
- Docker
- PostgreSQL
- SQLite

---

## API Endpoints

| Метод | Endpoint | Описание |
|------|---------|----------|
| GET | `/api/tasks/` | Получить список задач |
| POST | `/api/tasks/` | Создать задачу |
| GET | `/api/tasks/{id}/` | Получить задачу |
| PUT / PATCH | `/api/tasks/{id}/` | Обновить задачу |
| DELETE | `/api/tasks/{id}/` | Удалить задачу |

---

## Запуск проекта локально
1. Клонируем репозиторий.
```bash
git clone https://github.com/GohubSilently/taski.git && cd taski
```

2. Создаем виртуальное окружение и установливаем заввисимости.
```
python3 -m venv .venv && source .venv/bin/activate
pip install --upgrade pip && pip install -r requirements.txt
```

3. Создаем .env:
```
POSTGRES_DB=taski
POSTGRES_USER=taski_user
POSTGRES_PASSWORD=securepassword
DEBUG=False
SECRET_KEY=your_secret_key
ALLOWED_HOSTS=localhost 127.0.0.1
```

3. Запускаем проект.
```
docker compose up -d
```

4. Переходим по [ссылке](http://localhost:8000).

---
