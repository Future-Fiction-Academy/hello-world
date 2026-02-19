# Hello World Python App for Railway

A tiny Flask app designed for students to practice **clone → edit → deploy** workflows ("vibe coding") with Railway.

When deployed, visiting the Railway URL shows a styled "Hello, Railway!" page instantly.

## One-click Deploy with Railway

Railway's old direct GitHub template URL format is deprecated, so this repo now documents the **official template flow**.

### Use this repo as a template example

1. Go to Railway and sign in.
2. Click **New Project** → **Deploy from GitHub repo**.
3. Select `Future-Fiction-Academy/hello-world` (or your own repo).
4. Deploy once so Railway creates the project.
5. Open project **Settings**.
6. Click **Generate Template from Project** (or **Create Template**).
7. Copy your new template URL. It will look like:

   - `https://railway.app/new/template/<YOUR_TEMPLATE_ID>`
   - or `https://railway.com/template/<YOUR_TEMPLATE_ID>`

8. Replace the deploy button link with your template URL:

```md
[![Deploy on Railway](https://railway.com/button.svg)](https://railway.app/new/template/YOUR-TEMPLATE-ID-HERE)
```

Optional: append `?utm_source=github&utm_medium=button` for analytics.

### Current button placeholder

Update this link after you create your template ID:

[![Deploy on Railway](https://railway.com/button.svg)](https://railway.app/new/template/YOUR-TEMPLATE-ID-HERE)

If you want to publish it publicly later, use Railway Templates and click **Publish** so others can discover it from the Railway marketplace.

If you want to create your own Deploy on Railway button for another project, use this format and replace the placeholder:

```text
https://railway.app/new/template/<YOUR_TEMPLATE_ID>
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
