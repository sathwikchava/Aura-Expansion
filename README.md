<div align="center">

# 🌐 Aura Expansion

### An immersive 3D virtual meeting & learning platform built in Unity

*Step out of the video-call grid and into a shared virtual space — as an avatar.*

[![Unity](https://img.shields.io/badge/Engine-Unity%203D-000000?logo=unity&logoColor=white)](https://unity.com/)
[![C#](https://img.shields.io/badge/Language-C%23-239120?logo=csharp&logoColor=white)](https://learn.microsoft.com/en-us/dotnet/csharp/)
[![Photon PUN](https://img.shields.io/badge/Multiplayer-Photon%20PUN-6A1B9A)](https://www.photonengine.com/pun)
[![Gemini API](https://img.shields.io/badge/AI-Google%20Gemini%20API-4285F4?logo=googlegemini&logoColor=white)](https://ai.google.dev/)
[![PlayFab](https://img.shields.io/badge/Backend-PlayFab%20%2B%20Azure-107C10?logo=microsoftazure&logoColor=white)](https://playfab.com/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](#license)

[Demo](#-demo) • [Features](#-features) • [Tech Stack](#-tech-stack) • [Architecture](#-architecture) • [Getting Started](#-getting-started) • [Team](#-team)

</div>

---

## 📖 Overview

**Aura Expansion** reimagines what an online meeting or classroom can feel like. Instead of flattening every participant into a grid of video tiles, it drops them into a shared **3D virtual environment** where they're represented as **avatars** that can move, talk, and interact in real time — all from a regular screen, no VR headset required.

It was built to close the gap between the convenience of online meetings and the presence of being in the same room, combining real-time multiplayer, an interactive whiteboard, and an AI chatbot into a single Unity experience.

> This project began as **[VR-Classroom](https://github.com/AnnavarapuGanesh/VR-CLASSROOM)** — a single-user immersive classroom prototype — and **Aura Expansion is its multiplayer evolution**, adding Photon-powered real-time networking and PlayFab/Azure backend integration on top of the original concept.

## 🎥 Demo

▶️ **[Watch the project demo video](https://drive.google.com/file/d/105t2VANDtn_SxQQtPohvnpj__QxLZzC3/view?usp=sharing)**

## 🧩 Problem

Online meetings and classes often feel distant and disengaging. Static video tiles make natural interaction hard, weaken collaboration, and leave learners and teams feeling less connected than they would be in person.

## ✅ Solution

Aura Expansion places every participant inside a shared **metaverse-style virtual space**. Users join as 3D avatars, move around freely, collaborate on a shared whiteboard, and can even ask an AI chatbot for help — all accessible through a normal screen, keeping the experience lightweight and hardware-agnostic while still feeling far more natural than a typical video call.

## ✨ Features

| Feature | Description |
|---|---|
| 🧍 **3D Avatars** | Every participant is represented by a customizable avatar inside the shared environment, giving meetings real spatial presence. |
| 🔴 **Real-Time Multiplayer** | Powered by Photon PUN, so multiple users can join, move, and interact in the same session simultaneously. |
| 🖊️ **Virtual Whiteboard** | A shared, interactive whiteboard for teaching, brainstorming, and live collaboration. |
| 🤖 **AI Chatbot** | A Gemini API–powered assistant embedded in the environment for instant help and Q&A. |
| 🖥️ **Screen-First Accessibility** | Runs on a regular desktop screen — no dedicated VR hardware needed to participate. |
| ☁️ **Cloud & Backend Integration** | PlayFab and Azure handle backend services to support authentication, sessions, and data. |

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Game Engine | **Unity 3D** |
| Programming Language | **C#** |
| Multiplayer Networking | **Photon PUN** |
| AI Chatbot | **Google Gemini API** |
| Backend / Cloud | **Azure** + **PlayFab** |
| Version Control | **Git / GitHub** |

## 🏗️ Architecture

```
                        ┌───────────────────────┐
                        │         User           │
                        │   (Regular Screen)     │
                        └───────────┬────────────┘
                                    │
                                    ▼
                        ┌───────────────────────┐
                        │       Unity 3D         │
                        │  Virtual Meeting Space │
                        └──────┬─────────┬───────┘
                               │         │
              ┌────────────────┘         └────────────────┐
              ▼                                            ▼
   ┌────────────────────┐                       ┌────────────────────┐
   │    Photon PUN       │                       │  Interactive Layer  │
   │  Real-Time Sync      │                       │  Avatars • Whiteboard│
   └──────────┬──────────┘                       └──────────┬──────────┘
              │                                              │
              ▼                                              ▼
   ┌────────────────────┐                       ┌────────────────────┐
   │  Other Participants │                       │   Gemini AI Chatbot │
   └─────────────────────┘                       └─────────────────────┘

                        ┌───────────────────────┐
                        │    Azure + PlayFab      │
                        │  Backend & Cloud Layer  │
                        └───────────────────────┘
```

## 🚀 Getting Started

### Prerequisites

- **Unity Hub** + a Unity Editor version matching this project's `ProjectSettings`
- **Git**
- A **Photon PUN** App ID ([create one free on the Photon dashboard](https://www.photonengine.com/pun))
- A **Google Gemini API** key ([Google AI Studio](https://ai.google.dev/))
- A **PlayFab** Title ID (and Azure credentials, if you're using Azure-backed services)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/sathwikchava/Aura-Expansion.git
cd Aura-Expansion

# 2. Open the project in Unity Hub
#    Unity Hub → Add → select the cloned "Aura-Expansion" folder
#    Let Unity import assets and generate the local Library cache
```

### Configuration

Add your own credentials locally — **never commit real API keys or secrets**:

```
PHOTON_APP_ID=your_photon_app_id_here
GEMINI_API_KEY=your_gemini_api_key_here
PLAYFAB_TITLE_ID=your_playfab_title_id_here
```

1. Open **Window → Photon Unity Networking → PUN Wizard** and set your Photon App ID.
2. Add your Gemini API key to the chatbot script/config where indicated.
3. Set your PlayFab Title ID in the PlayFab settings window.
4. Open the main scene from `Assets/` and hit **Play**.

## 📂 Project Structure

```
Aura-Expansion/
├── Assets/              # Scenes, scripts, prefabs, models, materials, audio, etc.
├── Library/             # Unity-generated editor/import cache
├── Packages/            # Unity package manifest and dependency lock file
├── ProjectSettings/     # Unity project and editor configuration
├── Windows/             # Windows-related build/project files
├── *.csproj             # Generated C# project files
├── *.sln                # Visual Studio solution
├── .gitignore           # Git ignore rules
├── README.md            # Project documentation
└── LICENSE              # MIT License
```
## 🙏 Run
To directly run the final app/product/project we have made 
➡️"main\Windows\My project (3).exe"

## 🔮 Roadmap

- 💠 More realistic, customizable avatars with improved animations & expressions
- 💠 AI-powered virtual tutors for guided learning
- 💠 Multiple virtual classroom / meeting environment themes
- 💠 Native mobile support
- 💠 Full VR headset support

## 🌱 Benefits

- **Engaging learning environment** — feels closer to an in-person class than a standard video call
- **Enhanced collaboration** — students, teachers, and teammates interact instantly in a shared space
- **Interactive teaching tools** — whiteboard, avatars, and AI chat support richer sessions
- **Scalable** — fits classrooms, universities, and corporate training alike

## 🤝 Contributing

Contributions and ideas are welcome!

```bash
git checkout -b feature/your-feature
git commit -m "Add your feature"
git push origin feature/your-feature
```

Then open a pull request describing your change.

## 👥 Team — Hack Street Boys

| Name |
|---|
| **Ch. Sathwik** 
| **A. Ganesh**
| **M. V. Mourya Goud** |
| **C. Johith** |
## 📄 License

This project is licensed under the **MIT License** — feel free to fork, modify, and build on it for learning or development purposes.

## 🙏 Acknowledgements

Built with **Unity**, **Photon PUN**, **Google Gemini API**, **PlayFab**, and **Azure**.
