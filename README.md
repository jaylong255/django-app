# django-app

This is almost a fork of the hello django repo to get started. I mainly wanted to setup a docker compose config for django, postgres, redis, and maybe some other services and this was a pretty simple boilerplate that demonstrates django and connects to postgres. 

## Commands
- `docker-compose up --build`
- `docker-compose run django /opt/venv-hellodjango/bin/python manage.py migrate`
- `docker-compose run django /opt/venv-hellodjango/bin/python manage.py createsuperuser`

