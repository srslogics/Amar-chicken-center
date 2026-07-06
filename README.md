# Amar Chicken Center

## Deploy on Render as one service

This project can run as a single Render web service. FastAPI serves both:

- the API from `app/main.py`
- the frontend from `frontend/`

### Render settings

- Environment: `Python`
- Build Command: `pip install -r requirements.txt`
- Start Command: `uvicorn app.main:app --host 0.0.0.0 --port 10000`

### Required environment variable

- `DATABASE_URL`

### Notes

- The frontend now calls the API on the same origin, so no separate frontend service is required.
- Static files such as `css/`, `js/`, and `assets/` are served by FastAPI.
