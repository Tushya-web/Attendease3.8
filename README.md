
<center><img width="290" height="80" alt="AttendEase" src="https://github.com/user-attachments/assets/18f6c229-4bda-4c21-b791-4ee18e2ccdc3" /></center>

> AttendEase is an AI-powered face recognition attendance system built with Django, DeepFace (FaceNet), OpenCV, and Jazzmin.  
> It ensures secure, real-time attendance logging using deep learning–based face verification and anti-spoofing.
> (Django + DeepFace/FaceNet + Jazzmin + HTML/CSS/JS)

### AttendEase is a full-stack, intelligent attendance automation system powered by Django, DeepFace/FaceNet, OpenCV, and a clean Jazzmin-powered admin dashboard.
It features secure face verification, user registration, attendance tracking, leave management, and admin control.

## Table of Contents
- [Technology Documentation](#-technology-documentation-which-used)
- [Project Information](#project-information)
- [AI + Face Verification](#ai--face-verification)
- [User Portal](#user-portal)
- [Admin Panel](#admin-panel-jazzmin-dashboard)
- [Demo](#demo)
- [Installation](#installation--setup-step-by-step)
- [Project Structure](#project-structure)
- [Author](#author)

## Technology Documentation

**Frontend**
<p align="left"> <!-- HTML --> <a href="https://developer.mozilla.org/en-US/docs/Web/HTML" target="_blank"> <img src="https://img.shields.io/badge/HTML5-Frontend-E34F26?style=for-the-badge&logo=html5&logoColor=white"/> </a> <!-- CSS --> <a href="https://developer.mozilla.org/en-US/docs/Web/CSS" target="_blank"> <img src="https://img.shields.io/badge/CSS3-Styling-1572B6?style=for-the-badge&logo=css3&logoColor=white"/> </a> <!-- JavaScript --> <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://img.shields.io/badge/JavaScript-ES6-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/> </a> </p>

**Backend**
<p align="left"> <!-- Python --> <a href="https://www.python.org/" target="_blank"> <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white"/> </a> </p>

**Frameworks & Libraries**
<p align="left"> <!-- Django --> <a href="https://www.djangoproject.com/" target="_blank"> <img src="https://img.shields.io/badge/Django-4.x-0C4B33?style=for-the-badge&logo=django&logoColor=white"/> </a> <!-- Jazzmin --> <a href="https://django-jazzmin.readthedocs.io/" target="_blank"> <img src="https://img.shields.io/badge/Jazzmin-Admin%20Theme-8A2BE2?style=for-the-badge&logo=django&logoColor=white"/> </a> </p>

**AI & Computer Vision**
<p align="left"> <!-- Conversational AI --> <img src="https://img.shields.io/badge/Conversational-AI%20Chatbot-blueviolet?style=for-the-badge&logo=chatbot&logoColor=white"/> <!-- AI Powered --> <img src="https://img.shields.io/badge/AI-Powered-orange?style=for-the-badge&logo=artificial-intelligence&logoColor=white"/> <!-- DeepFace --> <a href="https://serengil.github.io/deepface/" target="_blank"> <img src="https://img.shields.io/badge/DeepFace-FaceNet-F9A825?style=for-the-badge&logo=google&logoColor=white"/> </a> <!-- FaceNet --> <a href="https://arxiv.org/abs/1503.03832" target="_blank"> 
  <!-- OpenCV -->  <img src="https://img.shields.io/badge/OpenCV-Computer%20Vision-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white"/>
  <img src="https://img.shields.io/badge/FaceNet-Embedding%20Model-1976D2?style=for-the-badge&logo=google&logoColor=white"/> </a> </p>

## Screenshots

### Index Page
<p align="center">
  <img src="https://github.com/user-attachments/assets/de6da535-f86a-4315-a29c-66527c078409" alt="Index Page" width="800"/>
</p>

---

### Admin Dashboard 
<p align="center">
  <img src="https://github.com/user-attachments/assets/fd5eb022-6f4d-4dc2-a0c2-7ad3905fb48d" alt="Admin Dashboard" width="800"/>
</p>

---

### User Dashboard
<p align="center">
  <img src="https://github.com/user-attachments/assets/a01975f3-d9c7-4a8c-ad60-820e106b4042" alt="User Dashboard" width="800"/>
</p>



## Demo
https://github.com/user-attachments/assets/03b4130c-6bcc-4957-811b-0bff7711e6cb 

## Features
- Django-based full-stack architecture
- Gemini AI Chatbot for Information & Assistance 
- DeepFace FaceNet-based face matching  
- Secure master-face verification  
- Real-time webcam-based recognition  
- IN/OUT time-based attendance  
- User + Admin dashboards  
- Leave management system  
- Attendance export (CSV/PDF)  

## Project Information

- Django-based Web Application
- Face Recognition using DeepFace (FaceNet backend)
- Real-Time Attendance Marking with Liveness Detection
- Admin Dashboard Powered by Jazzmin
- Student/Employee Management
- Daily Attendance, Time-based Attendance (IN/OUT)
- Export Attendance as CSV/Excel
- Responsive UI (HTML, CSS, JS)

## Gemini AI Integration
- AttendEase uses a Gemini-powered chatbot as an intelligent assistant to provide
system-related information, attendance rules, and user guidance through
conversational AI, improving usability and system understanding.

## AI + Face Verification
- DeepFace with FaceNet model
- Real-time webcam recognition
- Liveness detection (anti-spoofing)
- Face must match the master/default face uploaded by admin

## User Portal
- Register & Login
- Add face (must match master data)
- Mark attendance
- View attendance
- View uploaded faces
- Apply for leave
- Update personal information
- Download attendance (PDF/CSV)

## Admin Panel (Jazzmin Dashboard)
- Upload master data (student/faculty records)
- Approve or reject user registration
- Manage users, faculty, students
- Approve/reject leave requests
- Manage face entries
- View attendance analytics
- Export attendance reports

### Installation & Setup (Step-by-Step)

**1️. Clone the Repository**
```
git clone https://github.com/Tushya-web/Attendease.git

```

**2️. Create Virtual Environment**
```
python -m venv env

source env/bin/activate   # Linux/Mac

env\Scripts\activate      # Windows
```

**3️. Install Dependencies**
```
pip install -r requirements.txt
```

**4️. Apply Migrations**
```
python manage.py makemigrations

python manage.py migrate
```

**5️. Create Superuser (Admin Login)**
```
python manage.py createsuperuser
```

**6️. Run Development Server**
```
python manage.py runserver
```

## Project Structure
```
AttendEase/
│
├── attendease/                 # Django project configuration
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py
│
├── accounts_app/             # Core attendance application
│   ├── models.py               # Database models
│   ├── views.py                # Request handling logic
│   ├── facesystem.py/          # Face detection & recognition modules
│   ├── forms.py/               # For custom forms
│   ├── templates/              # HTML templates
│   ├── static/                 # CSS, JavaScript, assets
│   ├── utils/                  # Helper functions
│   └── urls.py
│
├── static/                     # Css & js for Admin Dashboard
├── staticfiles/
├── media/                      # Face image storage
│   ├── master_faces/           # Registered faces
│   ├── Master_data_csv/        # csv file store here
│   ├── deepface_model/         # Deepface Facenet Model stores here
│   └── user_faces/             # Captured attendance images
│
├── requirements.txt            # Python dependencies
└── README.md                   # Project documentation
```

### Author

Tushya R. Parmar

AI and Computer Vision Enthusiast

> Disclaimer: This project is created for educational and academic purposes only. It is not affiliated with or based on any existing product, company, or trademark.


![GitHub Repo stars](https://img.shields.io/github/stars/Tushya-web/Attendease_3.9?style=flat)
![GitHub forks](https://img.shields.io/github/forks/Tushya-web/Attendease_3.9?style=flat)
![GitHub issues](https://img.shields.io/github/issues/Tushya-web/Attendease_3.9?style=flat)
