# Tumuratas Web Project

This repository contains the web project for *Tumuratas Group, built using the **Django* web framework.

## Table of Contents
- [Project Overview](#project-overview)
- [Technologies Used](#technologies-used)
- [Project Structure](#project-structure)
- [Installation and Setup](#installation-and-setup)
- [Running the Application](#running-the-application)
- [Usage](#usage)
- [Customization](#customization)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

---

## Project Overview
The *Tumuratas Web Project* is a modern web application developed for *Tumuratas Group*, providing a platform for users to explore company services and information interactively.

---

## Technologies Used
- *Django* – High-level Python web framework.
- *Python* – Programming language used for backend development.
- *HTML5 & CSS3* – Structuring and styling the web interface.
- *JavaScript* – Enables interactivity and dynamic content.
- *Database* – Uses SQLite by default but can be switched to PostgreSQL or MySQL.
- *Git & GitHub* – Version control and project hosting.

---

## Project Structure

Tumuratas/
├── manage.py             # Django management script
├── tumuratas/            # Main project directory
│   ├── init.py
│   ├── settings.py       # Project settings
│   ├── urls.py           # URL routing
│   ├── wsgi.py           # WSGI configuration
│   └── asgi.py           # ASGI configuration
├── pages/                # Application for general pages
│   ├── migrations/       # Database migrations
│   ├── init.py
│   ├── admin.py          # Admin definitions
│   ├── apps.py           # App configuration
│   ├── models.py         # Database models
│   ├── tests.py          # Test cases
│   └── views.py          # View functions
├── properties/           # Application for properties (if applicable)
│   ├── migrations/
│   ├── models.py
│   ├── views.py
│   ├── admin.py
│   └── apps.py
├── static/               # Static files (CSS, JS, images)
│   ├── css/
│   ├── js/
│   └── images/
├── templates/            # HTML templates
│   ├── base.html         # Base template
│   ├── index.html        # Homepage
│   └── …
├── .gitignore            # Git ignored files
└── requirements.txt      # List of dependencies

---

## Installation and Setup
To run the project locally, follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/erenaktuerk/Tumuratas.git
cd Tumuratas

2. Create and Activate a Virtual Environment

python -m venv venv

	•	Windows: venv\Scripts\activate
	•	Mac/Linux: source venv/bin/activate

3. Install Dependencies

pip install -r requirements.txt



⸻

Running the Application

1. Apply Database Migrations

python manage.py migrate

2. Create a Superuser (Optional)

python manage.py createsuperuser

Follow the prompts to enter a username, email, and password.

3. Start the Development Server

python manage.py runserver

The application will be accessible at http://127.0.0.1:8000/.

⸻

Usage
	•	Navigation: Users can explore different sections of the website.
	•	Interactivity: JavaScript enables dynamic content and interactions.
	•	Admin Panel: The Django admin interface allows management of content.

⸻

Customization
	•	Design: Modify CSS files in static/css/ to change the website’s appearance.
	•	Content: Update HTML templates in templates/ to modify the website’s content.
	•	Functionality: Extend Django apps inside pages/ and properties/ to add new features.

⸻

Deployment

For production deployment:

1. Configure Production Settings

Modify settings.py to use a production database and secure settings.

2. Collect Static Files

python manage.py collectstatic

3. Set Up a Web Server

Use Gunicorn for WSGI and configure a reverse proxy with Nginx or Apache.

4. Configure the Domain

Ensure the domain points to your server and update Django’s ALLOWED_HOSTS.

⸻

Contributing

Contributions are welcome! To contribute:
	1.	Fork the repository.
	2.	Create a feature branch:

git checkout -b feature/new-feature


	3.	Commit changes:

git commit -m "Description of changes"


	4.	Push the branch:

git push origin feature/new-feature


	5.	Create a Pull Request.

⸻

License

This project is licensed under the MIT License.

⸻

Contact

For questions or support, please contact Tumuratas Group or visit the GitHub repository.