# Платформа торговой сети электроники EL shop
### Клонируйте репозиторий
- заранее перейдите в папку где будет находиться это приложение
- клонируйте репозиторий используя команду `git clone git@github.com:sam2486555/El_shop.git`
### Перейдите в проект командой
- `cd El_shop/`
- Установить зависимости из файла requirements.txt командой `pip install -r requirements.txt`
- В файл `.env.sample` внесите свои данные и переименуйте его в `.env`
### Настройки django
- SECRET_KEY= секретный ключ от приложения django
- DEBUG= режим отладки включен или выключен
### Настройки базы данных
POSTGRES_DB= имя базы данных
POSTGRES_USER= пользователь базы данных
POSTGRES_PASSWORD= пароль от базы данных
POSTGRES_HOST=db хост указан в файле docker-compose.yml
POSTGRES_PORT= порт
- Примените миграции используя команду `python manage.py migrate`
- Для доступа к административной странице нужно создать суперпользователя командой `python manage.py csu`
- Для запуска проекта наберите в терминале команду `python manage.py runserver`
- далее перейдите по ссылке http://0.0.0.0:8000/admin/ и войдите как админ в админ-панель
- Документация API доступна после запуска сервера по адресу: http://localhost:8000/redoc/ или http://localhost:8000/swagger/
### Для запуска через docker введите команды
- `docker compose up -d --build` или `sudo docker compose up -d --build`
- далее перейдите по ссылке http://0.0.0.0:8000/admin/ и войдите как админ в админ-панель
### Для остановки docker контейнера введите
`ctrl+c`

