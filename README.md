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
- change secret_key in webapp/settings.py
    + environment variable?
- ...
- ...
- ...
- change DEBUG to False