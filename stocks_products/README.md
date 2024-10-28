API Server по управлению складами и наличием продуктов внутри них

Инструкция по запуску контейнера

1. Склонируйте репозиторий 
   
```bash
git clone https://github.com/username/warehouse.git
cd warehouse

2. Создайте файл .env на основе .env.example и отредактируйте его при необходимости.

3. Соберите Docker-контейнер

```bash
docker build -t warehouse-api .

4. Запустите контейнер

```bash
docker run -p 8000:8000 --env-file .env warehouse-api

После запуска контейнер будет доступен по адресу http://localhost:8000
