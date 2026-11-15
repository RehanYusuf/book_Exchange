# 📚 Book_Exchange API

A RESTful API built with **FastAPI** for managing book exchanges and user interactions.

## ✨ Features

- **User Management**: Endpoints for user registration, profiles, and interactions (`/users`).
- **Book Management**: Endpoints for listing, browsing, and managing book exchanges (`/books`).
- **Automated Database Setup**: Automatically initializes database tables upon application startup.
- **Interactive API Docs**: Built-in Swagger UI and ReDoc documentation powered by FastAPI.

## 🛠️ Tech Stack

- **Framework**: [FastAPI](https://fastapi.tiangolo.com/)
- **Language**: Python 3.8+
- **ASGI Server**: Uvicorn
- **Database**: SQL-based (configured via `database.py`)

## 📁 Project Structure

```text
├── main.py          # Application entry point and router configuration
├── database.py      # Database connection and table initialization
├── routes/
│   ├── books.py     # Book exchange endpoints
│   └── users.py     # User management endpoints
└── README.md        # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.8+ installed on your machine.

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/kitab-exchange-api.git
   cd kitab-exchange-api
   ```

2. **Create and activate a virtual environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```

3. **Install dependencies:**
   ```bash
   pip install fastapi uvicorn sqlalchemy
   ```
   *(Note: If you have a `requirements.txt` file, run `pip install -r requirements.txt` instead.)*

### Running the Application

Start the development server using Uvicorn:

```bash
uvicorn main:app --reload
```

The API will be available at `http://127.0.0.1:8000`.

## 📖 API Documentation

Once the server is running, you can explore and test the endpoints interactively:

- **Swagger UI**: [http://127.0.0.1:8000/docs](http://127.0.0.1:8000/docs)
- **ReDoc**: [http://127.0.0.1:8000/redoc](http://127.0.0.1:8000/redoc)

### Base Endpoint

- `GET /` — Health check / welcome message:
  ```json
  {
    "message": "Welcome to the Kitab Exchange API!"
  }
  ```

## 🤝 Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request for any improvements or bug fixes.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request
