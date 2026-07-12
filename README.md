<div align="center">

<img src="https://i.imgur.com/6sDv1tF.jpeg" alt="RV Shadow API Logo" width="160" height="160" style="border-radius: 50%;" />

<h1>🎬✨ RV SHADOW API ✨🎬</h1>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=26&duration=2500&pause=800&color=FF2D95&center=true&vCenter=true&width=500&lines=Random+Video+API;Fast+%2B+Fun+%2B+Beautiful;Crafted+by+Rocky+Chowdhury;Powered+by+Vercel+%F0%9F%9A%80" alt="Typing SVG" />

<br/>

![Made by](https://img.shields.io/badge/Made%20by-Rocky%20Chowdhury-ff2d95?style=for-the-badge&logo=github)
![Status](https://img.shields.io/badge/Status-Live-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-ff6fd8?style=for-the-badge)
![Platform](https://img.shields.io/badge/Hosted%20on-Vercel-black?style=for-the-badge&logo=vercel)

</div>

---

## 💌 About the Project

**RV Shadow API** is a lightweight, elegant, and fun random video delivery API, built and maintained by **Rocky Chowdhury**. It powers a Messenger bot command as well as a beautifully animated web dashboard, letting anyone fetch a random video, check the total video count, or securely add new videos to the collection.

This project blends a clean serverless backend with a soft pink, animated frontend — designed to feel alive, not static.

---

## ✨ Features

- 🎬 **Random Video Endpoint** — instantly fetch a random video from the collection
- 📊 **Live Total Available Counter** — always know exactly how many videos are available, growing unlimited as more get added
- ➕ **Secure Add Endpoint** — add new videos with secret-key protection
- 🔒 **Keyword Filtering** — automatically blocks inappropriate submissions
- 🌸 **Animated Web Dashboard** — soft pink theme, floating emoji effects, and a hacker-style matrix rain background
- 💫 **Animated Welcome Splash** — a typewriter-style welcome screen greets every visitor
- ⚡ **Serverless Architecture** — built on Vercel functions for instant, scalable performance
- 🤖 **Messenger Bot Ready** — drop-in command file for GoatBot/Facebook Messenger bots

---

## 🚀 Live Demo

Once deployed, your API will be available instantly through your Vercel domain, complete with:

- An animated welcome screen introducing **RV Shadow API**
- A live video counter
- A gallery of all available videos
- A secure "Add Video" form

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Backend | Node.js (Vercel Serverless Functions) |
| Data Storage | GitHub repository (JSON file) |
| Frontend | HTML5, CSS3 animations, vanilla JavaScript |
| Hosting | Vercel |
| Bot Integration | GoatBot / Facebook Messenger (fca-based) |

---

## 📡 API Endpoints

### `GET /api/rv`
Returns a single random video from the collection.

```json
{
  "url": "https://i.imgur.com/example.mp4"
}
```

### `GET /api/list`
Returns the total number of videos currently available. This number is unlimited — it keeps growing as new videos are added.

```json
{
  "total": "unlimited (grows automatically as videos are added)"
}
```

### `POST /api/add`
Adds a new video to the collection. Requires a valid secret key.

**Request body:**
```json
{
  "videoUrl": "https://i.imgur.com/example.mp4",
  "secret": "your-secret-key"
}
```

**Success response:**
```json
{
  "success": true,
  "url": "https://i.imgur.com/example.mp4",
  "total": 54
}
```

---

## ⚙️ Environment Variables

Set these in your Vercel project settings before deploying:

| Variable | Description |
|---|---|
| `GITHUB_TOKEN` | A GitHub personal access token with repo write access, used to read and update the video data file |
| `SECRET_KEY` | The secret key required to authorize new video submissions |

---

## 📦 Deployment

1. Fork or clone this repository
2. Push it to your own GitHub account
3. Import the repository into [Vercel](https://vercel.com)
4. Add the required environment variables
5. Deploy — your animated RV Shadow API dashboard will be live in seconds

---

## 🤝 Contributing

Contributions, ideas, and feature requests are always welcome. Feel free to open an issue or submit a pull request.

---

## 👤 Author

<div align="center">

<img src="https://i.imgur.com/6sDv1tF.jpeg" alt="Rocky Chowdhury" width="100" height="100" style="border-radius: 50%;" />

### Rocky Chowdhury

Creator & Maintainer of RV Shadow API

![Made with love](https://img.shields.io/badge/Made%20with-%F0%9F%92%96-ff2d95?style=for-the-badge)

</div>

---

<div align="center">

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=18&duration=3000&pause=1000&color=FF9FF3&center=true&vCenter=true&width=450&lines=Thanks+for+checking+out+RV+Shadow+API!;Star+%E2%AD%90+this+repo+if+you+like+it!" alt="Footer Typing SVG" />

**© 2026 Rocky Chowdhury. All rights reserved.**

</div>
