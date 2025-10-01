# 🎓 CampusConnect

CampusConnect is a web-based platform designed to connect students and organizers within a campus.  
Built using **Flask** and **SQLite**, it provides a simple yet powerful way to manage events, registrations, and user interactions.  

---

## ✨ Features
- 🔐 User authentication (students & admins)  
- 🗓️ Event creation and management  
- 📝 Event registration for attendees  
- 📊 Dashboard for organizers to track participants  
- 💬 Community space for students to stay updated  

---

## 💻 Tech Stack
- **Backend:** Flask (Python)  
- **Database:** SQLite  
- **Frontend:** HTML, CSS, Bootstrap  
- **ORM:** SQLAlchemy  
- **Other Tools:** email-validator, Jinja2  

---

## 🏃 How to Run CampusConnect Locally

### 1️⃣ Prerequisites
Make sure you have:  
- Python 3.10+  
- pip (Python package installer)  
- Git (optional, for cloning the repo)  

---

### 2️⃣ Clone the Repository

git clone https://github.com/YOUR-USERNAME/CampusConnect.git
cd CampusConnect

3️⃣ Create a Virtual Environment
# Windows
python -m venv venv
venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate

4️⃣ Install Dependencies
pip install -r requirements.txt


Example requirements.txt:

Flask==2.3.2
Flask-SQLAlchemy==3.0.3
Werkzeug==2.3.8
Jinja2==3.1.2
email-validator==2.1.1

5️⃣ Set Environment Variables
# Windows
set FLASK_APP=app.py
set FLASK_ENV=development

# macOS/Linux
export FLASK_APP=app.py
export FLASK_ENV=development

6️⃣ Initialize the Database
from app import db
db.create_all()

7️⃣ Run the Application
flask run


Open your browser and go to:
http://127.0.0.1:5000

8️⃣ Optional: Admin Setup

To make a user admin:

Open campusconnect.db in DB Browser for SQLite

Navigate to the User table

Set is_admin = 1 for your user

✅ Notes

Always activate your virtual environment before running the app.

Keep requirements.txt updated with any new packages.

For production deployment, consider Gunicorn or Docker.
