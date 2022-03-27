# django-celery
Django with celery and rabbitmq to demo how to asynchronously handle a heavy load or process

by passing the load to the queue so to be executed in the background there by keeping the 

server ready to respond to new requests.

#instructions

pip install -r requirements.txt

python manage.py migrate

python manage.py runserver

celery -A mysite worker -l info

Make sure you have RabbitMQ service running.

rabbitmq-server
