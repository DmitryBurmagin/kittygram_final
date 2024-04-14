# Kittygram

## Описание Проекта

Kittygram - это интернет-платформа, созданная специально для любителей кошек. Здесь владельцы могут регистрировать своих питомцев, предоставляя информацию о их имени, цвете, дате рождения и даже загружая фотографии. Кроме того, на платформе можно отмечать достижения каждого кота. Kittygram позволяет создать удобный реестр кошачьих питомцев, что делает его незаменимым инструментом для любого котовода.

## Инструкции по Запуску Проекта

1. Клонируйте репозиторий: `git clone https://github.com/DmitryBurmagin/kittygram_final.git`
2. Перейдите в директорию проекта: `cd kittygram_final`
3. Создайте файл `.env` в корне проекта со следующим содержимым:
    ```
    POSTGRES_DB=kittygram
    POSTGRES_USER=kittygram_user
    POSTGRES_PASSWORD=kittygram_password
    DB_HOST=db
    DB_PORT=5432
    SECRET_KEY= #Secret key django
    DEBUG= # True or False
    ALLOWED_HOSTS=127.0.0.1,localhost
    ```
4. Запустите Docker Compose: `docker-compose up -d`
5. Перейдите по адресу `http://localhost:8000/` в вашем браузере. Проект теперь доступен для использования.

## Примеры Запросов к API

- Добавить питомца: `POST /cats/add`
- Редактировать питомца: `PATCH /cats/edit`
- Просмотр питомца: `GET /cats/{cat_id}`

## Автор и Используемые Технологии

Автор проекта: **Дмитрий Бурмагин**

Используемые технологии:

- Django
- djangorestframework
- React
