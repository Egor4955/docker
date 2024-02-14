FROM python:3.11-alpine

WORKDIR /app

COPY . .

RUN pip3 install --no-cache-dir --upgrade  -r requirements.txt

CMD python manage.py makemigrations
CMD python manage.py migrate

CMD gunicorn stocks_products.wsgi:application -b 0.0.0.0:8000