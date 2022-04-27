# REST API для проекта Yatube

### Описание проекта:
Данный API для социльной сети блогеров озволяет работать с постами, комментариями к ним, группами и подписками.
Реализована аутентификация по JWT-токену.

Позволяет делать запросы к моделям проекта: Посты, Группы, Комментарии, Подписки.
Поддерживает методы GET, POST, PUT, PATCH, DELETE.
Предоставляет данные в формате JSON.

### Используемые технологии: 
Django
Django REST Framework
Pillow
Pytest
Python 3
SimpleJWT

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
https://github.com/AxelVonReems/api_final_yatube.git
```

Перейти в папку с проектом

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
WIN: python -m venv venv
MAC: python3 -m venv venv
```

```
WIN: source venv/scripts/activate
MAC: source venv/bin/activate
```

Установить зависимости из файла requirements.txt:

```
WIN: python -m pip install --upgrade pip
MAC: python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
WIN: python manage.py migrate
MAC: python3 manage.py migrate
```

Запустить проект:

```
WIN: python manage.py runserver
MAC: python3 manage.py runserver
```

### Примеры запросов
Документация:
- /redoc/

Получить список всех публикаций:
- /api/v1/posts/

Получить все комментарии к посту 1:
- /api/v1/posts/1/comments/

Получить информацию о сообществе 1:
- /api/v1/groups/1/

Получить все подписки пользователя, сделавшего запрос:
- /api/v1/follow/
