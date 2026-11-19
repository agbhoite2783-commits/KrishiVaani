# 🌾 KrishiVaani — Voice of Agriculture

<div align="center">

### Giving farmers a simpler way to access useful agricultural information.

**KrishiVaani** is a web-based agricultural assistance platform designed to make information and digital support more accessible to farmers through a simple interface and an AI-assisted help experience.

[![Python](https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Flask](https://img.shields.io/badge/Flask-Web%20Framework-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![SQLite](https://img.shields.io/badge/SQLite-Database-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://www.sqlite.org/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-5-7952B3?style=for-the-badge&logo=bootstrap&logoColor=white)](https://getbootstrap.com/)

</div>

---

## 📌 About the Project

Agriculture plays a major role in India's economy and supports millions of livelihoods. However, farmers can face challenges in finding clear, accessible, and useful information when they need it.

**KrishiVaani — Voice of Agriculture** aims to help address this information gap by bringing agricultural support into one easy-to-use web platform.

The project combines a Flask-based web application with an AI-assisted interface. It is being developed as a student project with a focus on applying computer science to a meaningful real-world problem.

## ✨ Key Features

- **AI-assisted agricultural help:** An assistant experience intended to help users find relevant agricultural information.
- **Centralised platform:** A single place to access the support and information offered by the application.
- **Simple web interface:** Designed with usability and accessibility in mind.
- **Database-backed application:** Uses SQLite with SQLAlchemy for application data management.
- **Secure password handling:** Uses Werkzeug password-hashing utilities for password storage.
- **Fallback assistant behaviour:** Includes a rule-based fallback so the assistant experience can still respond when an optional AI service is not configured.
- **Responsive UI:** Uses Bootstrap 5 to support a range of screen sizes.
- **Visual insights:** Chart.js supports data visualisation in the interface.

> **Note:** AI-generated responses are informational and should not replace advice from qualified agricultural experts or official government sources. Users should verify important decisions before acting on them.

## 🧰 Technology Stack

| Layer | Technology |
|---|---|
| Backend | Python, Flask |
| Database | SQLite |
| ORM | SQLAlchemy |
| Authentication utilities | Werkzeug password hashing |
| Frontend | HTML, CSS, Bootstrap 5 |
| Visualisations | Chart.js |
| Optional AI integration | OpenAI API or Gemini API |
| Configuration | Environment variables (.env) |

## 🏗️ Application Overview

At a high level, the application follows this flow:

1. A user opens the KrishiVaani web interface.
2. The Flask application handles the incoming request.
3. Application data is managed through SQLAlchemy and SQLite.
4. When the user interacts with the assistant, the application uses the configured AI integration when available.
5. If an external AI service is not configured, the rule-based fallback provides the available assistant behaviour.
6. The response is returned to the web interface.

## 🚀 Getting Started

Follow these steps to run the project locally once the application source code is added to this repository.

### Prerequisites

- Python 3 installed
- Git installed
- A code editor such as Visual Studio Code

### 1. Clone the repository

~~~bash
git clone https://github.com/agbhoite2783-commits/KrishiVaani.git
cd KrishiVaani
~~~

### 2. Create and activate a virtual environment

**Windows PowerShell:**

~~~powershell
py -m venv venv
.\venv\Scripts\Activate.ps1
~~~

If PowerShell blocks script activation, use Command Prompt instead:

~~~bat
venv\Scripts\activate.bat
~~~

**macOS / Linux:**

~~~bash
python3 -m venv venv
source venv/bin/activate
~~~

### 3. Install dependencies

If a requirements.txt file is present:

~~~bash
python -m pip install -r requirements.txt
~~~

If it is not present yet, add the project's dependency list before running this step.

### 4. Configure environment variables

If you use an optional AI provider, create a local .env file based on the example configuration:

~~~env
# Add only the provider key used by your application.
OPENAI_API_KEY=
GEMINI_API_KEY=
~~~

Keep API keys private. **Never commit your real .env file or secret keys to GitHub.** The application should continue to use its rule-based fallback when an AI key is not configured.

### 5. Run the application

Run the Flask entry-point used by your project. For example, if your main file is app.py:

~~~bash
python app.py
~~~

Then open the local address printed in your terminal (commonly http://127.0.0.1:5000).

> The exact entry-point and commands may need adjustment to match the source files once they are uploaded.

## 📁 Suggested Project Structure

The layout below is a suggested structure for organising the application. Update it to match the actual files in this repository.

~~~text
KrishiVaani/
├── app.py                 # Flask application entry point
├── models.py              # Database models (if separated)
├── requirements.txt       # Python dependencies
├── .env.example           # Example environment variables
├── .gitignore             # Files excluded from version control
├── templates/             # HTML templates
├── static/
│   ├── css/               # Stylesheets
│   ├── js/                # Frontend JavaScript
│   └── images/            # Project images and assets
└── README.md
~~~

## 🔐 Security & Responsible Use

- Passwords should be stored as secure hashes, never as plain text.
- Keep API keys and other credentials in environment variables.
- Do not upload .env, database files containing personal data, or other secrets.
- Validate and handle user input on the server.
- Treat AI output as informational; verify critical agricultural guidance with reliable sources.

## 🖼️ Screenshots

Screenshots of the application will be added here as the interface and features are documented.

<!-- Add screenshots by committing image files and linking them here. -->

## 🛣️ Future Improvements

Potential areas for further development include:

- More agricultural topics and structured knowledge resources.
- Improved multilingual and voice-based interaction.
- Better access to verified agricultural schemes and resources.
- Expanded testing, accessibility, and mobile usability.
- More detailed dashboards and useful visualisations.

## 👥 Team & Contributions

This project is being developed as a student project. Contributions, suggestions, and constructive feedback are welcome.

If you would like to contribute:

1. Fork the repository.
2. Create a feature branch.
3. Make your changes and test them.
4. Open a pull request with a clear description.

## 📄 License

A license has not been selected for this repository yet. Until one is added, all rights are reserved by the project owner.

---

<div align="center">

**KrishiVaani — Voice of Agriculture** 🌱

*Technology with a purpose: making useful agricultural support more accessible.*

Built with 💚 by [Anushka Bhoite](https://github.com/agbhoite2783-commits)

</div>
