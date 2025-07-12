# 🧩 Практическая работа №1: Backend API на Flask

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-1-backend/backend/README.md)
[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-1-backend/backend/translation/README.ru.md)

### Меркурьев Максим Андреевич
**Группа:** М9124-09.04.04рпис  
**Дальневосточный федеральный университет, 2025**

---

## 📚 Дисциплина

**Инженерия интернет-систем**  
Цель этапа — создать REST API на Flask с доступом к данным из реального датасета и реализацией CRUD-операций.

---

## 📊 Используемый датасет

**Grocery Sales Database**  
Источник: [Kaggle](https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset)

---
## 🚀 Быстрый запуск

### 🐳 Запуск с Docker

> Убедитесь, что установлен [Docker](https://www.docker.com/)

1. Клонируйте репозиторий и переключитесь на ветку `stage-1-backend`:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-1-backend
git cd backend
```

2. Сборка образа:

```bash
docker build -t flask-api-nse:latest .
```

3. Запуск контейнера:
```bash
docker run -p 5000:5000 flask-api-nse:latest
```
API будет доступен по адресу:
http://127.0.0.1:5000/

## 💻 (Альтернативно) Запуск локально:

> Требуется Python 3.8 или выше

1. Клонируйте репозиторий и переключитесь на ветку `stage-1-backend`:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-1-backend
git cd backend
```

2. Установка зависимостей:

```bash
pip install -r requirements.txt
# или
poetry install
```

3. Запуск сервера:

```bash
python app.py
```

API будет доступен по адресу:
http://127.0.0.1:5000/

## API Эндпоинты

### 1. Эндпоинты городов (`/api/v1/cities`)

| Метод  | URL                        | Описание                            |
| ------ | -------------------------- | ----------------------------------- |
| GET    | `/api/v1/cities/`          | Получить список всех городов        |
| GET    | `/api/v1/cities/<city_id>` | Получить данные о конкретном городе |
| POST   | `/api/v1/cities/`          | Добавить новый город                |
| PUT    | `/api/v1/cities/<city_id>` | Обновить данные города              |
| DELETE | `/api/v1/cities/<city_id>` | Удалить город                       |

### Примеры запросов

#### Получить список городов

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/cities/
```

#### Добавить новый город

```bash
curl -L -X POST http://127.0.0.1:5000/api/v1/cities/ \  
    -H "Content-Type: application/json" \  
    -d '{"name": "New City", "zipcode": 12345}'
```

## 2. Эндпоинты товаров (`/api/v1/products`)

| Метод | URL                    | Описание                   |
| ----- | ---------------------- | -------------------------- |
| GET   | `/api/v1/products/max` | Самый дорогой товар        |
| GET   | `/api/v1/products/min` | Самый дешевый товар        |
| GET   | `/api/v1/products/avg` | Средняя цена по категориям |

### Примеры запросов

#### Получить самый дорогой товар

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/products/max
```

#### Получить среднюю цену по категориям

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/products/avg
```
