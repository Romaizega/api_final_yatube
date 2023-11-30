# Проект "АPI для Yatube"

## Стек технологий: 

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=green)
![Django](https://img.shields.io/badge/Django-3.2.16-red?style=for-the-badge&logo=django&logoColor=blue)
![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=blue)
![JWT](https://img.shields.io/badge/JWT_Djoser-black?style=for-the-badge&logo=JSON%20web%20tokens)

### Описание:
АPI социальной сети Yatube для авторов и подписчиков. Реализован функционал:
Просмотр, создание, обновление, удаление публикаций и комментарий;
Просмотр информации о сообществах;
Подписка пользователей;

### Запуск приложения:

Клонируем проект:

```bash
git clone https://github.com/Romaizega/yatube_api_final.git
```

Переходим в папку с проектом:

```bash
cd yatube_api_final
```

Установить виртуальное окружение:

linux
```bash
python3 -m venv env
```
windows
```bash
python -m venv venv
```
Активировать виртуальное окружение:

linux
```bash
source venv/bin/activate
```
windows
```bash
source venv/Script/activate
```
Установить зависимости:

linux
```bash
python3 -m pip install --upgrade pip
```
windows
```bash
python -m pip install --upgrade pip
```
```bash
pip install -r requirements.txt
```

Выполнить миграции:

linux
```bash
python3 manage.py migrate
```
windows
```bash
python manage.py migrate
```
Запустить проект:

linux
```bash
python3 manage.py runserver
```
windows
```bash
python manage.py runserver
```
После запуска проекта,  по адресу  http://127.0.0.1:8000/redoc/ будет доступна документация для API Yatube. Документация представлена в формате Redoc. 

### Пример запросов к API:

Получение публикаций

GET  http://127.0.0.1:8000/api/v1/posts/

Responses: 200 Удачное выполнение запроса без пагинации 
```bash
{
  "count": 123,
  "next": "http://api.example.org/accounts/?offset=400&limit=100",
  "previous": "http://api.example.org/accounts/?offset=200&limit=100",
  "results": [
    {
      "id": 0,
      "author": "string",
      "text": "string",
      "pub_date": "2021-10-14T20:41:29.648Z",
      "image": "string",
      "group": 0
    }
  ]
}
```

### Автор:
[Р.Г. Изегов](https://github.com/Romaizega)