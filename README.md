# Project "АPI for Yatube"

## Technology stack: 

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python&logoColor=green)
![Django](https://img.shields.io/badge/Django-3.2.16-red?style=for-the-badge&logo=django&logoColor=blue)
![DjangoREST](https://img.shields.io/badge/DJANGO-REST-ff1709?style=for-the-badge&logo=django&logoColor=white&color=ff1709&labelColor=blue)
![JWT](https://img.shields.io/badge/JWT_Djoser-black?style=for-the-badge&logo=JSON%20web%20tokens)

### Description: 
API for the Yatube social network for authors and followers. The following functionality is implemented:  
- Viewing, creating, updating, and deleting posts and comments  
- Viewing community information  
- User subscriptions

### Starting the application:

Clone the project:

```bash
git clone https://github.com/Romaizega/yatube_api_final.git
```

Navigate to the project folder:

```bash
cd yatube_api_final
```

Install a virtual environment:

linux
```bash
python3 -m venv env
```
windows
```bash
python -m venv venv
```
Activate the virtual environment:

linux
```bash
source venv/bin/activate
```
windows
```bash
source venv/Script/activate
```
Install dependencies:

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

Apply migrations:

linux
```bash
python3 manage.py migrate
```
windows
```bash
python manage.py migrate
```
Run the project:

linux
```bash
python3 manage.py runserver
```
windows
```bash
python manage.py runserver
```
After starting the project, the API documentation for Yatube will be available at http://127.0.0.1:8000/redoc/. The documentation is provided in Redoc format.

### Example API requests:

Getting posts:

GET  http://127.0.0.1:8000/api/v1/posts/

Responses: 200 Successful request execution without pagination
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

### Author:
[Roman Izegov](https://github.com/Romaizega)
