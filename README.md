# My First Django Website

This is my first project using the Django framework. It's a simple news website with basic functionality for creating, 
reading, updating, and deleting news articles.

---

## Features

- **Home Page** – main page of the website.
- **About Us** – information about the creators or the project.
- **News Page** – displays a list of news articles.
  - Add new news
  - Edit existing news
  - Delete news

---

## Technologies Used

- Python
- Django
- SQLite (default database)
- HTML / CSS
- Bootstrap (for styling)

---

## Project Structure

```
djweb
    ├───djweb    # Project settings and config
    │   ├───__init__.py
    │   ├───asgi.py
    │   ├───settings.py
    │   ├───urls.py
    │   └───wsgi.py
    ├───main    # Main app (e.g. homepage, about page)
    │   ├───migrations
    │   │   └───__init__.py
    │   ├───static
    │   │   └───main
    │   │       ├───css
    │   │       │   └───main.css
    │   │       ├───img
    │   │       │   └───logo.png
    │   │       └───js
    │   ├───templates
    │   │   └───main
    │   │       ├───about.html
    │   │       ├───index.html
    │   │       └───layout.html
    │   ├───__init__.py
    │   ├───admin.py
    │   ├───apps.py
    │   ├───models.py
    │   ├───tests.py
    │   ├───urls.py
    │   └───views.py
    └───news    # News app (CRUD functionality)
    │   ├───migrations
    │   │   ├───0001_initial.py
    │   │   └───__init__.py
    │   ├───templates
    │   │   └───news
    │   │       ├───create.html
    │   │       ├───details_view.html
    │   │       ├───news_delete.html
    │   │       └───news_home.html
    │   ├───__init__.py
    │   ├───admin.py
    │   ├───apps.py
    │   ├───forms.py
    │   ├───models.py
    │   ├───tests.py
    │   ├───urls.py
    │   └───views.py
    ├───db.sqlite3    # SQLite database
    └───manage.py    # Django management script
```

---

## How to Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/your-repo-name.git 
   cd your-repo-name
   
2. Create and activate a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
   
3. Install dependencies:

    ```bash
    pip install -r requirements.txt
   
4. Apply migrations:

    ```bash
    python manage.py migrate
   
5. Run the development server:

    ```bash
    python manage.py runserver
   
6. Open your browser and go to: http://127.0.0.1:8000/

---

## Admin Panel

To access the admin panel:

1. Create a superuser:

    ```bash
    python manage.py createsuperuser
   
2. Go to: http://127.0.0.1:8000/admin

---

## Testing

You can test the functionality of adding, editing, and deleting news articles through the News page or the admin panel.
