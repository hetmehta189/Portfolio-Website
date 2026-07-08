# 🌐 Interactive Developer Portfolio

A modern, responsive, and visually stunning developer portfolio website built using **Flask**, **Tailwind CSS**, **Google Fonts**, and **Font Awesome**. The site features a futuristic dark theme with glowing neon backdrop blur effects, interactive 3D layout cards with translation depth, and is production-ready for instant cloud hosting.

---

## 🚀 Features

* **Futuristic Dark Theme**: Sleek background gradients with dynamic glowing background blobs (blur filters) that add a depth effect.
* **Interactive 3D Cards**: Utilizes custom CSS 3D viewport matrix perspectives (`perspective`, `preserve-3d`, `translateZ`) to pop text elements and create subtle rotation effects when hovering.
* **Multi-Page Architecture**: Structured clean navigation routing via Flask for Home, About, Skills, Projects, and Contact sections.
* **Responsive Design**: Designed mobile-first using Tailwind CSS, ensuring accessibility on screens of all sizes.
* **Production-Ready**: Preconfigured with `Procfile` and `requirements.txt` for instant deployment on cloud servers like Render or Heroku.

---

## 🛠️ Tech Stack & Badges

[![Python Version](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)](https://www.python.org/)
[![Flask Version](https://img.shields.io/badge/Flask-3.0%2B-lightgrey?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-v3-38B2AC?logo=tailwind-css&logoColor=white)](https://tailwindcss.com/)
[![Deploy to Render](https://img.shields.io/badge/Deploy%20to-Render-46E3B7?logo=render&logoColor=white)](https://render.com/)

---

## 📂 Project Structure

```text
├── static/
│   └── app.css           # Custom 3D perspective transition utility styles
├── templates/            # Jinja2 HTML Templates
│   ├── base.html         # Global layout (glowing blobs, navigation bar, footer)
│   ├── index.html        # Home intro page featuring 3D developer card
│   ├── about.html        # Detailed about bio section
│   ├── skills.html       # Tech skill lists with percentage badges
│   ├── projects.html     # Projects showcase cards with hover actions
│   └── contact.html      # Personal contact form and detail links
├── app.py                # Core Flask application and routing definitions
├── Procfile              # Gunicorn configuration script for production hosting
├── requirements.txt      # List of project Python requirements
└── .gitignore            # Files excluded from git tracking
```

---

## ⚙️ Local Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/hetmehta189/Portfolio-Website.git
cd Portfolio-Website
```

### 2. Create and Activate a Virtual Environment
**On Windows:**
```bash
python -m venv venv
venv\Scripts\activate
```
**On macOS/Linux:**
```bash
python3 -m venv venv
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Run the Application
Start the development server:
```bash
python app.py
```
Open **`http://127.0.0.1:5000`** in your browser to view the portfolio.

---

## ☁️ Deployment on Render

This application is ready to be hosted as a Web Service on [Render](https://render.com/).

### Steps to Deploy:
1. Push your code changes to GitHub.
2. Sign in to **Render** and click **New > Web Service**.
3. Link your GitHub repository.
4. Set the following settings:
   - **Environment**: `Python`
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `gunicorn app:app`
5. Click **Deploy Web Service**.
