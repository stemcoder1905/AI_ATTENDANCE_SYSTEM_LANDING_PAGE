# SnapClass — Landing Website

Simple Flask-based landing site for the SnapClass AI Attendance project. Provides a static home page and assets used by the main application or project demo.

## Summary

This repository contains a small Flask app that serves the marketing/demo landing page. Static assets (CSS, JavaScript, images) are under the `static/` folder and the HTML is in `templates/index.html`.

## Tech Stack

- Python 3.8+
- Flask
- Gunicorn (recommended for production)

## Project Structure

- `app.py` — Flask entrypoint and route definitions
- `templates/index.html` — landing page markup
- `static/` — CSS, JS, images, fonts
- `requirements.txt` — dependencies

## Installation

1. Create and activate a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate    # macOS / Linux
.venv\Scripts\activate      # Windows
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```

3. Run locally:

```bash
python app.py
```

The app runs by default on port `5002` (see `app.py`).

## Production

Use a WSGI server like `gunicorn`:

```bash
gunicorn app:app -b 0.0.0.0:8000
```

There's a `vercel.json` present for (static) deployments — adapt as needed if you deploy using Vercel or another platform.

## Contributing

Fixes and small content updates are welcome. Please open a PR with clear changes to `templates/index.html` or static assets.

## License

Add a license file if you plan to open source this repository.
# ai-attendance-project-landing