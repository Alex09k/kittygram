# Kittygram

## О проекте
**Это социальная сеть для обмена фотографиями любимых питомцев. Это полностью рабочий проект, который состоит из бэкенд-приложения на Django и фронтенд-приложения на React.**

## Технологии:
- Python 3.11.1 
- Django 4.1 
- Django REST framework 
- React 
- Docker 
- Nginx

## Запуск проекта на локальном компьютере

- 1 Для запуска проекта необходимо иметь установленные: 
- node.js 
- python 
- pip.

- 2 клонировать проект: git clone git@github.com:Alex09k/kittygram_final.git 
- frontend: cd frontend npm i rpm run dev
- backend: cd backend python -m venv venv


## Установка возможна при налиичи на локальом компьютере Docker compose

# Запустите проект из корня с помощью команды:
- docker compose up

# Соберите статику Django с помощью команды:
- docker compose exec backend python manage.py collectstatic

# Скопируйте статику командой:
- docker compose exec backend cp -r /app/collected_static/. /static/static/

# Приминить миграции:
- docker compose exec backend python manage.py migrate

# По адресу http://127.0.0.1:9000/ сайт будет доступен.
 
 ## Для взаимодействия с приложением через API предусмотрены следующие методы:

- /api/cats/ - принимает GET и POST, для добавления новых и получения существующих объектов
- /api/achievements/ - принимает GET и POST, для добавления новых и получения существующих навыков домашнего питомца
## Авторы:
- backend: yandex-practicum
- frontend: yandex-practicum
- DevOps: Кривов Александр
