<h1>Финальный проект по созданию API</h1>
<h2>с использованием Django REST framework</h2>

<h3><i>Описание</h3></i>
Позволяет пользоваться функционалом приложения без посещения сайта.

<h3><i>Реализованные возможности API:</h3></i>
<ul>
  
 <li>Подписка на пользователя,</li>
 <li>Просмотр, создание и удаление постов,</li>
 <li> Просмотр и создание групп,</li>
 <li>Возможность комментировать, просматривать и удалять комментарии,</li>
 <li>Фильтрация по полям.</li></ul>
 <h3>Документация расположена по адресу http://localhost:8000/redoc/</h3><br>
 <h3>Установка</h3>
 Клонируем репозиторий на локальную машину:

$ <b>git clone</b> https://github.com/EvaBee/api_final_yatube.git

Создание виртуального окружения:

$ <b>python -m venv venv</b>

Установка зависимостей:

$ <b>pip install -r requirements.txt</b>

Создание и применение миграций:

$ <b>python manage.py makemigrations</b> и $ <b>python manage.py migrate</b>

Запуск django сервера:

$ <b>python manage.py runserver</b><br>

API готов к использованию.

<h3>Пример запроса:</h3>
GET http://127.0.0.1:8000/api/v1/posts/

```
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





