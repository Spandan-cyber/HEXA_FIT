# ⬡ HexaFit V2

> **Trainer-grade guidance, no trainer required.**

HexaFit is a modern, AI-powered fitness web app that gives you real-time posture analysis, workout tracking, and personalized fitness guidance — all from your browser.

---

## 🚀 Features

- **Real-time Posture Analysis** — Uses MediaPipe Pose to detect and score your posture live via webcam
- **AI Workout Guidance** — Step-by-step exercise coaching with angle feedback
- **Google Authentication** — Secure sign-in via Firebase Auth + Google OAuth
- **Firebase Analytics** — Integrated usage tracking with Firebase Analytics
- **Responsive Design** — Fully mobile-friendly with a bold neobrutalist UI
- **No Installation Required** — Runs entirely in the browser via CDN

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| UI Framework | React 18 (UMD via CDN) |
| Styling | Vanilla CSS (neobrutalist design) |
| Pose Detection | MediaPipe Pose |
| Authentication | Firebase Auth (Google Sign-In) |
| Analytics | Firebase Analytics |
| Fonts | Anton, Space Grotesk, Space Mono (Google Fonts) |
| Local Server | Node.js HTTP server |

---

## 📁 Project Structure

```
HEXAFIT V2/
├── hexafit.html        # Main single-page app
├── server.js           # Local Node.js dev server
├── package.json        # npm dependencies
├── .gitignore          # Git ignore rules
└── README.md           # This file
```

---

## 🔧 Running Locally

### Prerequisites
- [Node.js](https://nodejs.org/) installed

### Steps

```bash
# 1. Clone the repository
git clone https://github.com/Spandan-cyber/HEXA_FIT.git
cd HEXA_FIT

# 2. Install dependencies
npm install

# 3. Start the local server
node server.js

# 4. Open your browser
# Visit: http://localhost:3000
```

---

## 🔥 Firebase Setup

This project uses Firebase for authentication and analytics. The config is already embedded in `hexafit.html`.

**Firebase Services Used:**
- `firebase-app` — Core Firebase initialization
- `firebase-analytics` — Usage analytics
- `firebase-auth` — Google Sign-In authentication

To use your own Firebase project:
1. Go to [Firebase Console](https://console.firebase.google.com/)
2. Create a new project
3. Add a Web App and copy your config
4. Replace the `firebaseConfig` object in `hexafit.html`

---

## 📸 Screenshots

> Real-time posture detection, workout tracking, and more — all in one sleek interface.

---

## 📄 License

MIT License © 2026 [Spandan-cyber](https://github.com/Spandan-cyber)

---

## 🙌 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

<p align="center">Built with ❤️ by <a href="https://github.com/Spandan-cyber">Spandan</a></p>
