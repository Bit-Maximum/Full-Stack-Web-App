# 🎨 Practical Work #2: React MUI Frontend (Multipage SPA)

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-2-frontend/frontend/README.md)
[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-2-frontend/frontend/translation/README.ru.md)

### Maxim Merkurev
**Far Eastern Federal University, 2025**

---

## 📚 Course

**Engineering of Internet Systems**  
The goal of this stage is to develop the frontend of a web application using **React** and **Material UI**.

---

## 🚀 Quick Start

### 🐳 Run with Docker

> Make sure [Docker](https://www.docker.com/) is installed.

1. Clone the repository and switch to the `stage-2-frontend` branch:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-2-frontend
git cd backend
```

2. Build the Docker image:
```bash
docker build -t nse-task-3:latest .
```
3. Run the container:
```bash
docker run -p 3000:3000 nse-task-3:latest
```

Once launched, the app will be available at:
http://localhost:3000

## 💻 (Alternatively) Run Locally:

> Make sure **Node.js** (version 16 or higher) and **npm** are installed.

1. Clone the repository and switch to the `stage-2-frontend` branch:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-2-frontend
git cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm start
```

## 🧱 Technologies Used
* React (SPA)
* React Router DOM
* Material UI (v5)
* Responsive layout
