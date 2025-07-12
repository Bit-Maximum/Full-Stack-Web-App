# 🌐 Full Stack Web App: Flask + React

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/main/README.md)
[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/main/translation/README.ru.md)

🧪 _Проект в рамках курса "Инженерия интернет-систем"_  
🧱 Полноценное full-stack веб-приложение, разработанное поэтапно в рамках трёх практических заданий.  
📦 Состоит из backend-части (Python + Flask + REST API) и frontend-части (React + MUI), объединённых с помощью Docker Compose.

---

## 📚 Цель проекта

Создание полнофункционального клиент-серверного приложения: от проектирования API до реализации интерфейса и контейнеризации.

Проект выполнен в 3 этапа:

| Этап | Название             | Краткое описание |
|------|----------------------|------------------|
| 1    | Backend (API)        | Реализация REST API на Flask, работа с Kaggle-датасетом |
| 2    | Frontend (React SPA) | Создание веб-интерфейса на React с использованием Material UI |
| 3    | Интеграция FE и BE   | Связка интерфейса и API, тестирование взаимодействия |

---

## 🛠️ Используемые технологии

**Backend:**
- Python 3
- Flask + Flask-RESTful
- CORS, JSON-сериализация

**Frontend:**
- React
- MUI (Material UI)

## ▶️ Быстрый запуск через Docker

### Предварительные требования
- Установленный [Docker](https://docs.docker.com/get-docker/)
- Установленный [Docker Compose](https://docs.docker.com/compose/install/)

### 📝 Инструкция
1. Клонировать репозиторий:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
cd Full-Stack-Web-App
```

2. Собрать и запустить проект:
```bash
docker-compose up --build
```

Приложение будет доступно по адресу:
http://localhost:3000

>_Frontend будет отправлять запросы на backend, доступный внутри контейнера по http://localhost:5000._

## 🔍 Просмотр отдельных этапов разработки:

### Для просмотра отдельно REST API сервера перейдите в ветку `stage-1-backend`:
[backend/README.md](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-1-backend/backend/README.md)

### Для просмотра отдельно REST API сервера перейдите в ветку `stage-1-backend`:
[backend/README.md](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-2-frontend/frontend/README.md)

## 💡Описание сервисов

### 🧩 Backend API:
* Создано REST API на Flask
* Загружен и обработан датасет с Kaggle
* Реализованы CRUD операции
* Реализована обработка ошибок и CORS


### 🧩 Frontend:
* Разработан интерфейс на React
* Использован UI-фреймворк Material UI
* Добавлена таблица, фильтры, детализация

## 📷 Галерея

<img src="media/1.png" width="45%"></img> <img src="media/2.png" width="45%"></img> <img src="media/3.png" width="45%"></img> <img src="media/4.png" width="45%"></img>

## 👤 Автор
Меркурьев Максим Алексеевич
**Дальневосточный федеральный университет, 2025**