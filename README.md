# 🤖 AtlasHub
### More than a bot — a full automation hub

![License](https://img.shields.io/badge/License-GPL%20v3-blue.svg)
![Commercial License](https://img.shields.io/badge/Commercial-License%20Available-gold)
![Version](https://img.shields.io/badge/version-1.9-black)
![Node](https://img.shields.io/badge/node-%3E=20-green)
![Status](https://img.shields.io/badge/status-stable-brightgreen)
![WhatsApp Bot](https://img.shields.io/badge/platform-WhatsApp-25D366)
![Company](https://img.shields.io/badge/Kinetic-Space%20Inc.-purple)

[![Discord](https://img.shields.io/badge/Discord-Join-5865F2?logo=discord&logoColor=white)](https://discord.gg/AkQenmwgV3)
[![WhatsApp Channel](https://img.shields.io/badge/WhatsApp-Channel-25D366?logo=whatsapp&logoColor=white)](https://www.whatsapp.com/channel/0029VbCBwNP9RZAXiMPOAe3f)

> All-in-one WhatsApp bot platform — economy, games, moderation, leveling system and web dashboard.

---

# 🌍 Community & Support

Stay connected with updates, releases and support.

## 💬 Discord (Support • Premium • Help • Community)
👉 https://discord.gg/AkQenmwgV3

Inside Discord you can:
- Get technical support
- Report bugs
- Suggest features
- Receive updates
- Access premium versions
- Buy tokens / premium access
- Talk with the AtlasHub community

## 📢 WhatsApp Channel (News • Releases • Announcements)
👉 https://www.whatsapp.com/channel/0029VbCBwNP9RZAXiMPOAe3f

Official place for:
- News
- Version releases
- Changelogs
- Improvements
- Project announcements

---

# 🚀 What is AtlasHub?

AtlasHub is an advanced **WhatsApp automation platform** developed by **Kinetic Space Inc.**

It goes far beyond a simple chatbot and acts as a complete ecosystem:

- 💰 Economy system
- 🎮 Games
- 🛡 Moderation
- 📊 Levels & ranking
- 🌐 Web dashboard
- ⚙ Modular commands
- 🔌 Developer friendly API

Designed for communities, businesses and large groups.

---

# ✨ Features

| System | Included |
|------------|------------|
| Economy | ✅ |
| Games | ✅ |
| Moderation | ✅ |
| XP & Levels | ✅ |
| Rankings | ✅ |
| Dashboard | ✅ |
| Multi-group | ✅ |
| Anti-spam | ✅ |
| Modular commands | ✅ |

---

# 🛠 Tech Stack

```
Node.js
whatsapp-web.js
Express
Puppeteer
JSON / SQLite
```

---

# 📦 Installation

## Requirements
- Node.js 18+
- NPM
- WhatsApp account

## Setup

```bash
git clone https://github.com/YOUR_USER/atlashub
cd atlashub
npm install
node index.js
```

---

# ⚙ Configuration

Create `.env` file:

```
PREFIX=#
PORT=3000
SESSION_NAME=atlas
```

---

# 🔑 Command Prefix

```
#
```

Example:
```
#menu
```

---

# 📚 Commands

## 💰 Economy
```
#daily
#work
#balance
#bank
#deposit
#withdraw
#pay
```

## 🎮 Games
```
#coinflip
#dice
#slots
#rps
#blackjack
```

## 👤 Profile
```
#profile
#level
#rank
#top
```

## ⚙ Utility
```
#menu
#ping
#uptime
#info
```

## 👑 Admin
```
#warn
#reset
#addcoins
#ban
#unban
```

---

# 🧠 Architecture

```
User
  ↓
whatsapp-web.js
  ↓
AtlasHub Core
  ├─ Commands
  ├─ Economy
  ├─ Games
  ├─ Moderation
  ↓
Database
  ↓
Web Panel (Express)
```

---

# 📁 Project Structure

```
atlashub/
│
├─ src/
│   ├─ core/
│   ├─ commands/
│   ├─ database/
│   └─ utils/
│
├─ panel/
├─ data/
├─ docs/
│
├─ index.js
├─ package.json
├─ README.md
└─ LICENSE
```

---

# 🔌 Developer API

Create commands easily:

```js
module.exports = {
  name: "ping",
  cooldown: 3000,
  run: async (client, message) => {
    message.reply("Pong!");
  }
}
```

---

# 🌐 Web Panel

Run:

```bash
npm run panel
```

Open:

```
http://localhost:3000
```

Features:
- User stats
- Economy management
- Logs
- Monitoring
- System control

---

# 🤝 Contributing

1. Fork
2. Create branch
3. Commit
4. Pull Request

We welcome contributions ❤️

---

# 🏢 Organization

Developed by:

**Kinetic Space Inc.**

Software • Automation • AI • Platforms

---

# 📬 Contact

### 🤖 AI Department
Kinetic.AI@post.com

### 🌐 General / Business
KineticSpaceOfficial@gmail.com

---

## 📜 License

AtlasHub is distributed under a **Dual License model**:

### 🟢 Open Source
GNU GPL v3 – Free and open-source usage.

### 🔵 Commercial
For private, closed-source, SaaS or enterprise usage,
a commercial license is required.

Contact:
Kinetic.AI@post.com
KineticSpaceOfficial@gmail.com


---

# ⭐ AtlasHub
### More than a bot — a full automation hub
