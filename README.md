## Сборка nginx
В директории Task1
```
docker build --tag ng .
docker run -d -p 80:80 --name my_nginx ng
```
перейти в http://127.0.0.1

## Сборка django-проекта
В директории Task2 
```
docker build --tag django_project:1.0 ./
docker run -p 8000:8000 -d --name django_server django_project:1.0
```
перейти в http://127.0.0.1:8000/api/v1/
