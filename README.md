# M-Tracker 2.0

A personal money-tracking app built as a hands-on learning project during a Flutter course.

## What it does

- **Track expenses and income** — add transactions with amounts, categories, and dates
- **Categorize spending** — organize transactions by category
- **Monthly summaries** — visualize spending with charts
- **Secure login** — JWT-based user authentication
- **Export data** — export transactions to CSV

## Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | Flutter (Dart) |
| Backend | Python / Flask |
| Database | SQLite (dev) → PostgreSQL (prod) |
| Auth | JWT (Flask-JWT-Extended) |

## Project Structure

```
M-tracker-2.0/
├── budget_app_frontend/   # Flutter app
└── budget_app_backend/    # Flask REST API
```

## Running the project

### Backend
```bash
cd budget_app_backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
python app.py
```
Backend runs at `http://127.0.0.1:5000`.

### Frontend
```bash
cd budget_app_frontend
flutter pub get
flutter run -d chrome          # web
flutter run -d emulator-5554   # Android emulator
```

## Notes

This was built purely as a learning exercise — it is not production-ready.
