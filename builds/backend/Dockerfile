# syntax=docker/dockerfile:1
FROM python:3.9.6
ENV PYTHONUNBUFFERED=1
RUN pip install --upgrade pip
WORKDIR /tranquillity
COPY Requirements.txt /tranquillity/

RUN pip install -r Requirements.txt
COPY tranquillity/ /tranquillity/

EXPOSE 8080

RUN python manage.py makemigrations
RUN python manage.py migrate

#CMD ["python", "manage.py", "runserver", "0.0.0.0:8080"]
#CMD ["gunicorn", "--env", "DJANGO_SETTINGS_MODULE=tranquillity.settings", "tranquillity.wsgi", "-b", ":8080", "--workers=4"]