# 🔐 login-system

This project is a simple login system developed to practice and demonstrate backend and frontend integration using Flask. It's perfect for learning how to build a full-stack web application with user authentication, password security, and session control.

---

## 🚀 Features

This login system includes essential user authentication functionality with session management and secure password handling.

### 📝 User Registration
- Form with:
  - Name
  - Email
  - Password
- Required field validation (client-side and server-side)
- Password is stored securely using hash (via Werkzeug)

### 🔓 User Login
- Verifies user credentials (email + hashed password)
- Creates a session after successful login
- Redirects user to the dashboard

### 📋 Dashboard
- Accessible only by authenticated users
- Displays a welcome message:  
  _"Welcome, [username]!"_
- Redirects unauthenticated users to the login page

### 🔚 Logout
- Destroys the session
- Redirects back to the login page

---

## 🧱 Tech Stack

- **Backend:** Python, Flask, SQLite, Werkzeug
- **Frontend:** HTML, CSS, JavaScript
- **Other Tools:** Git, GitHub

---

## 📂 Project Structure

```
login-system/
│
├── backend/
│   ├── app.py                # Main Flask app
│   ├── database.db           # SQLite database
│   └── models.py             # Database interaction
│
├── frontend/
│   ├── templates/            # HTML (Jinja2)
│   │   ├── login.html
│   │   ├── register.html
│   │   └── dashboard.html
│   └── static/               # CSS and JS
│       ├── style.css
│       └── script.js
│
├── .gitignore
└── README.md
```

---

## ⚙️ How to Run

```bash
# Clone the repository
git clone https://github.com/your-username/login-system.git
cd login-system

# (Optional but recommended) Create virtual environment
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate

# Install required packages
pip install flask werkzeug
```

```bash
# Run the app
cd backend
python app.py
```

Open your browser and visit: [http://localhost:5000](http://localhost:5000)

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change or improve.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

Made with ❤️ by [@hadrielyharrizon](https://github.com/hadrielyharrizon) and [@A1cantar4](https://github.com/A1cantar4)