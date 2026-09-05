# Django Blog

A full-stack blog application built with **Python, Django, and PostgreSQL**. The project allows users to create and manage blog posts, interact through comments, and authenticate through a user registration and login system.

## Features

### 🔐 User Authentication

* User registration
* User login and logout
* Django's built-in authentication system
* Authentication required for creating posts
* Users can manage their own posts

### 📝 Blog Posts

* View all published posts on the home page
* View individual posts
* Create new posts
* Edit existing posts
* Delete posts
* Posts are associated with their authors
* Post creation and editing are handled through Django ModelForms

### 💬 Comments

* Add comments to individual posts
* Display comments on post detail pages
* Comments are linked to their corresponding posts

### 🎨 User Interface

* Django template inheritance
* Reusable templates and navigation
* Custom styling
* Static assets for the front-end
* Separate pages for authentication, post creation, editing, deletion, and post details

## 🛠️ Technologies

 **Python**            Backend programming    
 **Django 6.1**        Web framework          
 **PostgreSQL**        Relational database    
 **HTML**              Page structure         
 **CSS**               Styling               
 **Django Templates**  Dynamic page rendering 



## 🗄️ Database Models

The application uses Django's ORM to manage its database.

### Post

Each post contains:

* Title
* Content
* Creation date
* Author

Posts are associated with Django's built-in `User` model.

### Comment

Each comment contains:

* Username
* Comment content
* Associated post

Comments have a relationship with their corresponding posts, allowing comments to be retrieved directly from a post.


The application uses Django views, forms, models, URL routing, and templates to connect these parts together.

## 🚀 Getting Started

### Prerequisites

Make sure you have installed:

* Python 3.10+
* PostgreSQL
* Git

### 1. Clone the repository

```bash
git clone https://github.com/lanabasuni/django-blog.git
cd django-blog
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

On Windows:

```bash
.venv\Scripts\activate
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Configure PostgreSQL

Create a PostgreSQL database and configure the database connection in your Django settings.

**Do not commit database passwords, secret keys, or other credentials to GitHub.**

### 5. Apply migrations

```bash
python manage.py makemigrations
python manage.py migrate
```

### 6. Create an administrator account

```bash
python manage.py createsuperuser
```

### 7. Run the development server

```bash
python manage.py runserver
```

Then open:

```text
http://127.0.0.1:8000/
```

## 🧠 What I Learned

Building this project helped me practice:

* Django project and app structure
* Django's Model-View-Template architecture
* Relational database design
* Django ORM and model relationships
* PostgreSQL integration
* User authentication
* Forms and ModelForms
* CRUD operations
* URL routing
* Template inheritance
* Static files
* Git and GitHub workflow

## 🔮 Future Improvements

Possible future improvements include:

* Add post search and filtering
* Add categories and tags
* Add pagination
* Improve comment management
* Add user profile pages
* Add profile images
* Improve form validation and error handling
* Add automated tests for models, forms, and views
* Deploy the application for public access

## 👩‍💻 Author

**Lana Basuni**

Computer Science & AI Student

GitHub: [@lanabasuni](https://github.com/lanabasuni)
