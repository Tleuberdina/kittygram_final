###Kittygram - проект, в котором реализован запуск в контейнерах на удаленном сервере. При пуше в ветку main проект автоматически тестируется, в случае успешного тестирования образы обновляются, на сервере запущены контейнеры из обновленных образов, при успешном завершении всех этапов направляется сообщение мне в Telegram.

###Инструкция по развертыванию проекта в Docker

Предварительные требования
Установленный Docker и Docker Compose

Шаги развертывания
Клонируйте репозиторий: git clone git@github.com:Tleuberdina/kittygram_final.git
cd foodgram
Постройте и запустите контейнеры: docker-compose up -d --build
Выполните миграции: docker-compose exec web python manage.py migrate
Откройте проект в браузере по адресу: http://localhost:8000/

###Технологии:
Python
Django
DRF
PyYAML
Docker
Docker Hub
CI/CD
GitHub Actions
Nginx
PostgreSQL
