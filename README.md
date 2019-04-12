# inetman28_microservices
inetman28 microservices repository

# Monitoring-2

https://cloud.docker.com/u/inetman28/repository/docker/inetman28/alertmanager
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/prometheus
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/post
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/comment
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/ui

В этой лабораторной работе я развернул мониторинг для моих микросервисом :), а именно:
- grafana
- alertmanager

Замониторил микросервисы, а также настроил алертинг с интеграцией в Slack. 

# monitoring-1

Репы образов на DockerHub:
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/prometheus
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/post
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/comment
https://cloud.docker.com/u/inetman28/repository/docker/inetman28/ui

В этой лабораторной работе я развернул систему мониторинга prometheus и смог замониторить свое приложение базовыми метриками.

# gitlab-ci-1

В этой лабораторной работе:
- поставил Gitlab CI в Docker
- сделал свой первый pipeline, который является CI/CD
pipeline, и когда-нибудь в следующих лабах сможет задеплоить приложение :) 

# docker-4

В этой лабораторной работе я научился управлять:
- сетью в docker
- импользовать docker-compose

Чтобы убрать префикс 'src_' из названия контейнеров - мне пришлось в docker-compose.yml добавить
переменную окружения 'COMPOSE_PROJECT_NAME=dockermicroservices'

# docker-3 

Запустил три (4) контейнера:
- 1 с БД
- 2 с post-py, который отвечает за посты 
- 3 с comment, который отвечает за комментарии
- 4 с ui, который отвечает за web-интерфейс

Для того, чтобы после перезапуска контейнера не пропадали данные, внесенные после старта контейнера, я подал в контейнер с БД - volume. 

# docker-2

Изоляция PID NS: Docker контейнер можно запустить с НЕ изолированным PID NS. Это даст нам видимость всех процессов на хостовой ОС из контейнера. 

В этой лаботорной работе я:
- Развернул тестовое приложение reddit в GCP и на локальной машине
- Запушил свой image в docker hub
- Убил pid 1, после чего контейнер схлопнулся 

# docker-1

В этой лабораторной работе я:
- установил Docker CE на виртуальную машину
- запустил свой тестовый контейнер "Hello World"
- научился деплоить контейнеры из image, которые стягиваются с docker hub
- конвертировать контейнер обратно в image
- научился базовым командам управления контейнерами: start, run, kill, rm, ps, exec... etc...
