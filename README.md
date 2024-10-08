# API Yatube

Автор: [Евгений](https://github.com/ClinkyClink)

## Использованные технологии
•**Python**

•**Django**

•**Django Rest Framework**

•**JWT+Djoser**

•**Postman**

## Описание
API для проекта социальной сети Yatube.

## Возможности:

- Получение, создание, обновление, удаление публикаций.
- Получение, создание, обновление, удаление комментариев к публикациям.
- Просмотр сообществ и детальной информации о них.
- Отслеживание подписок на авторов, а так же возможность подписки на интересующего автора.

## Запуск проекта на локальном репозитории
Клонировать репозиторий, cоздать и активировать виртуальное окружение:

`python -m venv venv`

`source venv/Scripts/activate`

## Установить зависимости:

`pip install -r requirements.txt`

## Выполнить миграции:

`python3 manage.py migrate`

## Как работать:

Запустите проект 

`python manage.py runserver`

После запуска проекта, документация будет доступна по адресу:

```
http://localhost:port/redoc/
```

Для неавторизованных пользователей доступно:

```
GET api/v1/posts/ - получить список всех публикаций.
При указании параметров limit и offset выдача должна работать с пагинацией
GET api/v1/posts/{id}/ - получение публикации по id

GET api/v1/groups/ - получение списка доступных сообществ
GET api/v1/groups/{id}/ - получение информации о сообществе по id

GET api/v1/{post_id}/comments/ - получение всех комментариев к публикации
GET api/v1/{post_id}/comments/{id}/ - Получение комментария к публикации по id
```
