# HEXA FIT

### Trainer-grade guidance. No trainer required.

**HEXA FIT** is a modern, browser-based fitness guidance platform designed to bring structured workout assistance, movement awareness, and a trainer-inspired experience directly to the user.

Built with a bold, responsive interface and browser-native technologies, HEXA FIT combines **React**, **Google authentication**, **Firebase**, and **MediaPipe Pose** into a lightweight fitness experience that runs directly in the browser.

---

## ⚡ What is HEXA FIT?

HEXA FIT is built around a simple idea:

> **Make high-quality fitness guidance accessible without requiring a personal trainer.**

Instead of presenting fitness as another collection of static workout pages, HEXA FIT is designed as an interactive experience.

The platform focuses on:

- 🏋️ Workout guidance
- 🧍 Movement and posture awareness
- 📐 Pose-based analysis
- 🔐 User authentication
- 📱 Responsive design
- ⚡ Fast browser-based execution
- 🎯 Trainer-inspired feedback
- 🎨 Distinctive visual identity

---

## ✨ Core Experience

### 🧍 Pose & Movement Awareness

HEXA FIT integrates **MediaPipe Pose** to enable browser-based body and movement analysis.

This creates the foundation for features such as:

- Pose detection
- Movement tracking
- Exercise form awareness
- Posture analysis
- Real-time visual feedback

The goal is to move beyond simple workout instructions toward a more interactive training experience.

---

### 🔐 Authentication

HEXA FIT includes Google Identity Services integration for user authentication.

Authenticated users can be represented inside the application with:

- Profile information
- Profile image
- User identity
- Sign-out functionality

Firebase is included as a project dependency for application data and authentication-related expansion.

---

### 🎨 Distinctive UI

HEXA FIT intentionally avoids the conventional "generic fitness app" aesthetic.

Its visual system uses:

- High-contrast layouts
- Heavy typography
- Strong borders
- Offset shadows
- Neon lime accents
- Pink highlights
- Cobalt interaction states
- Monospace technical labels
- Responsive layouts
- Motion-driven interactions

The design language is deliberately energetic, physical, and technical.

---

## 🧠 Design Philosophy

HEXA FIT follows three principles:

### 01 — GUIDANCE

The application should help users understand **what to do**, not merely display information.

### 02 — AWARENESS

Movement should be observable.

The platform is designed around the idea that fitness technology should understand the user's movement rather than treating the user as a passive reader.

### 03 — ACCESSIBILITY

Trainer-style assistance should be available without requiring a trainer physically present.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| HTML5 | Application structure |
| CSS3 | UI, responsive design & animations |
| JavaScript | Application logic |
| React 18 | UI layer |
| Babel Standalone | Browser-side JSX transformation |
| Node.js | Local application server |
| Firebase | Application/backend services |
| Google Identity Services | Authentication |
| MediaPipe Pose | Pose estimation |
| Google Fonts | Typography |

---

## 📁 Project Structure

```text
HEXA_FIT-main/
│
├── index.html
├── server.js
├── package.json
├── .gitignore
└── README.md
```

### `index.html`

The primary application entry point.

It contains the HEXA FIT interface, styling, React application logic, authentication integration, and MediaPipe integration.

### `server.js`

A lightweight Node.js static file server.

It:

- Serves `index.html`
- Handles static assets
- Provides MIME types
- Supports SPA-style fallback
- Runs on port `3000`
- Allows access from the local network

### `package.json`

Defines the project's Node.js dependency configuration.

Current dependency:

```text
firebase
```

---

# 🚀 Getting Started

## Prerequisites

Make sure the following are installed:

- Node.js
- npm
- A modern web browser

Recommended browsers include current versions of:

- Chrome
- Edge
- Firefox

For the best experience with camera and pose functionality, use a Chromium-based browser.

---

## 1. Clone or Extract the Project

Place the project somewhere convenient:

```text
HEXA_FIT-main/
```

Open a terminal inside the project directory.

---

## 2. Install Dependencies

Run:

```bash
npm install
```

---

## 3. Start HEXA FIT

Run:

```bash
node server.js
```

The server will start on:

```text
http://localhost:3000
```

Open that address in your browser.

---

## 🌐 Network Access

The server listens on:

```text
0.0.0.0:3000
```

This means HEXA FIT can also be accessed from another device on the same local network using the host machine's local IP address:

```text
http://YOUR_LOCAL_IP:3000
```

Camera and authentication functionality may require additional browser security configuration depending on how the application is accessed.

---

# 🔐 Authentication Configuration

HEXA FIT includes Google Identity Services.

For production deployment, configure the appropriate Google OAuth credentials and authorized origins.

Do **not** commit private credentials, API secrets, service-account keys, or other sensitive configuration to the repository.

---

# 📷 Camera & Pose Detection

HEXA FIT uses MediaPipe Pose through browser-delivered libraries.

The application can use the device camera to provide the visual input required for pose analysis.

Users should grant camera permission when prompted.

Camera functionality may be affected by:

- Browser permissions
- HTTPS requirements
- Device camera availability
- Browser compatibility
- Network configuration

---

# 📱 Responsive Design

HEXA FIT is designed to work across different screen sizes.

The interface adapts for:

- Desktop
- Laptop
- Tablet
- Mobile

The navigation system switches to a mobile menu at smaller viewport sizes.

---

# ♿ Accessibility & Motion

HEXA FIT includes support for users who prefer reduced motion.

When the browser reports:

```text
prefers-reduced-motion: reduce
```

the application significantly reduces animation and transition effects.

Keyboard focus states are also visually emphasized.

---

# 🎯 Project Goals

HEXA FIT is intended to evolve into a more complete fitness technology platform.

Potential future directions include:

- Personalized workout programs
- Exercise libraries
- Rep counting
- Form scoring
- Movement classification
- Workout history
- Progress tracking
- User profiles
- Training analytics
- Goal tracking
- AI-assisted fitness guidance
- Mobile optimization
- Advanced pose analysis
- Cloud synchronization
- Personalized recommendations

---

# 🧩 Architecture Direction

The current project intentionally keeps the application lightweight.

The long-term architecture can evolve toward:

```text
                    ┌──────────────────┐
                    │     HEXA FIT     │
                    │   User Interface │
                    └────────┬─────────┘
                             │
             ┌───────────────┼───────────────┐
             │               │               │
             ▼               ▼               ▼
        Authentication   Fitness Logic   Pose Engine
             │               │               │
             ▼               ▼               ▼
          Google          Workouts       MediaPipe
             │               │               │
             └───────────────┼───────────────┘
                             │
                             ▼
                         Firebase
```

The architecture can progressively separate the current single-page implementation into dedicated application modules as HEXA FIT grows.

---

# 🛡️ Privacy & Safety

HEXA FIT deals with potentially sensitive fitness and movement information.

A production implementation should follow privacy-first principles.

Important considerations include:

- Request camera access only when necessary.
- Clearly explain why camera access is required.
- Avoid unnecessary collection of raw camera footage.
- Minimize personally identifiable information.
- Protect authentication data.
- Secure backend communication.
- Provide users with control over their information.

> HEXA FIT is a fitness technology platform, not a replacement for qualified medical or clinical advice.

Users with injuries, medical conditions, or exercise restrictions should seek appropriate professional guidance before undertaking strenuous physical activity.

---

# 🧪 Development

Start the local server:

```bash
node server.js
```

Then open:

```text
http://localhost:3000
```

For development, edit the source files and refresh the browser.

---

# 📦 Deployment

HEXA FIT can eventually be deployed using a suitable Node.js-compatible hosting environment or adapted for static hosting if server functionality is no longer required.

A production deployment should include:

- HTTPS
- Production authentication configuration
- Secure Firebase configuration
- Proper domain configuration
- Environment-specific settings
- Error handling
- Monitoring
- Performance optimization
- Privacy documentation

---

# 🗺️ Roadmap

### Phase I — Foundation

- [x] Core HEXA FIT interface
- [x] Responsive navigation
- [x] Trainer-inspired visual system
- [x] Node.js development server
- [x] Google authentication integration
- [x] MediaPipe Pose integration
- [x] Reduced-motion support

### Phase II — Training Intelligence

- [ ] Exercise recognition
- [ ] Automatic repetition counting
- [ ] Form analysis
- [ ] Movement scoring
- [ ] Real-time feedback
- [ ] Workout sessions

### Phase III — Personalization

- [ ] User profiles
- [ ] Fitness goals
- [ ] Personalized programs
- [ ] Progress history
- [ ] Training analytics
- [ ] Adaptive recommendations

### Phase IV — Platform

- [ ] Cloud synchronization
- [ ] Advanced analytics
- [ ] AI-assisted coaching
- [ ] Expanded exercise library
- [ ] Mobile-first optimization
- [ ] Production infrastructure

---

# ⚠️ Current Status

**Project Status:** Active Development

**Version:** `0.1.0`

HEXA FIT is currently an evolving prototype/foundation rather than a finished production fitness platform.

Interfaces, architecture, APIs, authentication flows, and fitness-analysis capabilities may change as development progresses.

---

# 📄 License

A license has not yet been specified for this project.

Until a license is added, the repository should be treated as **all rights reserved** by the project owner.

If HEXA FIT is later intended to be open source, add an explicit license such as MIT, Apache-2.0, or another appropriate license.

---

# 💡 Vision

HEXA FIT is not meant to be another workout website.

The larger ambition is to create a fitness system where technology can observe, understand, and guide movement in a way that feels immediate and useful.

```text
SEE
  ↓
UNDERSTAND
  ↓
GUIDE
  ↓
TRAIN
  ↓
IMPROVE
```

**HEXA FIT**

> **Trainer-grade guidance. No trainer required.**

---

## Built for movement. Designed for progress.
