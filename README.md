# Blogicum

Учебный проект на Django: блог с категориями, геометками и пользователями.

# Видео

Видео проекта - https://disk.yandex.ru/d/Cj22DESG4ajMeQ

## Возможности

- Главная страница с последними публикациями
- Страница отдельной публикации
- Страница публикаций по категории
- Админка с удобным управлением моделями
- Русская локализация

## Установка

1. Клонируйте репозиторий:
   ```
   git clone <repo_url>
   cd django-sprint3
   ```

2. Создайте и активируйте виртуальное окружение:
   ```
   python3 -m venv venv
   source venv/bin/activate
   ```

3. Установите зависимости:
   ```
   pip install -r requirements.txt
   ```

4. Примените миграции:
   ```
   python manage.py makemigrations
   python manage.py migrate
   ```

5. (Опционально) Загрузите тестовые данные:
   ```
   python manage.py loaddata db.json
   ```

6. Запустите сервер:
   ```
   python manage.py runserver
   ```

7. Откройте [http://127.0.0.1:8000/](http://127.0.0.1:8000/) в браузере.

## Структура моделей

- **Post** — публикация (заголовок, текст, дата публикации, автор, категория, местоположение, опубликовано, дата создания)
- **Category** — категория (заголовок, описание, slug, опубликовано, дата создания)
- **Location** — геометка (название, опубликовано, дата создания)
- **User** — пользователь (используется стандартная модель Django)

## Админка

- Для доступа используйте `/admin/`
- Все основные поля моделей выведены в списки, доступны фильтры и поиск

## Константы

- Все магические числа и параметры вынесены в `blog/constants.py`

## Локализация

- Интерфейс и админка на русском языке

---

**Для вопросов и предложений:**  
Пишите в issues или pull requests.
