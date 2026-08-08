# TikTok Content Publisher

A desktop application for automatically uploading original videos to the owner's TikTok account using the official TikTok Content Posting API.

This project is designed for personal use to streamline the content publishing workflow.

---

## Features

- Upload videos using the official TikTok Content Posting API
- OAuth 2.0 authentication
- Automatic access token refresh
- Draft upload support
- Direct publish support (subject to TikTok approval)
- Upload local MP4 files
- Upload from URL (optional)
- Automatic retry
- Detailed logging

---

## Workflow

```
Video Production
        │
        ▼
Render Final MP4
        │
        ▼
TikTok OAuth Login
        │
        ▼
TikTok Content Posting API
        │
        ▼
Upload Draft / Publish
```

---

## Technology

- Python
- TikTok Content Posting API
- OAuth 2.0
- Requests
- Flask (OAuth callback)

---

## Requirements

- Python 3.11+
- TikTok Developer Account
- TikTok Content Posting API enabled
- Access Token

---

## Installation

```bash
pip install -r requirements.txt
```

---

## Configuration

Create a `.env` file.

```env
CLIENT_KEY=YOUR_CLIENT_KEY
CLIENT_SECRET=YOUR_CLIENT_SECRET
REDIRECT_URI=http://localhost:8080/callback
```

---

## Privacy

No personal information is sold or shared.

OAuth credentials are stored locally on the owner's computer.

---

## Intended Use

This application is intended solely for publishing content owned or authorized by the account owner.

Users are responsible for ensuring uploaded content complies with TikTok's Terms of Service, Community Guidelines, and applicable copyright laws.

---

## License

MIT License