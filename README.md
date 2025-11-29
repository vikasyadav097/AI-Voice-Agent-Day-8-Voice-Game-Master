---

# 🎮 Voice Game Master – AI-Powered D&D Adventure

An immersive, voice-driven Dungeons & Dragons experience featuring real-time AI narration, natural conversation flow, tactical combat, and a stunning cyberpunk interface. Built using **LiveKit Agents** and **Murf.ai Falcon** for ultra-fast, realistic voice synthesis.

**Tags:** Cyberpunk UI • Voice AI • Real-Time Interaction

---

## ✨ Features

### 🎭 Immersive Gameplay

* **Real-time voice interaction** with an AI Game Master
* **Dynamic storytelling** where every decision shapes the world
* **Automated D20 dice rolls** with modifiers
* **Character progression:** HP, stats, inventory, quests
* **Cinematic narrative scenes** and dramatic encounters

### 🎨 Cyberpunk UI

* Dark theme with **neon cyan + purple** futuristic glow
* Animated backgrounds with particles
* Real-time **character sheet updates**
* Built-in **audio visualizer** for AI speech
* Fully responsive across all devices

### 🤖 AI-Powered Engine

* Natural Language Understanding for complex commands
* Context-aware memory of choices and game state
* Dynamic quest generation
* Intelligent combat + dice mechanics
* Smart inventory/skills management

---

## 🚀 Quick Start

### **Prerequisites**

* Node.js 18+ & pnpm
* Python 3.11+
* LiveKit account
* Murf.ai API key

---

## 📥 Installation

### 1. Clone the repository

```bash
git clone https://github.com/vikasyadav097/AI-Voice-Agent-Day-8-Voice-Game-Master 
```

---

### 2. Backend Setup

```bash
cd backend
python -m venv .venv
```

**Activate venv**

Windows:

```bash
.venv\Scripts\activate
```

Mac/Linux:

```bash
source .venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

### 3. Configure Environment Variables

Create `backend/.env.local`:

```
LIVEKIT_URL=wss://your-livekit-url
LIVEKIT_API_KEY=your-api-key
LIVEKIT_API_SECRET=your-api-secret
MURF_API_KEY=your-murf-api-key
OPENAI_API_KEY=your-openai-key
```

Create `frontend/.env.local`:

```
LIVEKIT_API_KEY=your-api-key
LIVEKIT_API_SECRET=your-api-secret
LIVEKIT_URL=https://your-livekit-url
```

---

### 4. Install Frontend Dependencies

```bash
cd ../frontend
pnpm install
```

---

## ▶️ Running the Application

### **Terminal 1 – LiveKit Server**

```bash
cd ten-days-of-voice-agents-2025
.\livekit-server.exe --dev
```

### **Terminal 2 – Backend Agent**

```bash
cd backend
.venv\Scripts\activate
python src/agent.py dev
```

### **Terminal 3 – Frontend**

```bash
cd frontend
pnpm dev
```

Open: **[http://localhost:3000](http://localhost:3000)**

---

## 🎮 How to Play

1. Click **START CALL**
2. Speak naturally—just like talking to a DM
3. Make decisions that alter the world
4. Use dice commands (e.g., "Roll perception")
5. Track stats on the live character sheet

### Example Commands

* “I look around for enemies.”
* “Roll for stealth.”
* “Check my inventory.”
* “I attack with my sword.”
* “I cast fireball.”

---

## 🏗️ Architecture Overview

### **Tech Stack**

* **Frontend:** Next.js 15, React, TypeScript, Tailwind CSS, Framer Motion
* **Backend:** Python, LiveKit Agents, OpenAI GPT-4
* **Voice Engine:** Murf.ai Falcon
* **Real-Time Layer:** LiveKit WebRTC

### **Project Structure**

```
ten-days-of-voice-agents-2025/
├── backend/
│   ├── src/
│   │   ├── agent.py
│   │   └── murf_tts.py
│   └── .env.local
├── frontend/
│   ├── components/app/
│   │   ├── welcome-view.tsx
│   │   ├── session-view.tsx
│   │   └── character-sheet.tsx
│   └── .env.local
├── shared-data/
│   └── game_state.json
└── livekit-server.exe
```

---

## 🎨 UI Customization

Cyberpunk palette:

* **Cyan:** `#00ffff`
* **Purple:** `#a855f7`
* **Pink:** `#ec4899`
* **Black:** `#000000`

Customize in:
`frontend/styles/globals.css`

---

## 🔧 Configuration Options

### **Game State**

Modify `shared-data/game_state.json` to alter:

* Character stats
* Inventory
* Quests
* NPCs & world details

### **Agent Behavior**

Edit `backend/src/agent.py` to configure:

* Game Master personality
* Dice logic
* Quest generation
* Combat mechanics

---

## 📝 API Keys Setup

### **LiveKit**

1. Create project
2. Copy API key + secret

### **Murf.ai**

1. Create account
2. Use Falcon model for fastest TTS

### **OpenAI**

1. Get API key
2. Use GPT-4 for best performance

---

## 🎯 Roadmap

* Multiplayer support
* Save/load campaigns
* Custom character creator
* Additional classes
* Advanced quest generator
* Combat animations
* SFX support
* Mobile app

---

## 🤝 Contributing

Pull requests are welcome — feel free to improve anything!

---

## 📄 License

Distributed under the **MIT License**.

---

## 🙏 Acknowledgments

* Built for the **Murf.ai Voice Agents Challenge**
* Powered by **LiveKit**, **Murf.ai**, and **OpenAI**

---
| Day      | Status         |
| -------- | -------------- |
| Day 1    | ✅ Completed    |
| Day 2    | ✅ Completed    |
| Day 3    | ✅ Completed    |
| Day 4    | ✅ Completed    |
| Day 5    | ✅ Completed    |
| Day 6    | ✅ Completed    |
| Day 7    | ✅ Completed    |
| Day 8    | ✅ Completed    |
| Day 9–10 | 🔜 Coming soon |


⭐ *If you like this project, don’t forget to star the repo!* ⭐

---


