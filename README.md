# Задание 1 
    winpty docker build -t nginx .
    docker run -d -p 8090:80 --name my_nginx nginx
    curl localhost:8090

# Задание 2 
    winpty docker build -t rest_api .
    winpty docker run -d -p 8000:8000 --name stokcs rest_api
