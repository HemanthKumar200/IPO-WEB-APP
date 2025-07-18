# Bluestock IPO Web Application

Bluestock is a full-stack IPO Management web application developed as part of an internship project. It allows authorized users to register IPOs, upload related documents, and monitor IPO details on a dashboard.

---

## 🌐 Project Structure

- **Frontend**: React.js  
- **Backend**: Django + Django REST Framework  
- **Database**: SQLite (can be upgraded to PostgreSQL/MySQL)  
- **Authentication**: JWT (via `djangorestframework-simplejwt`)  
- **File Uploads**: RHP, DRHP, Company Logos

---

## 🚀 Features

- Secure login system using JWT
- Register new IPOs with logo and PDF uploads
- View IPOs in a clean tabular dashboard
- Real-time form validations
- RESTful API backend with CORS enabled

---

## 📁 Folder Structure



IPO_Web_App/
├── bluestock-frontend/ # React Frontend

│ ├── public/

│ └── src/

│ ├── components/

│ │ ├── Login.js

│ │ ├── Dashboard.js

│ │ └── IPOForm.js

│ └── App.js

├── ipo_project/ # Django Backend

│ ├── ipo_app/

│ └── ipo_project/

├── db.sqlite3

└── manage.py


## ⚙️ Setup Instructions

### 🔹 Backend (Django)

```bash
cd IPO_Web_App
python -m venv venv
venv\Scripts\activate  # Windows
pip install -r requirements.txt

# Run migrations and start server
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
