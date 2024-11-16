# cw_drf
Курсовая работа по DRF DJANGO (good habbits)


### работают следующие команды для Windows с celery и celery-beat
`celery -A config worker --loglevel=info -E -P eventlet`

`celery -A config beat -l info -S django`

***
1. Запустить докер

* `docker run -p 8080:80 nginx:latest`

2. Задать настройки приложения в `docker-compose.yaml`

3. Заполняем файл .env по примеру .env.example

4. Создать образ и запускаем контейнеры

* `docker-compose up -d --build`

5. Проверяем работоспособность в браузере

* `http://localhost:8000/swagger/`