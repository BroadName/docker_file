## Задание 1
Создание docker image с http сервером nginx:

```bash
docker run -d -p 8888:80 -v ${PWD}/test_html:/usr/share/nginx/html nginx
```
Проверяем приветственную страничку nginx:
```bash
curl.exe localhost:8888/
```
## Задание 2
### Создание контейнера для проекта
Собираем Docker образ при помощи докер-файла
```bash
docker build . --tag=my_app:1.0
```

Запускаем контейнер

```base
docker run -d -p 8000:8000 my_app:1.0
```
Тестируем функционал используя Postman или другие доступные инструменты.