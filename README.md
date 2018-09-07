# Django Docker

## Description

This defines and runs a multi-container Dockerized Django application that uses PostgreSQL and is served by Nginx.

## How to Use

TBA

### Initial Configuration

_outline of config steps: more details to come_

- change allowed_hosts in webapp/settings.py
- docker-compose exec app python manage.py migrate
- docker-compose exec app python manage.py collectstatic
- docker-compose exec app python manage.py createsuperuser
- change database name, user, password
- set `DJANGO_SECRET_KEY` environment variable in `docker/django/Dockerfile`
```
ENV DJANGO_SECRET_KEY 1234567890!@#$%^&*()MY!SUPER!SECET!KEY)(*&^%$#@!)
```
- ...
- ...
- ...
- change DEBUG to False