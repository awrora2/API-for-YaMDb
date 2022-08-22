# API для YaMDb
API для блога, который позволяет оставлять отзывы на произведения, на основе которых составляется его общий рейтинг. 

## Getting Started:
Клонировать репозиторий и перейти в него в командной строке:
```
git clone https://github.com/awrora2/API_for_YaMDb.git
```
Установить и активировать виртуальное окружение:
```
python3 -m venv env
source env/bin/activate
python3 -m pip install --upgrade pip
```
Установить зависимости из файла requirements.txt
```
python -m pip install --upgrade pip
pip install -r requirements.txt
```
Выполнить миграции:
```
python manage.py migrate
```
В папке с файлом manage.py выполнить команду:
```
python manage.py runserver
```
Для загрузки тестовых данных из csv-файлов выполнить команду:
```
python manage.py load_data
```
## Prerequisites:
```
Django==2.2.16
pytest==6.2.4
pytest-pythonpath==0.7.3
pytest-django==4.4.0
djangorestframework==3.12.4
djangorestframework-simplejwt==4.7.2
Pillow==8.3.1
PyJWT==2.1.0
requests==2.26.0
```

### Examples:

В рамках API YaMDb реализованы следующие ресурсы:
- аутентификация;
- отзывы на произведения;
- комментарии к отзывам.

Документация доступна после запуска по адресу:
```
http://127.0.0.1/redoc/
```
