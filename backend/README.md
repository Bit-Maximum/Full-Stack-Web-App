# 🧩 Practical Work #1: Backend API with Flask

[![en](https://img.shields.io/badge/lang-en-red.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-1-backend/backend/README.md)
[![ru](https://img.shields.io/badge/lang-ru-blue.svg)](https://github.com/Bit-Maximum/Full-Stack-Web-App/blob/stage-1-backend/backend/translation/README.ru.md)

### Maxim Merkurev
**Far Eastern Federal University, 2025**

---

## 📚 Course

**Engineering of Internet Systems**  
The goal of this stage is to develop a REST API using Flask that connects to a real dataset and supports full CRUD operations.

---

## 📊 Dataset Used

**Grocery Sales Database**  
Source: [Kaggle](https://www.kaggle.com/datasets/andrexibiza/grocery-sales-dataset)

---
## 🚀 Quick Start

### 🐳 Run with Docker

> Make sure [Docker](https://www.docker.com/) is installed.

1. Clone the repository and switch to the `stage-1-backend` branch:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-1-backend
git cd backend
```

2. Build the Docker image::

```bash
docker build -t flask-api-nse:latest .
```

3. Run the container:
```bash
docker run -p 5000:5000 flask-api-nse:latest
```
The API will be available at:
http://127.0.0.1:5000/

## 💻 (Alternative) Run Locally:

> Requires Python 3.8 or higher

1. Clone the repository and switch to the `stage-1-backend` branch:
```bash
git clone https://github.com/Bit-Maximum/Full-Stack-Web-App.git
git cd Full-Stack-Web-App

git checkout stage-1-backend
git cd backend
```

2. Install dependencies:

```bash
pip install -r requirements.txt
# or
poetry install
```

3. Start the server:

```bash
python app.py
```

The API will be available at:
http://127.0.0.1:5000/

## API Endpoints

### 1. City Endpoints (`/api/v1/cities`)

| Method  | URL                        | Description                           |
| ------ | -------------------------- | ---------------------------------- |
| GET    | `/api/v1/cities/`          | Get list of all cities       |
| GET    | `/api/v1/cities/<city_id>` | Get details of a specific city |
| POST   | `/api/v1/cities/`          | Add a new city                |
| PUT    | `/api/v1/cities/<city_id>` | Update city details             |
| DELETE | `/api/v1/cities/<city_id>` | Delete a city                      |

### Example Requests

#### Get all cities

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/cities/
```

#### Add a new city

```bash
curl -L -X POST http://127.0.0.1:5000/api/v1/cities/ \  
    -H "Content-Type: application/json" \  
    -d '{"name": "New City", "zipcode": 12345}'
```

## 2. Product Endpoints (`/api/v1/products`)

| Method | URL                    | Description                   |
| ----- | ---------------------- | -------------------------- |
| GET   | `/api/v1/products/max` | Get the most expensive product        |
| GET   | `/api/v1/products/min` | Get the cheapest product        |
| GET   | `/api/v1/products/avg` | Get average prices by category |

### Example Requests

#### Get the most expensive product

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/products/max
```

#### Get average prices by category

```bash
curl -L -X GET http://127.0.0.1:5000/api/v1/products/avg
```
