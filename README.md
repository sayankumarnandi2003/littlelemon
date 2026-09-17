🍋 Little Lemon Restaurant Web Application

A full-stack web application built with Django, HTML5, CSS3, and JavaScript for Little Lemon — a charming Mediterranean restaurant located in Chicago, Illinois.

📌 Project Overview

This application serves as the interactive digital storefront and table reservation portal for Little Lemon. It allows patrons to explore the restaurant's background, view menu offerings, and book table reservations seamlessly online.

✨ Features & Functionality
Home Page (/) — Welcoming hero banner, featured dishes, and highlights of the Mediterranean dining experience.
About Page (/about/) — Shares the heritage, story, and culinary vision of Little Lemon's co-founders, Mario and Adrian.
Table Reservation System (/book/) — An interactive booking form (BookingForm) that lets customers reserve a table with their name, guest count, and special requests, backed by a Booking model.
Responsive Design — Polished UI with custom CSS styling and static assets (images, icons, typography).
Django Admin — Manage bookings and site content through Django's built-in admin panel.
🛠️ Tech Stack & Dependencies
Layer	Technology
Backend Framework	Django 4.x
Language	Python 3.10+
Frontend	HTML5, CSS3, JavaScript
Database	SQLite3 (default Django relational database)
Environment / Packages	pipenv or pip + venv
🚀 Installation & Setup Guide
1. Prerequisites

Ensure you have Python 3.10+ and pip installed on your machine.

2. Clone the Repository
bash
git clone https://github.com/your-username/littlelemon.git
cd littlelemon
3. Set Up a Virtual Environment & Install Dependencies

Using pipenv:

bash
pipenv install
pipenv shell

Or using standard venv:

bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
pip install django
4. Apply Database Migrations
bash
python manage.py makemigrations
python manage.py migrate
5. Run the Local Development Server
bash
python manage.py runserver

Then navigate to http://127.0.0.1:8000/ in your browser to access the application.

📂 Project Directory Structure
littlelemon/
│
├── littlelemon/                 # Project configuration directory
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py              # Core settings & app configuration
│   ├── urls.py                  # Root URL routing
│   └── wsgi.py
│
├── restaurant/                  # Core restaurant application
│   ├── admin.py                 # Django admin registrations
│   ├── apps.py
│   ├── forms.py                 # BookingForm model form definition
│   ├── models.py                # Database models (Booking, Menu)
│   ├── tests.py                 # Unit tests
│   ├── urls.py                  # App-level URL routing
│   ├── views.py                 # Request handlers & template renderers
│   │
│   ├── static/                  # Static assets
│   │   ├── css/
│   │   │   └── style.css
│   │   └── img/                 # Restaurant & menu image assets
│   │
│   └── templates/               # HTML templates
│       ├── about.html
│       ├── base.html
│       ├── book.html
│       ├── index.html
│       └── partials/            # Header & footer partials
│           ├── _header.html
│           └── _footer.html
│
├── db.sqlite3                   # SQLite database file
├── manage.py                    # Django management script
├── Pipfile
└── README.md                    # Project documentation
🗺️ Roadmap
 Define and migrate the Menu model referenced in views.py
 Add a dynamic menu listing page
 Add form validation feedback and a booking confirmation page
 Deploy to a production host (e.g. Render, Railway, or PythonAnywhere)
🤝 Credits & Acknowledgments

Special thanks to:

freeCodeCamp — for exceptional open-source learning resources, tutorials, and curriculum guidance that shaped this project's foundations.
Code With Adel — for practical tutorials, step-by-step project walkthroughs, and insightful web development content used as a reference while building this app.
Meta / Coursera — for the original Little Lemon Capstone project specification and design assets that inspired this build.
📄 License

This project is open-source and available under the MIT License.
