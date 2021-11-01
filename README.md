# Финальный проект по созданию API
## с использованием Django REST framework

### Описание
*Позволяет пользоваться функционалом приложения без посещения сайта.*

### Реализованные возможности API:

  
 - Подписка на пользователя-
 - Просмотр, создание и удаление постов,
 - Просмотр и создание групп
 - Возможность комментировать, просматривать и удалять комментарии,
 - Фильтрация по полям.

 ### Документация расположена по адресу:
[ http://localhost:8000/redoc/](http://localhost:8000/redoc)

 ### Установка
 **Клонируем репозиторий на локальную машину:**

> git clone https://github.com/EvaBee/api_final_yatube.git

**Создание виртуального окружения:**

> python -m venv venv

**Установка зависимостей:**

> pip install -r requirements.txt

**Создание и применение миграций:**

> python manage.py makemigrations** и python manage.py migrate

#### Запуск django сервера:

> python manage.py runserver

*API готов к использованию*.

### Пример запроса:
GET [http://127.0.0.1:8000/api/v1/posts/](http://127.0.0.1:8000/api/v1/posts/)

```json
[
  {
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2021-10-24T14:15:22Z",
    "image": "string",
    "group": 0
  }
]
