# Aura Expansion

> An immersive 3D virtual meeting and learning platform built with
> Unity, real-time multiplayer networking, AI-powered assistance, and
> interactive collaboration tools.

[![Unity](https://img.shields.io/badge/Engine-Unity%203D-black?logo=unity)](https://unity.com/)
[![C%23](https://img.shields.io/badge/Language-C%23-239120?logo=csharp&logoColor=white)](https://learn.microsoft.com/en-us/dotnet/csharp/)
[![Photon
PUN](https://img.shields.io/badge/Multiplayer-Photon%20PUN-6A1B9A)](https://www.photonengine.com/pun)
[![Gemini](https://img.shields.io/badge/AI-Gemini%20API-4285F4?logo=google)](https://ai.google.dev/)
[![PlayFab](https://img.shields.io/badge/Backend-PlayFab-107C10)](https://playfab.com/)

Aura Expansion explores a more interactive approach to online meetings
and collaborative learning. Instead of keeping participants inside a
conventional 2D video-call layout, the project places them together in a
shared 3D environment where they can communicate and interact through
avatars.

The platform combines **3D avatars, real-time multiplayer interaction, a
virtual whiteboard, and an AI chatbot** into one Unity-based experience.
It is designed to make remote collaboration feel more like being
together in the same space while remaining accessible through a regular
screen.

------------------------------------------------------------------------

## Demo

**Project demo:** Add your hosted demo video link here.

> Recommended: upload the demo to YouTube or another video host and
> replace the link above with the public URL.

------------------------------------------------------------------------

## Why Aura Expansion?

Traditional online meetings can make interaction feel distant and reduce
the sense of presence between participants. Aura Expansion approaches
the problem by creating a shared virtual space where users are
represented by avatars and can interact inside the environment.

The project is designed around four core ideas:

-   **Presence** --- participants share a 3D environment instead of
    appearing only as video tiles.
-   **Interaction** --- users can communicate and collaborate inside the
    same virtual space.
-   **Learning tools** --- interactive elements such as a virtual
    whiteboard support teaching and collaboration.
-   **AI assistance** --- an integrated chatbot provides an additional
    conversational interface.

------------------------------------------------------------------------

## Core Features

### 3D Avatars

Users are represented by 3D avatars inside the virtual environment,
giving meetings a stronger sense of presence than a conventional 2D
interface.

### Real-Time Multiplayer

Photon PUN provides the multiplayer layer required for participants to
share and interact within the same virtual space.

### Virtual Whiteboard

A shared whiteboard provides an interactive surface for teaching,
explaining concepts, and collaborative discussion.

### AI Chatbot

A Gemini-powered chatbot adds AI assistance to the environment and
provides a conversational interaction layer.

### Accessible Interaction

The experience is designed to work through a regular screen, making the
concept usable without requiring dedicated VR hardware.

------------------------------------------------------------------------

## Technology Stack

  Layer                         Technology
  ----------------------------- ---------------------------------------------------
  Game Engine                   Unity 3D
  Programming                   C#
  Multiplayer                   Photon PUN
  AI Chatbot                    Google Gemini API
  Backend / Cloud Integration   Azure + PlayFab
  3D Experience                 Unity-based virtual environment
  Collaboration                 Virtual whiteboard + real-time avatar interaction

The technology choices are based on the project architecture presented
in the project documentation. fileciteturn0file0L50-L54

------------------------------------------------------------------------

## High-Level Architecture

``` text
                         ┌──────────────────────┐
                         │       User           │
                         │   Regular Screen     │
                         └──────────┬───────────┘
                                    │
                                    ▼
                         ┌──────────────────────┐
                         │      Unity 3D        │
                         │   Virtual Meeting    │
                         │      Environment     │
                         └───────┬──────┬───────┘
                                 │      │
                 ┌───────────────┘      └───────────────┐
                 ▼                                      ▼
        ┌─────────────────┐                    ┌─────────────────┐
        │   Photon PUN    │                    │  Interactive    │
        │ Real-Time Sync  │                    │    Features     │
        └────────┬────────┘                    │ Avatar/Whiteboard│
                 │                             └────────┬────────┘
                 ▼                                      │
        ┌─────────────────┐                             │
        │ Multiplayer     │                             │
        │ Participants    │                             │
        └─────────────────┘                             │
                                                        ▼
                                              ┌─────────────────┐
                                              │  Gemini AI      │
                                              │    Chatbot      │
                                              └─────────────────┘

                         Azure / PlayFab
                    Backend & cloud integration
```

------------------------------------------------------------------------

## User Experience

A typical interaction flow is:

``` text
Launch Application
       │
       ▼
Enter Virtual Environment
       │
       ▼
Join / Interact with Participants
       │
       ├──────────────► Move and interact as an avatar
       │
       ├──────────────► Collaborate using the whiteboard
       │
       └──────────────► Interact with the AI chatbot
       │
       ▼
Collaborative Virtual Meeting / Learning Session
```

------------------------------------------------------------------------

## What the Project Demonstrates

Aura Expansion brings together several areas of interactive application
development in a single Unity project:

-   Real-time multiplayer networking
-   3D avatar-based interaction
-   Interactive virtual environments
-   AI API integration
-   Collaborative learning tools
-   Cloud/backend integration
-   User interaction design for remote collaboration

The project documentation identifies the intended benefits as a more
engaging learning environment, improved collaboration, interactive
teaching tools, and scalability across educational and training
contexts. fileciteturn0file0L59-L64

------------------------------------------------------------------------

## Target Use Cases

### Virtual Classrooms

Teachers and students can meet inside a shared environment and use the
whiteboard for explanations and collaborative activities.

### Remote Team Meetings

Teams can use a shared virtual environment to make remote meetings more
interactive.

### Training & Workshops

The platform can be adapted for organizations that need an interactive
space for remote training sessions.

### Collaborative Learning

The combination of avatars, shared interaction, and AI assistance
provides a foundation for more interactive online learning experiences.

------------------------------------------------------------------------

## Project Structure

The repository follows a Unity project structure. The main development
content is organized around Unity's standard project directories:

``` text
Aura-Expansion/
├── Assets/
│   └── Game assets, scenes, scripts and project content
├── Packages/
│   └── Unity package configuration
├── ProjectSettings/
│   └── Unity project configuration
├── Windows/
│   └── Windows-related project/build content
└── README.md
```

Generated Unity files such as the local `Library` cache are
environment-dependent and may not be required to open or develop the
project from a clean clone.

------------------------------------------------------------------------

## Getting Started

### Prerequisites

Install:

-   Unity with a version compatible with the project's `ProjectSettings`
-   Git
-   A working internet connection for multiplayer and API-backed
    functionality

The project uses Photon PUN for multiplayer, Gemini for the chatbot, and
PlayFab/Azure integration as documented in the project materials.
fileciteturn0file0L50-L54

### Clone the Repository

``` bash
git clone https://github.com/sathwikchava/Aura-Expansion.git
cd Aura-Expansion
```

### Open in Unity

1.  Open **Unity Hub**.
2.  Select **Add / Open Project**.
3.  Select the cloned `Aura-Expansion` directory.
4.  Allow Unity to import and generate its local project cache.
5.  Open the project's main scene from the `Assets` directory.
6.  Configure any required Photon, Gemini, PlayFab, or Azure credentials
    before running networked/API-dependent features.

> API keys and service credentials should be supplied through your local
> configuration. Do not commit secrets to the repository.

------------------------------------------------------------------------

## Configuration

The project integrates external services, so a local setup may require
credentials for:

-   Photon PUN
-   Google Gemini API
-   PlayFab
-   Azure services used by the project

Keep credentials outside the repository whenever possible.

For example:

``` text
API_KEY=your_key_here
```

Do not replace the example with a real secret inside `README.md`, source
code, or committed configuration files.

------------------------------------------------------------------------

## Future Direction

The project documentation identifies several possible extensions:

-   More realistic and customizable avatars
-   Improved avatar animations and expressions
-   AI-powered tutors
-   Multiple virtual classroom environments
-   Mobile support
-   VR support

These directions are intended to extend the platform toward broader
virtual learning and collaboration scenarios.
fileciteturn0file0L76-L81

------------------------------------------------------------------------

## Project Vision

Aura Expansion is built around a simple idea:

> **Make remote interaction feel more like sharing the same space.**

By combining a 3D environment with real-time multiplayer interaction,
collaborative tools, and AI assistance, the project provides a
foundation for virtual meetings and learning experiences that go beyond
a conventional video-call interface.

------------------------------------------------------------------------

## Team

Developed by:

-   **A. Ganesh**
-   **M. V. Mourya Goud**
-   **C. Johith**
-   **Ch. Sathwik**

The team members are listed in the project presentation.
fileciteturn0file0L103-L108

------------------------------------------------------------------------

## Contributing

Contributions, ideas, and improvements are welcome.

A typical contribution workflow:

``` bash
git checkout -b feature/your-feature
git add .
git commit -m "Add your feature"
git push origin feature/your-feature
```

Then open a pull request describing the change.

------------------------------------------------------------------------

## License

No license is currently specified for this repository.

If you intend to allow reuse, modification, or distribution of the
project, add an appropriate `LICENSE` file to the repository.

------------------------------------------------------------------------

## Acknowledgements

Built with:

-   Unity
-   Photon PUN
-   Google Gemini API
-   PlayFab
-   Azure

The project's documented technology stack and feature set are based on
the supplied project presentation. fileciteturn0file0L41-L54
