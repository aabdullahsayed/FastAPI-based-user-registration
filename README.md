# User Authentication App



## Features

- User registration with unique username and password
- Secure login and logout
- Password hashing with bcrypt
- Error messages (e.g., "Username already taken")
- Responsive design with Bootstrap 5
- Classic UI design with custom fonts and colors

---

## Tech Stack

**Backend:** FastAPI, SQLAlchemy (SQLite)  
**Frontend:** Jinja2 templates, Bootstrap 5, Google Fonts  
**Security:** Password hashing via passlib (bcrypt)  
**Session Management:** Cookie-based (demo purposes only)

---

## Quickstart

### 1. Clone the repository
```bash
git clone <repository-url>
cd user-auth-app

```

### 2. Create a virtual environment
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
```

### 3.Install dependencies

```bash
pip install fastapi uvicorn sqlalchemy passlib[bcrypt] jinja2
```

### 4. Run the Application

```bash

uvicorn app:app --reload

```

### Project Structure
user-auth-app/
├── app.py             # FastAPI app and routes
├── database.py        # Database setup
├── models.py          # User model
├── templates/         # HTML templates
│   ├── base.html
│   ├── register.html
│   └── login.html
└── users.db           # SQLite database
