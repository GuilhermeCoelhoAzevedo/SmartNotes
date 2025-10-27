# 🧠 SmartNotes

SmartNotes is a full-stack **Django web application** that allows users to **create, view, edit, and manage notes**.  
It includes authentication, note visibility control (private/public), and a simple like system — all built with clean and maintainable Django patterns.

## 🚀 Features

- ✍️ **User authentication** (signup, login, logout)
- 🗒️ **CRUD operations** for notes (create, read, update, delete)
- ❤️ **Like system** for each note
- 🌐 **Public or private visibility** toggle for notes
- 🧭 **Class-based views** for clean, reusable logic
- 🎨 **Responsive interface** using Bootstrap 5
- 🗄️ **SQLite3 database** with Django ORM
- 🧰 **Django Admin panel** for managing notes and users

---

## 🛠 Requirements

- **Python 3.13+**
- **Django 5.2.7+**

To install all required packages:

```bash
pip install -r requirements.txt
```

---

## 🛢️ Setting up the database

After setting up your environment:

```bash
# Activate your virtual environment
source .venv/bin/activate     # macOS/Linux
# or
.venv\Scripts\activate        # Windows

#Installing requirements
pip install -r requirements.txt

#Creating migrations
python manage.py makemigrations

#Saving migrations in the database
python manage.py migrate
```
---

## 🚀 Running the App

To start the app, run the following command:

```bash
# Run the app
python manage.py runserver
```

Once the app starts, visit:  
👉 http://127.0.0.1:8080

---

## 🧑 Create a superuser (optional, for admin access)
```bash
# Run the app
python manage.py createsuperuser
```

## 📂 Project Structure
```bash
Django-esst/
├── home/             # App for homepage and user authentication
│   ├── migrations/
│   ├── templates/    # Templates (login, signup, etc.)
│   ├── admin.py
│   ├── apps.py
│   ├── models.py    
│   ├── tests.py
│   ├── urls.py       # App routing
│   └── views.py      # Login, logout, signup, and welcome views
│
├── notes/            # App for user notes
│   ├── migrations/
│   ├── templates/    # Templates for CRUD pages
│   ├── admin.py
│   ├── apps.py
│   ├── forms.py      # NotesForm for validation
│   ├── models.py     # Notes model
│   ├── tests.py
│   ├── urls.py       # App routing
│   └── views.py      # CRUD and like/visibility views
│
├── smartnotes/       # Main Django project folder
│   ├── asgi.py
│   ├── settings.py   # Project settings
│   ├── urls.py       # Global routing
│   └── wsgi.py
│
├── static/           # Static files (CSS, base.html)
│   ├── css/
│   └── templates/
│
├── manage.py         # Django’s command-line utility
├── README.md
└── requirements.txt  # Python dependencies
```

---

## 🧰 Key Technologies

- **Django** – Web framework
- **Django Authentication System** – authentication
- **Django ORM** – Data modelling 
- **Django Generic Class-Based Views (CBVs)** – CRUD Operations 
- **Django Templating Engine** – Rendering dynamic HTML templates

---

## 🧑‍💻 Development Notes

- Always activate your virtual environment before running Django.
- Course link: [link](https://www.linkedin.com/learning-login/share?account=2189292&forceAccount=false&redirect=https%3A%2F%2Fwww.linkedin.com%2Flearning%2Fdjango-essential-training-25094632%3Ftrk%3Dshare_ent_url%26shareId%3D7WX6qeJQTBeHRIJ244RQbw%253D%253D)