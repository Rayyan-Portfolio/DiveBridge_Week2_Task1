# DiveBridge_Week2_Task1

## 📝 Blog API – Built with Django & Django REST Framework

This project is a fully functional **Blog API** built using **Django 5.2** and **Django REST Framework (DRF)**. It supports full CRUD operations (Create, Read, Update, Delete) for blog posts via a clean, RESTful API interface.

> 🔗 **Live Demo (Frontend/Client)**: [https://dive-bridge-week2-task1.vercel.app](https://dive-bridge-week2-task1.vercel.app)

---

## ⚙️ Tech Stack

- **Python 3.13**
- **Django 5.2**
- **Django REST Framework 3.16**
- SQLite (default dev database)

---

## 📁 Features

- ✅ Create, Read, Update, Delete blog posts
- ✅ DRF-powered browsable API UI
- ✅ Admin dashboard for managing posts
- ✅ Clean model-view-serializer-router structure

---

## 📦 API Endpoints

| Method | Endpoint           | Description         |
| ------ | ------------------ | ------------------- |
| GET    | `/api/posts/`      | List all blog posts |
| POST   | `/api/posts/`      | Create a new post   |
| GET    | `/api/posts/<id>/` | View a single post  |
| PUT    | `/api/posts/<id>/` | Update a post       |
| DELETE | `/api/posts/<id>/` | Delete a post       |

Test using browser, Postman, or frontend app.

---

## 🚀 How to Run the Project Locally

### 1. Clone the Repo

```bash
git clone <your-repo-url>
cd DiveBridge_Week2_Task1
```

### 2. Create Virtual Environment

```bash
python3 -m venv env
source env/bin/activate
```

### 3. Install Dependencies

```bash
pip install django djangorestframework
```

### 4. Apply Migrations

```bash
python3 manage.py makemigrations
python3 manage.py migrate
```

### 5. Create Superuser

```bash
python3 manage.py createsuperuser
```

### 6. Run Development Server

```bash
python3 manage.py runserver
```

Go to:

- **Admin Panel** → http://127.0.0.1:8000/admin/
- **API Endpoint** → http://127.0.0.1:8000/api/posts/

---

## 🧠 How It Was Built

### ➤ Step 1: Project & App Setup

- Started with `django-admin startproject blog_api .`
- Created a modular app `blog`

### ➤ Step 2: Model Creation

- Defined a `Post` model with `title`, `content`, `created_at`
- Registered in `admin.py` for dashboard use

### ➤ Step 3: REST API Logic

- Used **DRF's `ModelSerializer`** to convert data into JSON
- Created a `PostViewSet` to provide all CRUD logic
- Registered the viewset with a **`DefaultRouter`** to auto-generate routes

### ➤ Step 4: Testing

- Used DRF’s browsable API to interact with the backend
- Tested endpoints with Postman and via frontend client

---

## ✅ Lessons Learned

- The power of Django's MVT architecture
- How serializers convert between models and JSON
- How DRF simplifies RESTful CRUD APIs with minimal code
- How to connect APIs to external frontend (see [vercel app](https://dive-bridge-week2-task1.vercel.app))

---

## 📬 Contact

**Ahmad Rayyan**  
Built as part of my backend development learning path using [Mosh’s Django Course](https://www.youtube.com/watch?v=F5mRW0jo-U4) 🚀
