# 📰 NewsNepal — Nepali News Aggregator

NewsNepal is a **full-stack news aggregation platform** built with **Django** (backend) and **React** (frontend).

It collects and summarizes news articles from major Nepali news portals in **real-time**, supporting both **English and Nepali** languages.

---

## 🚀 Project Overview

**Frontend Repository:** [NewsNepal-Frontend](https://github.com/arjun28-ach/NewsNepal-Frontend)
**Backend Repository:** [NewsNepal-Backend](https://github.com/arjun28-ach/NewsNepal-Backend)

The application fetches and summarizes news from trusted Nepali sources, offering a clean, responsive, and bilingual user experience.

---

## 🌟 Features

### 📰 News & Categories

* **Real-time aggregation** from multiple news portals
* Filter by categories:
    * **Politics**, **Business**, **Technology**, **Sports**, **Entertainment**
    * **Education**, **Health**, **World**, **Lifestyle**

### 🌐 Bilingual Support

* Toggle between **English (EN)** and **Nepali (NP)**
* Interface and content adapt to the selected language

### 💡 User Experience

* **Dark/Light Mode**
* **Bookmark** favorite articles
* **Search** across all news
* Category-based filtering
* Load more articles dynamically
* **Responsive** for desktop and mobile

### ⚙️ Backend Highlights

* **Django 5.0.2**
* **BeautifulSoup4** and **Newspaper3k** for web scraping
* Real-time content update using cron jobs or Celery (optional)
* SQLite database (default) — easily switchable to **PostgreSQL**

### 🎨 Frontend Highlights

* **React** + Bootstrap + jQuery
* Modern responsive UI
* Dynamic content rendering
* **REST API** integration with Django backend

---

## 🧩 Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | React, HTML5, CSS3, JavaScript (ES6+), Bootstrap, Font Awesome, Google Fonts (Poppins) |
| **Backend** | Django 5.0.2, Python 3.x, BeautifulSoup4, Newspaper3k, Requests, PyTZ |
| **Database** | SQLite (default) |
| **APIs** | RESTful APIs via Django REST Framework (if applicable) |

---

## 🛠️ Setup Instructions

### 📦 1. Clone Both Repositories

```bash
# Backend
git clone [https://github.com/arjun28-ach/NewsNepal-Backend.git](https://github.com/arjun28-ach/NewsNepal-Backend.git)
cd NewsNepal-Backend

# Frontend
git clone [https://github.com/arjun28-ach/NewsNepal-Frontend.git](https://github.com/arjun28-ach/NewsNepal-Frontend.git)
cd NewsNepal-Frontend
```

### ⚙️ 2. Backend Setup (Django)

``` Bash
cd NewsNepal-Backend
python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
The backend will start at:

🔗 http://127.0.0.1:8000
```

### 💻 3. Frontend Setup (React)
```Bash

cd NewsNepal-Frontend
npm install
npm start
The frontend will start at:

🔗 http://localhost:3000
```
### 🔗 4. Connect Frontend & Backend
The React app fetches data from the Django API (default: http://127.0.0.1:8000/api/). Ensure both servers are running simultaneously.

You can configure API URLs in the frontend’s .env file:
```

REACT_APP_API_BASE_URL=[http://127.0.0.1:8000/api/](http://127.0.0.1:8000/api/)
```

### 📁 Project Structure
```
NewsNepal/
├── NewsNepal-Backend/
│   ├── news/
│   ├── newsnepal/
│   ├── requirements.txt
│   └── manage.py
│
└── NewsNepal-Frontend/
    ├── src/
    ├── public/
    ├── package.json
    └── .env
```
### 📚 Usage
```
Language Switch: Toggle EN/NP for bilingual view

Dark Mode: Click moon/sun icon to switch themes

Bookmarks: Save & manage favorite articles

Search: Find specific articles easily

Categories: Browse news by topics
```
### 🧠 Future Enhancements
```
Personalized recommendations using NLP

Telegram/Email news summaries

User authentication and profiles

Ad & premium subscription model
```

### 🤝 Contributing
Fork the repository

Create your feature branch:

Bash
```
git checkout -b feature/YourFeature
Commit your changes:
```
Bash
```
git commit -m "Add YourFeature"
Push to your branch:
```
Bash
```
git push origin feature/YourFeature
Open a Pull Request
```

### 📜 License
```
This project is licensed under the MIT License — see the LICENSE file for details.
```

### 👨‍💻 Author
```
Arjun Acharya
```


### 🌍 GitHub: @arjun28-ach ✉️ Email: acharayaarjun@gmail.com

### 🙏 Acknowledgments
```
News content sourced from various Nepali news portals

Thanks to all news providers and open-source contributors

Built with ❤️ using Django & React

