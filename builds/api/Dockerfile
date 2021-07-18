FROM tranquillity:latest

EXPOSE 8080

CMD ["gunicorn", "--env", "DJANGO_SETTINGS_MODULE=tranquillity.settings", "tranquillity.wsgi", "-b", ":8080", "--workers=4"]