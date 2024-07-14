## Django-проект для автоматической рассылки
Стек: 
* Python
* Django (приложения mailing, users, blog, django_apscheduler)
* PostgreSQL
* Redis
* Сервис рассылки smtp.yandex.ru

## Настройка проекта
После клонирования введите следующие команды (на винде, для другой системы команды отличаются) в консоли в папке проекта:

`python -m venv venv`

`venv/scripts/activate`

`pip install -r requirements.txt`

Конфигурировать переменные в .env.example, переименовать в .env

Не забудьте активировать миграции, чтобы связи с БД работали:

`python manage.py migrate`

Фикстуры загружать стандартной командой:

`python manage.py loaddata fixtures/шото-там.json`, 

json'ы находятся в папке fixtures в корне проекта

Кастом-команда для создания суперпользователя - `csu`
