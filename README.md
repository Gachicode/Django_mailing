## Требования

- python=3.8.10

## Настройка и установка проекта

1. Склонировать репозиторий
2. Установить **poetry**:
   ```
   pip3 install poetry
   ```
3. Активировать виртуальное окружение:
   ```
   poetry shell
   ```
4. Установить зависимости:
   ```
   poetry install
   ```
5. Установить Docker и docker-compose
6. Запустить сервисы в Docker (PostgreSQL, Redis):
7. Применить миграции:
   ```
   python3 src/manage.py migrate
   ```
8. Запустить сервер приложения:
    ```
    python3 src/manage.py runserver
    ```
9. При необходимости запустить Celery:
    ```
    cd src && celery -A automailing worker -B -l INFO
    ```
