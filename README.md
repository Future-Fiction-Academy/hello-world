# Hello World Python App for Railway

A tiny Flask app designed for students to practice **clone → edit → deploy** workflows ("vibe coding") with Railway.

When deployed, visiting the Railway URL shows a styled "Hello, Railway!" page instantly.

## One-click Deploy with Railway

You can add a **Deploy on Railway** button that points to this repo.

> Replace `<YOUR_GITHUB_USERNAME>` and `<YOUR_REPO_NAME>` with your actual GitHub values after you fork/copy this project.

[![Deploy on Railway](https://railway.app/button.svg)](https://railway.app/new/template?template=https://github.com/<YOUR_GITHUB_USERNAME>/<YOUR_REPO_NAME>)

If your repo URL is `https://github.com/acme/hello-world`, your button link should be:

```text
https://railway.app/new/template?template=https://github.com/acme/hello-world
```

## What's in this repo

- `app.py` — simple Flask server with one route (`/`)
- `templates/index.html` — the hello-world page
- `requirements.txt` — Python dependencies
- `Procfile` — production start command
- `railway.json` — Railway deployment config

## Quick Start (Local)

1. Clone the repo:

   ```bash
   git clone <your-repo-url>
   cd hello-world
   ```

2. (Optional but recommended) create a virtual environment:

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Run the app:

   ```bash
   python app.py
   ```

5. Open http://localhost:5000

## Deploy to Railway (manual flow)

1. Push this project to your GitHub repo.
2. In Railway, click **New Project**.
3. Choose **Deploy from GitHub repo**.
4. Select this repository.
5. Railway will detect Python and install `requirements.txt`.
6. Railway starts the app using `railway.json` / `Procfile` with Gunicorn.
7. Open the generated Railway domain from the service dashboard.

You should immediately see the hello-world page.

## Vibe Coding Practice Ideas

- Change the hero text and emoji.
- Add your name and a short bio.
- Add another Flask route (e.g. `/about`).
- Add a simple API endpoint returning JSON.
- Experiment with styling and deploy updates.

---

Have fun shipping small ideas quickly 🚢
