<div align="center">

<img src="logo.png" alt="ClubConnect Logo" width="260"/>

# 🏆 ClubConnect

**An all-in-one sports club management platform for football, cricket, basketball, and hockey clubs.**

ClubConnect streamlines team management, scheduling, payments, performance tracking, and communication into one modern, role-based web application — built for players, coaches, club owners, and system administrators.

[![Live Demo](https://img.shields.io/badge/demo-live-success?style=for-the-badge)](https://clubconnect-sports.netlify.app/)
[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](LICENSE)
![Status](https://img.shields.io/badge/status-active-brightgreen?style=for-the-badge)

[🌐 Live Demo](https://clubconnect-sports.netlify.app/) • [✨ Features](#-features) • [🚀 Getting Started](#-getting-started) • [📁 Project Structure](#-project-structure) • [👥 User Roles](#-user-roles) • [🤝 Contributing](#-contributing)

</div>

---

## 📌 Overview

**ClubConnect** is a static, fully client-side web platform designed to bring sports clubs, academies, and training centers into one connected system. It replaces scattered spreadsheets, WhatsApp groups, and paper registers with a single dashboard-driven experience for everyone involved in running a club — from the players on the field to the administrators overseeing the whole system.

The platform is built entirely with **HTML5, CSS3, and vanilla JavaScript** — no frameworks, no build step, no backend server required to run it. Data is persisted in the browser, and payments are handled through **Web3 / blockchain wallet integration** (MetaMask), making it deployable anywhere static files can be hosted.

> 🎓 Originally developed as a Fundamentals of Software Engineering project, ClubConnect has grown into a fully-featured demo platform showcasing multi-role dashboards, blockchain payments, and modern front-end architecture.

**🔗 Live Demo:** [https://clubconnect-sports.netlify.app/](https://clubconnect-sports.netlify.app/)

---

## ✨ Features

- 🏟️ **Team Management** — Create, organize, and manage teams across multiple sports
- 🧑‍🏫 **Coach & Player Management** — Hire coaches, register players, and track performance over time
- 📊 **Leaderboards** — Real-time performance leaderboards and rankings for teams and players
- 🧭 **Multi-Role Dashboards** — Purpose-built interfaces for Players, Coaches, Club Owners, and Super Admins
- 🥇 **Badges & Achievements** — Gamified performance tracking with unlockable badges (Hustler, Playmaker, and more)
- 💳 **Crypto Payments** — Secure blockchain-based payment processing via MetaMask (Sepolia testnet / Polygon mainnet)
- 💬 **Communication Hub** — Centralized contact, requests, and messaging system between roles
- 📅 **Training & Scheduling** — Session planning, squad overviews, and schedule tracking
- 🔒 **Source Protection** — Client-side developer tools and view-source restrictions
- 📱 **Fully Responsive** — Optimized layouts for desktop, tablet, and mobile
- ⚡ **Performance Optimized** — Preconnect hints, lazy-loaded images, deferred scripts, and aggressive caching via Netlify

---

## 🖼️ Screenshots

| Coach Dashboard | Player Dashboard |
|:---:|:---:|
| ![Coach Dashboard](coach-dashboard.png) | ![Player Dashboard](player-dashboard.png) |

| Owner Dashboard |
|:---:|
| ![Owner Dashboard](owner-dashboard.png) |

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Markup** | HTML5 (semantic elements) |
| **Styling** | CSS3 — custom properties / design tokens, mobile-first responsive layout |
| **Logic** | JavaScript (ES6+, vanilla — no frameworks) |
| **Payments** | Web3.js + MetaMask wallet integration |
| **Blockchain Networks** | Ethereum (Sepolia testnet), Polygon (mainnet) |
| **Icons** | [Font Awesome 6.4.0](https://fontawesome.com/) |
| **Typography** | [Google Fonts — Poppins](https://fonts.google.com/) |
| **Storage** | Browser `localStorage` / `sessionStorage` |
| **Hosting** | [Netlify](https://www.netlify.com/) (static hosting, custom headers, redirects) |

### Why no framework / backend?

ClubConnect is intentionally built as a **static, dependency-light front-end application**. This keeps it:
- Instantly deployable to any static host (Netlify, Vercel, GitHub Pages)
- Free of build tooling or compile steps
- Easy to read, fork, and learn from
- A clean foundation to later connect to a real backend/API (see [Roadmap](#-roadmap))

---

## 📁 Project Structure

```
clubconnect/
├── .github/
│   └── ISSUE_TEMPLATE/
│       ├── bug_report.md
│       ├── feature_request.md
│       └── pull_request_template.md
│
├── .editorconfig                 # Consistent editor/IDE settings
├── .gitignore                    # Git ignore rules
├── netlify.toml                  # Netlify build, headers & redirect config
├── package.json                  # Project metadata & scripts
│
├── index.html                    # Landing page
├── demo.html                     # Interactive demo / tutorial
├── features.html                 # Features overview
├── contact.html                  # Contact form & support
│
├── login.html                    # User login
├── signup.html                   # User registration
│
├── player-dashboard.html         # Player role dashboard
├── coach-dashboard.html          # Coach role dashboard
├── owner-dashboard.html          # Club owner dashboard
├── super-admin-dashboard.html    # System admin dashboard
│
├── teams.html                    # Team management
├── leaderboards.html             # Performance leaderboards
│
├── privacy.html                  # Privacy policy
├── cookies.html                  # Cookie policy
├── terms.html                    # Terms of service
│
├── app.js                        # Core application logic, payments, notifications
├── protection.js                 # Client-side source protection
├── style.css                     # Global design system & layouts
│
├── logo.png                      # Brand logo
├── coach-dashboard.png           # Screenshot
├── owner-dashboard.png           # Screenshot
├── player-dashboard.png          # Screenshot
├── hero.mp4                      # Landing page hero video
├── v_back.mp4                    # Background video
│
├── README.md                     # You are here
├── ARCHITECTURE.md               # Technical architecture deep-dive
├── DEPLOYMENT.md                 # Deployment instructions
├── SECURITY.md                   # Security policy
├── CONTRIBUTING.md               # Contribution guidelines
├── CODE_OF_CONDUCT.md            # Community standards
├── CHANGELOG.md                  # Version history
├── HTML_OPTIMIZATION_GUIDE.md    # Front-end performance checklist
├── PERFORMANCE_OPTIMIZATION.md   # Performance strategy & metrics
└── LICENSE                       # MIT License
```

> 📐 For a deeper technical breakdown — layered architecture, data flow, and module dependencies — see [ARCHITECTURE.md](ARCHITECTURE.md).

---

## 🚀 Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, or Edge)
- JavaScript enabled
- [MetaMask](https://metamask.io/) (or another Web3 wallet) — only needed to test crypto payment flows

### Installation

**1. Clone the repository**

```bash
git clone https://github.com/Zubair378/Sports-and-club-management-system.git
cd Sports-and-club-management-system
```

**2. Run it locally**

No build step is required — this is a static site. Pick whichever runner you have available:

```bash
# Python 3
python -m http.server 8000

# Node.js (no install needed)
npx http-server -p 8000

# Or use the npm script
npm run dev
```

**3. Open in your browser**

```
http://localhost:8000
```

That's it — no `npm install`, no compiling, no `.env` setup required to view the site.

---

## ⚙️ Configuration

### Blockchain / Payment Settings

Wallet and payment configuration lives in `app.js`:

```javascript
window.OWNER_WALLET_ADDRESS = "0xe2d165ab23cd2ed0cafb969b8bc55b9a71f17b5c";
window.PAYMENT_AMOUNTS = {
  playerRegistration: "0.01",  // ETH
  coachHiring: "0.02",         // ETH
  clubPayment: "0.05"          // ETH
};
window.SEPOLIA_CHAIN_ID = "0xaa36a7";  // Testnet
window.POLYGON_CHAIN_ID = "0x89";      // Mainnet
```

> ℹ️ The wallet address above is a **demo address** for testing on Sepolia testnet — swap it for your own before processing real funds.

---

## 👥 User Roles

ClubConnect ships with four distinct, purpose-built dashboards:

### 🏃 Players
- Sign up and join clubs/teams
- View profile, performance stats, and badges
- Check leaderboard rankings
- Track training schedule and submit requests
- Manage payments

### 🧑‍🏫 Coaches
- Manage assigned teams and squads
- Review players and leave performance feedback
- Plan and manage training sessions
- Track performance with built-in analytics

### 🏢 Club Owners
- Create and manage teams
- Hire coaches (no registration fee charged to coaches)
- Manage club profile, payroll, and payments
- Enroll in leagues and track club achievements/challenges

### 🛡️ Super Admins
- Manage all clubs, users, and roles across the system
- Monitor platform-wide metrics
- Generate reports and oversee system administration

---

## 🔒 Security Features

- **Source Code Protection** — Developer tools, view-source, and common inspection shortcuts (F12, Ctrl+U, Ctrl+Shift+I/J/C, etc.) are intercepted client-side
- **Context Menu Protection** — Right-click is disabled
- **Blockchain Payments** — Transparent, wallet-signed transactions instead of stored card data
- **No Sensitive Data Storage** — Passwords are never persisted in browser storage

> ⚠️ **Note:** Client-side protections (disabled dev tools, right-click, etc.) are deterrents, not absolute security. They can be bypassed by a determined user. See [SECURITY.md](SECURITY.md) for the full policy, server-side recommendations, and how to responsibly report a vulnerability.

---

## 🌐 Browser Compatibility

| Browser | Version | Status |
|---|---|---|
| Chrome | 90+ | ✅ Supported |
| Firefox | 88+ | ✅ Supported |
| Safari | 14+ | ✅ Supported |
| Edge | 90+ | ✅ Supported |
| Mobile (iOS) | 14+ | ✅ Supported |
| Mobile (Android) | 10+ | ✅ Supported |

---

## ⚡ Performance

ClubConnect's front end is tuned for fast load times even though it's media-rich:

- `preconnect` hints for Google Fonts & Font Awesome
- Critical CSS preloading
- Deferred script loading (`protection.js`, `app.js`)
- Lazy-loaded images
- Long-term immutable caching for static assets via `netlify.toml`
- Reduced font-weight loading (only the weights actually used)

See [PERFORMANCE_OPTIMIZATION.md](PERFORMANCE_OPTIMIZATION.md) and [HTML_OPTIMIZATION_GUIDE.md](HTML_OPTIMIZATION_GUIDE.md) for the full strategy and measured impact.

---

## 💳 Payment Processing

| | |
|---|---|
| **Testnet** | Sepolia (`0xaa36a7`) |
| **Mainnet** | Polygon (`0x89`) |
| **Wallet Integration** | MetaMask-compatible |

| Transaction Type | Amount |
|---|---|
| Player Registration | 0.01 ETH |
| Coach Hiring | 0.02 ETH |
| Club Operations | 0.05 ETH |

---

## 🗺️ Roadmap

- [ ] Backend API + database (move off browser-only storage)
- [ ] Real-time notifications via WebSocket
- [ ] Advanced analytics dashboard
- [ ] Video integration for game reviews
- [ ] Native iOS & Android applications
- [ ] Public REST API documentation
- [ ] Multi-language support (i18n)
- [ ] Advanced roles & granular permissions

Full version history is tracked in [CHANGELOG.md](CHANGELOG.md).

---

## 📖 Documentation

| Doc | Description |
|---|---|
| [ARCHITECTURE.md](ARCHITECTURE.md) | Technical architecture, data flow, module dependencies |
| [DEPLOYMENT.md](DEPLOYMENT.md) | Deployment instructions for Netlify, Vercel, Docker, etc. |
| [SECURITY.md](SECURITY.md) | Security policy & vulnerability reporting |
| [CONTRIBUTING.md](CONTRIBUTING.md) | How to contribute, style guide, PR process |
| [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) | Community standards |
| [CHANGELOG.md](CHANGELOG.md) | Version history & roadmap |
| [PERFORMANCE_OPTIMIZATION.md](PERFORMANCE_OPTIMIZATION.md) | Performance strategy & metrics |

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for our code style guide, branch naming, and PR process before submitting changes.

```bash
# 1. Fork the repository
# 2. Create your feature branch
git checkout -b feature/AmazingFeature

# 3. Commit your changes
git commit -m "Add AmazingFeature"

# 4. Push to your branch
git push origin feature/AmazingFeature

# 5. Open a Pull Request
```

---

## 📜 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.

---

## 📞 Support & Feedback

- 📧 Contact: via the [Contact Page](contact.html)
- 🔐 Privacy: [Privacy Policy](privacy.html)
- ⚖️ Legal: [Terms of Service](terms.html)
- 🍪 Cookies: [Cookie Policy](cookies.html)

## 🙏 Acknowledgments

- [Font Awesome](https://fontawesome.com/) — icon library
- [Google Fonts](https://fonts.google.com/) — typography
- [Ethereum](https://ethereum.org/) — Web3 resources
- [MetaMask](https://metamask.io/) — wallet integration
- [Netlify](https://www.netlify.com/) — hosting & deployment

---

<div align="center">

**Made with ❤️ for sports club management**

[🌐 Live Demo](https://clubconnect-sports.netlify.app/) • [📂 Repository](https://github.com/Zubair378/Sports-and-club-management-system) • [🐛 Report Bug](https://github.com/Zubair378/Sports-and-club-management-system/issues) • [✨ Request Feature](https://github.com/Zubair378/Sports-and-club-management-system/issues)

</div>
