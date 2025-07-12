# 🎨 Практическая работа №2: React MUI Frontend (Multipage SPA)

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-2-frontend/frontend/README.md)
[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-2-frontend/frontend/translation/README.ru.md)

### Меркурьев Максим Андреевич
**Группа:** М9124-09.04.04рпис  
**Дальневосточный федеральный университет, 2025**

---

## 📚 Дисциплина

**Инженерия интернет-систем**  
Цель этапа — разработка клиентской части (frontend) веб-приложения с использованием **React** и **Material UI**.

---

## 🚀 Быстрый запуск

### 🐳 Запуск с Docker

> Убедитесь, что установлен [Docker](https://www.docker.com/)

1. Клонируйте репозиторий и переключитесь на ветку `stage-2-frontend`:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-2-frontend
git cd backend
```

2. Сборка образа:
```bash
docker build -t nse-task-3:latest .
```
3. Запуск контейнера:
```bash
docker run -p 3000:3000 nse-task-3:latest
```

После запуска приложение будет доступно по адресу:
http://localhost:3000

## 💻 (Альтернативно) Запуск локально:

> Перед началом убедитесь, что у вас установлены **Node.js** (рекомендуемая версия 16+) и **npm**.

1. Клонируйте репозиторий и переключитесь на ветку `stage-2-frontend`:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-2-frontend
git cd backend
```

2. Установите зависимости:
```bash
npm install
```

3. Запустите приложение:
```bash
npm start
```

## 🧱 Используемые технологии
* React (SPA)
* React Router DOM
* Material UI (v5)
* Адаптивная вёрстка
