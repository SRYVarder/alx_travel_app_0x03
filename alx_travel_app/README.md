# alx_travel_app_0x03

Django travel booking app extended with Celery background task management using RabbitMQ and email notifications.

## Features
- Celery configured with RabbitMQ
- Email confirmation sent asynchronously when a booking is created
- Fully compatible with Django REST Framework

## Setup
```bash
pip install -r requirements.txt
python manage.py migrate
rabbitmq-server
celery -A alx_travel_app worker --loglevel=info
python manage.py runserver
```
