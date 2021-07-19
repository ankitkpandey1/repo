# repo
Contains Docker file to build images.
Builds contain following images:
1. Backend - Django code base
2. Rabbit - Rabbitmq image with configuration
3. Worker - Backend + celery
4. API - Backend + gunicorn

For build images:
1. Go to Builds folder.
2. Go to backend and run `docker build -t backend .`
3. Go to Worker and api folders and run `docker build -t worker .` && `docker build -t api .`.
4. Go to Rabbit folder and build `docker build -t my-rabbit .`
