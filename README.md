<div align="center">

# 🔍 OSINet Portal

**An Open Source Intelligence (OSINT) Investigation Tool**

![Python](https://img.shields.io/badge/Python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)
![SQLite](https://img.shields.io/badge/SQLite-07405E?style=for-the-badge&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

*Investigate email breaches, phone numbers, and digital footprints — all in one place.*

</div>

---

## 📌 About The Project

**OSINet Portal** is a full-stack OSINT (Open Source Intelligence) web application built entirely from scratch — frontend and backend. It allows users to investigate digital identities by checking email breach databases, looking up phone number information, and maintaining a searchable investigation history.

This project was built as a practical tool to learn real-world full-stack development, REST API integration, containerization, and deployment.

---

## ✨ Features

- 🔐 **Email Breach Checker** — Integrated with the [Have I Been Pwned (HIBP) API](https://haveibeenpwned.com/API/v3) to check if an email has been exposed in data breaches
- 📞 **Phone Number Investigator** — Uses APILayer to look up carrier, location, and line type for any phone number
- 🗄️ **Investigation History** — All searches are persisted in a local SQLite database for later review
- 🐳 **Dockerized** — Fully containerized with Docker & Docker Compose for consistent deployment
- ☁️ **Cloud Deployable** — Supports one-click deployment on Railway with included `Procfile` and `runtime.txt`

---

## 🛠️ Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Flask |
| Frontend | HTML5, CSS3, JavaScript (Jinja2 templates) |
| Database | SQLite |
| APIs | HIBP API, APILayer Phone API |
| DevOps | Docker, Docker Compose |
| Deployment | Railway, Heroku-compatible |

---

## 📁 Project Structure

```
osinet-portal/
│
├── app.py                  # Main Flask application & all routes
├── history.db              # SQLite database for investigation history
├── requirements.txt        # Python dependencies
├── runtime.txt             # Python runtime version
├── Procfile                # For Railway/Heroku deployment
├── Dockerfile              # Docker image configuration
├── docker-compose.yml      # Multi-container Docker setup
│
├── templates/              # Jinja2 HTML templates (frontend views)
│   └── *.html
│
├── static/                 # CSS, JavaScript, and assets
│   ├── css/
│   └── js/
│
├── DEPLOYMENT_GUIDE.md     # Full deployment documentation
├── EASY_DEPLOYMENT.md      # Quick-start deployment guide
├── RAILWAY_DEPLOYMENT.md   # Railway-specific deployment steps
└── HIBP_API_SETUP.md       # HIBP API key setup instructions
```

---

## 🚀 Getting Started

### Prerequisites

- Python 3.9+
- pip
- Docker (optional, for containerized setup)

### 1. Clone the Repository

```bash
git clone https://github.com/nani-coder-ship-it/osinet-portal.git
cd osinet-portal
```

### 2. Create a Virtual Environment

```bash
python -m venv venv
source venv/bin/activate      # On Windows: venv\Scripts\activate
```

### 3. Install Dependencies

```bash
pip install -r requirements.txt
```

### 4. Set Up Environment Variables

Create a `.env` file in the root directory:

```env
HIBP_API_KEY=your_hibp_api_key_here
APILAYER_API_KEY=your_apilayer_key_here
SECRET_KEY=your_flask_secret_key
```

> 📖 See [HIBP_API_SETUP.md](./HIBP_API_SETUP.md) for how to get your API keys.

### 5. Run the App

```bash
python app.py
```

Visit `http://localhost:5000` in your browser.

---

## 🐳 Run with Docker

```bash
# Build and start the container
docker-compose up --build

# Stop the container
docker-compose down
```

---

## ☁️ Deploy to Railway

See [RAILWAY_DEPLOYMENT.md](./RAILWAY_DEPLOYMENT.md) for step-by-step instructions.

Quick steps:
1. Push your repo to GitHub
2. Connect it to [Railway](https://railway.app)
3. Add your environment variables in the Railway dashboard
4. Deploy 🚀

---

## 📸 Screenshots

> *(Add screenshots of the app here)*

---

## 🔮 Future Improvements

- [ ] Add user authentication & login system
- [ ] IP address lookup & geolocation
- [ ] Username search across social platforms
- [ ] Export investigation reports as PDF
- [ ] Dark mode UI

---

## 🙋‍♂️ Author

**Vaigandla Venkata Naga Vignesh**

[![GitHub](https://img.shields.io/badge/GitHub-nani--coder--ship--it-181717?style=flat&logo=github)](https://github.com/nani-coder-ship-it)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/vaigandla-venkata-naga-vignesh-231b65351)
[![Email](https://img.shields.io/badge/Email-vigneshvaigandla@gmail.com-D14836?style=flat&logo=gmail)](mailto:vigneshvaigandla@gmail.com)

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

<div align="center">

⭐ If you found this project useful, please consider giving it a star!

</div>
