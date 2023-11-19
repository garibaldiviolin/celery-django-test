# Redis

docker run --name some-redis -p 6379:6379 -d redis


# RabbitMQ

docker run -d --name some-rabbit -e RABBITMQ_DEFAULT_USER=user -e RABBITMQ_DEFAULT_PASS=password -p 5672:5672 rabbitmq:3-management


# celery worker

celery -A celery_django_test.celery worker -l INFO


# celery beat

celery -A celery_django_test.celery beat

# OK
