# Client Finance ACC Theme

This is a safe workspace copy of `client-finance` with the `Amar-chicken-center`
visual theme layered on top.

## What changed

- `client-finance` app logic and files remain the functional base.
- The frontend styling is switched to the `Amar-chicken-center` look.
- FastAPI serves both the API and frontend from one service.

## Render deploy

Use a single Render web service with:

- Environment: `Python`
- Build Command: `pip install -r requirements.txt`
- Start Command: `uvicorn app.main:app --host 0.0.0.0 --port 10000`

### Required environment variable

- `DATABASE_URL`

## Notes

- The frontend now uses same-origin API calls.
- Static paths like `css/`, `js/`, `assets/`, `manifest.webmanifest`, and `sw.js`
  are served by FastAPI.
