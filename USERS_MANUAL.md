# DesignXpress AI Studio Pro — User Manual

## 1) Create Account / Login
- Go to **/auth** and choose **Register**.
- Login to access the **Dashboard**.

## 2) Create a Series
From Dashboard:
- Click **Create New Series**
- Fill required fields:
  - Series Name
  - Niche
  - Art Style
  - Voice Type
  - Posting Schedule
  - Platforms
- Click **Create Series**

## 3) Generate Videos
- Open a series
- Click **Generate Video**
- Enter/paste a script or prompt
- Click **Generate**
- Watch progress in real‑time (WebSocket). When complete, a video URL appears.

## 4) Connect Social Media Accounts (OAuth)
- Go to **Settings**
- Click **Connect Social Media**
- Choose a provider (YouTube/Google, TikTok, etc.)
- Approve access in the popup window
- The account appears in your connected list

## 5) Security
- Your login uses JWT stored locally.
- For production, enable HTTPS and consider encrypting stored OAuth tokens at rest.
