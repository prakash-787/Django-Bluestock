# 📈 Bluestock IPO Web App

A Django + DRF-based web application to manage IPO listings and company profiles, with PostgreSQL as the backend database.
A full-stack Django + DRF-based web application to manage IPO listings and company data. This system allows users to create and view IPOs, while the admin panel provides control over data management.

---

## 🚀 Features

- ✅ Add and manage companies
- ✅ Create and list IPOs
- ✅ Admin interface for managing users, IPOs, and companies
- ✅ API endpoints using Django REST Framework
- ✅ Bootstrap-powered frontend for quick UI interaction
- Add & view IPO listings
- Create and manage companies
- Admin panel with authentication
- RESTful APIs using Django REST Framework
- PostgreSQL integration
- Bootstrap-based minimal frontend

---

## 🛠️ Tech Stack

- **Backend**: Django, Django REST Framework
- **Database**: PostgreSQL (or SQLite for local testing)
- **Frontend**: HTML + Bootstrap (optional enhancements)
- **Others**: Git, GitHub, Python virtual environment
- **Backend**: Django, Django REST Framework (DRF)
- **Frontend**: Bootstrap, HTML
- **Database**: PostgreSQL (or SQLite for development)
- **Tools**: Git, GitHub, Virtual Environment

---

## 📁 Project Structure

bluestock-ipo-webapp/
├── ipo/ # Django app for IPOs
├── ipoproject/ # Django project configuration
│
├── ipo/ # Django app
├── ipoproject/ # Django project settings
├── env/ # Virtual environment (excluded from Git)
├── manage.py # Django entry point
├── .gitignore
├── requirements.txt # Dependencies (optional)
└── README.md

yaml
@@ -38,81 +41,65 @@ Edit

---

## 🧪 Local Setup
## 💻 How to Run the Project Locally

### 1. Clone the repository

```bash
git clone https://github.com/pranee-v/bluestock-ipo-webapp.git
cd bluestock-ipo-webapp
2. Create and activate virtual environment
2. Create and activate a virtual environment
bash
Copy
Edit
python -m venv env
env\Scripts\activate  # On Windows
env\Scripts\Activate.ps1   # On Windows PowerShell
3. Install dependencies
bash
Copy
Edit
pip install -r requirements.txt  # (or manually install)
pip install django djangorestframework psycopg2-binary
or if you have a requirements.txt:

bash
Copy
Edit
pip install django djangorestframework psycopg2-binary
4. Set up database
pip install -r requirements.txt
4. Apply database migrations
bash
Copy
Edit
python manage.py makemigrations
python manage.py migrate
5. Create superuser (optional, for admin panel)
5. (Optional) Create a superuser
bash
Copy
Edit
python manage.py createsuperuser
6. Run the server
6. Run the development server
bash
Copy
Edit
python manage.py runserver
Visit: http://127.0.0.1:8000
Go to: http://127.0.0.1:8000

🔐 Admin Panel
Visit: http://127.0.0.1:8000/admin
🔌 API Endpoints
Method	Endpoint	Description
GET	/api/ipos/	List all IPOs
POST	/api/ipos/	Create new IPO
GET	/api/company/	List all companies
POST	/api/company/	Add a new company

Login using the superuser credentials you created.
🔐 Admin Access
Visit: http://127.0.0.1:8000/admin

🔌 API Endpoints
Endpoint	Description
/api/ipos/	List & Create IPOs
/api/company/	List & Create Companies
Login using your superuser credentials to manage IPOs, companies, and users.

📦 Deployment (optional)
You can deploy this on platforms like:
🌐 Deployment (optional)
To deploy online, consider using platforms like:

Render

Railway

Vercel (Frontend) + Render (Backend)

📄 License
This project is for educational/demo purposes only.

yaml
Copy
Edit

---

## ✅ How to Use It

1. In VS Code, create a file `README.md` in your root project folder (same level as `manage.py`)
2. Paste the content above into it
3. Save the file and commit it:

```bash
git add README.md
git commit -m "Add README"
git push
Heroku (deprecated free tier, not recommended)
