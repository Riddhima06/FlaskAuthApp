# FlaskAuthApp
FlaskAuthApp

FlaskAuthApp is a simple authentication web application built using Flask.
It provides user registration with proper backend validation and ensures secure handling of user credentials.

This project was enhanced to fix a registration validation bug and successfully deployed on Render.

🚀 Features

✅ User Registration

✅ Backend (Server-Side) Validation

✅ Unique Email Check

✅ Password Length Validation (Minimum 6 Characters)

✅ Error Message Display on Validation Failure

✅ GitHub Hosted Repository

✅ Live Deployment on Render

🐞 Bug Fixed
❌ Previous Issue

The application allowed users to register even if:

Name was empty

Email was empty

Password was empty

This happened because validation was only handled at the frontend (HTML required attribute), which is not secure.

✅ Solution Implemented

Server-side validation was added inside the /register route in Flask:

Name must not be empty

Email must not be empty

Password must not be empty

Email must be unique

Password must contain at least 6 characters

If validation fails:

The form does not submit

Proper error messages are displayed

🛠 Tech Stack

Backend: Flask (Python)

Frontend: HTML, CSS

Database: SQLite (or your configured DB)

Deployment: Render

Version Control: Git & GitHub

📂 Project Structure
FlaskAuthApp/
│
├── app.py
├── templates/
│   ├── register.html
│   ├── login.html
│
├── static/
│   ├── styles.css
│
├── requirements.txt
├── README.md
└── Procfile (if required for deployment)
⚙️ Installation & Setup (Local Run)
1️⃣ Clone the Repository
git clone https://github.com/your-username/FlaskAuthApp.git
cd FlaskAuthApp
2️⃣ Create Virtual Environment
python -m venv venv

Activate it:

Windows:

venv\Scripts\activate

Mac/Linux:

source venv/bin/activate
3️⃣ Install Dependencies
pip install -r requirements.txt
4️⃣ Run the Application
python app.py

The app will run on:

http://127.0.0.1:5000/
🌍 Live Deployment

The application is deployed on Render.
