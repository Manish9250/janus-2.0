# Janus 2.0 👁️

**Janus 2.0** is a deeply integrated personal AI assistant designed specifically for the **Ubuntu** ecosystem. Unlike standard chatbots, Janus lives inside the OS, bridging the gap between high-level LLM intelligence and low-level system control.

## 🚀 Architecture

Janus 2.0 operates using a decoupled Client-Server architecture to ensure system stability and performance:

* **Brain (Backend):** A Python-based local server that handles:
    * LLM Inference / API calls (Gemini, OpenAI, or Local LLaMA).
    * System command execution (via `subprocess`).
    * Context management.
* **Face (Frontend):** A custom **GNOME Shell Extension** (JavaScript/GJS) that:
    * Resides in the system tray/top bar.
    * Captures user input (Voice/Text).
    * Displays responses natively in the OS UI.

## 🛠️ Tech Stack

* **OS:** Ubuntu (Linux)
* **Backend:** Python 3.x (FastAPI/Flask, Systemd)
* **Frontend:** JavaScript (GJS - GNOME JavaScript)
* **Communication:** WebSockets / REST API

## 📂 Project Structure

```text
janus-2.0/
├── backend/            # Python server logic
│   ├── core/           # LLM and System logic
│   ├── server.py       # API entry point
│   └── requirements.txt
├── extension/          # GNOME Shell Extension files
│   ├── extension.js    # Main UI logic
│   ├── metadata.json   # Extension config
│   └── stylesheet.css  # UI Styling
└── README.md
```

## 💿 Installation
Instructions coming soon...

## 📝 Usage
Instructions coming soon...

## 📜 License
MIT
