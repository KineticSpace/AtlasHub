# 🤖 AtlasHub

AtlasHub es un bot avanzado para WhatsApp desarrollado en Node.js utilizando la librería **whatsapp-web.js**.  
Este repositorio corresponde **exclusivamente** a la edición **Open Source** del proyecto.

Proyecto propiedad de **Kinetic Space Inc.**

---

## Edición Lite (Open Source)

La edición Lite es **pública**, **educativa** y **autohospedable**.

**❌ No incluye:**
- Funciones premium  
- Comercio  
- Sistemas de pago  
- Características privadas de la versión FULL  

La versión FULL existe, pero **NO** se documenta en este repositorio.

---

## ⚙️ Arquitectura General (Lite)

- Sistema de comandos modular  
- Core desacoplado  
- Sistema económico básico  
- Juegos de azar  
- Perfiles de usuario  
- Ranking  
- Panel web local  
- Persistencia de datos local (JSON)  

---

## 🎮 Juegos Incluidos (Lite)

- Coinflip  
- Dice  
- Roulette  
- Higher / Lower  
- Slots  
- Blackjack  
- Lottery  

---

## 📲 Comandos

**Prefijo global:** `!`

### Economía
- `!balance`  
- `!daily`  
- `!work`  
- `!profile`  

### Juegos
- `!coinflip`  
- `!dice`  
- `!roulette`  
- `!higherlow`  
- `!slots`  
- `!blackjack`  
- `!lottery`  

### Ranking
- `!leaderboard`  
- `!rank`  
- `!stats`  

### Utilidad
- `!help`  
- `!info`  
- `!ping`  
- `!version`  
- `!botinfo`  

---

## 🧰 Requisitos

- Node.js v18 o superior  
- npm  
- Cuenta activa de WhatsApp  

---

## 📊 Panel Web Local

Disponible en:
http://localhost:3000

Incluye:

Estado del bot

Estadísticas básicas

Ranking

---

## 📂 Estructura del proyecto
AtlasHub/
│
├─ core/
│  ├─ economy.js
│  ├─ games.js
│  ├─ database.js
│  ├─ commands.js
│  └─ utils.js
│
├─ panel/
│  └─ server.js
│
├─ index.js
├─ package.json
└─ .env

---

## Configuracion (.env)
BOT_NAME=AtlasHub
BOT_VERSION=2.1.0-LITE
BOT_PREFIX=!
OWNER_ID=XXXXXXXXXX@c.us
PORT=3000

---

## Licencia

Este proyecto utiliza licencia dual:

MIT

GPL-3.0

---

## Contribuciones

Se aceptan Pull Requests.
El código debe respetar estrictamente la arquitectura existente del proyecto.

---

## Comunidad y Contacto

Discord: https://discord.gg/AkQenmwgV3

Canal de WhatsApp: https://www.whatsapp.com/channel/0029VbCBwNP9RZAXiMPOAe3f

---

# Créditos

AtlasHub es un proyecto desarrollado por Kinexa Inc.
La edición Open Source (Lite) representa la base pública del ecosistema AtlasHub.

---

## 📦Instalación

```bash
git clone https://github.com/KineticSpaceInc/AtlasHub
cd AtlasHub
npm install
npm start
Durante el primer inicio se generará un código QR para vincular WhatsApp Web.
