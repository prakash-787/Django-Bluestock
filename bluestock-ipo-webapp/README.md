# 📈 Bluestock IPO Web App

A full-stack Django + DRF-based web application to manage IPO listings and company data. This system allows users to create and view IPOs, while the admin panel provides control over data management.

---

## 🚀 Features

- Add & view IPO listings
- Create and manage companies
- Admin panel with authentication
- RESTful APIs using Django REST Framework
- PostgreSQL integration
- Bootstrap-based minimal frontend

---

## 🛠️ Tech Stack

- **Backend**: Django, Django REST Framework (DRF)
- **Frontend**: Bootstrap, HTML
- **Database**: PostgreSQL (or SQLite for development)
- **Tools**: Git, GitHub, Virtual Environment

---

## 📁 Project Structure

bluestock-ipo-webapp/
│
├── ipo/ # Django app
├── ipoproject/ # Django project settings
├── env/ # Virtual environment (excluded from Git)
├── manage.py # Django entry point
├── requirements.txt # Dependencies (optional)
└── README.md

yaml
Copy
Edit

---

## 💻 How to Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/pranee-v/bluestock-ipo-webapp.git
cd bluestock-ipo-webapp
2. Create and activate a virtual environment
bash
Copy
Edit
python -m venv env
env\Scripts\Activate.ps1   # On Windows PowerShell
3. Install dependencies
bash
Copy
Edit
pip install django djangorestframework psycopg2-binary
or if you have a requirements.txt:

bash
Copy
Edit
pip install -r requirements.txt
4. Apply database migrations
bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
5. (Optional) Create a superuser
bash
Copy
Edit
python manage.py createsuperuser
6. Run the development server
bash
Copy
Edit
python manage.py runserver
Go to: http://127.0.0.1:8000

🔌 API Endpoints
Method	Endpoint	Description
GET	/api/ipos/	List all IPOs
POST	/api/ipos/	Create new IPO
GET	/api/company/	List all companies
POST	/api/company/	Add a new company

🔐 Admin Access
Visit: http://127.0.0.1:8000/admin

Login using your superuser credentials to manage IPOs, companies, and users.

🌐 Deployment (optional)
To deploy online, consider using platforms like:

Render

Railway

Heroku (deprecated free tier, not recommended)
