# Aura Expansion

```{=html}
<p align="center">
```
`<strong>`{=html}Aura Expansion`</strong>`{=html}`<br>`{=html}
`<em>`{=html}An immersive 3D virtual meeting and learning environment
built with Unity.`</em>`{=html}
```{=html}
</p>
```
```{=html}
<p align="center">
```
`<a href="#features">`{=html}Features`</a>`{=html} •
`<a href="#technology-stack">`{=html}Technology`</a>`{=html} •
`<a href="#getting-started">`{=html}Getting Started`</a>`{=html} •
`<a href="#architecture">`{=html}Architecture`</a>`{=html} •
`<a href="#team">`{=html}Team`</a>`{=html} •
`<a href="#license">`{=html}License`</a>`{=html}
```{=html}
</p>
```
```{=html}
<p align="center">
```
`<img src="https://img.shields.io/badge/Unity-3D-black?logo=unity" alt="Unity">`{=html}
`<img src="https://img.shields.io/badge/C%23-239120?logo=csharp&logoColor=white" alt="C#">`{=html}
`<img src="https://img.shields.io/badge/Photon-PUN-6A1B9A" alt="Photon PUN">`{=html}
`<img src="https://img.shields.io/badge/Google-Gemini%20API-4285F4?logo=google" alt="Gemini API">`{=html}
`<img src="https://img.shields.io/badge/PlayFab-107C10" alt="PlayFab">`{=html}
`<img src="https://img.shields.io/badge/License-MIT-yellow.svg" alt="MIT License">`{=html}
```{=html}
</p>
```

------------------------------------------------------------------------

## Overview

**Aura Expansion** is a Unity-based 3D virtual meeting and learning
platform designed to make remote interaction more natural, interactive,
and engaging.

Instead of limiting participants to a conventional 2D video-call
interface, the project places users inside a shared virtual environment
where they can interact through 3D avatars, collaborate using a virtual
whiteboard, and access an AI-powered chatbot.

The platform is designed around a simple idea:

> **Make remote collaboration feel more like being together in the same
> space.**

The project supports interaction through a regular screen, keeping the
experience accessible without requiring dedicated VR hardware.

------------------------------------------------------------------------

## Why This Project?

Traditional online meetings and remote learning environments can feel
distant. Participants often lose the spatial presence and natural
interaction of a physical room.

Aura Expansion addresses this by combining:

-   A shared 3D environment
-   Real-time avatar interaction
-   Collaborative learning tools
-   AI-assisted interaction
-   Multiplayer networking
-   Cloud/backend integration

The goal is to provide a flexible foundation for **virtual classrooms,
remote meetings, workshops, and collaborative learning environments**.

------------------------------------------------------------------------

## Features

### 3D Avatars

Users are represented by 3D avatars inside the virtual environment,
creating a stronger sense of presence and interaction.

### Real-Time Interaction

The multiplayer layer enables users to share the same virtual
environment and interact with other participants in real time.

### Virtual Whiteboard

A shared whiteboard provides a space for explanations, teaching,
presentations, and collaborative discussion.

### AI Chatbot

The platform integrates the **Google Gemini API** to provide an
AI-powered conversational assistant inside the environment.

### Screen-Based Accessibility

The project is designed to work through a conventional desktop screen,
allowing users to experience the environment without requiring a VR
headset.

### Cloud Integration

The project includes **PlayFab/Azure integration** as part of its
backend and cloud-service architecture.

------------------------------------------------------------------------

## Demo

### Project Walkthrough

> **Demo video:** Add the public demo URL here.

For the best repository presentation, upload the walkthrough to YouTube
or another stable video host and replace the placeholder above.

You can also add a thumbnail here:

``` markdown
[![Aura Expansion Demo](https://img.youtube.com/vi/YOUR_VIDEO_ID/maxresdefault.jpg)](https://www.youtube.com/watch?v=YOUR_VIDEO_ID)
```

------------------------------------------------------------------------

## Screenshots

Add project screenshots to a directory such as `docs/images/` and place
them here.

``` markdown
![Virtual Environment](docs/images/virtual-environment.png)
![3D Avatars](docs/images/avatars.png)
![Virtual Whiteboard](docs/images/whiteboard.png)
![AI Chatbot](docs/images/ai-chatbot.png)
```

A README with real screenshots and a short demo video gives visitors an
immediate understanding of the project before they inspect the Unity
source.

------------------------------------------------------------------------

## Technology Stack

  -----------------------------------------------------------------------
  Technology                          Role
  ----------------------------------- -----------------------------------
  **Unity 3D**                        3D environment, scenes, interaction
                                      and application development

  **C#**                              Application and gameplay logic

  **Photon PUN**                      Real-time multiplayer networking

  **Google Gemini API**               AI chatbot / conversational
                                      assistance

  **PlayFab**                         Backend and cloud integration

  **Azure**                           Cloud-service integration
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Architecture

``` text
                         ┌─────────────────────┐
                         │        User         │
                         │   Desktop / Screen  │
                         └──────────┬──────────┘
                                    │
                                    ▼
                         ┌─────────────────────┐
                         │      Unity 3D       │
                         │ Virtual Environment │
                         └─────────┬───────────┘
                                   │
              ┌────────────────────┼────────────────────┐
              │                    │                    │
              ▼                    ▼                    ▼
      ┌───────────────┐    ┌───────────────┐    ┌───────────────┐
      │  3D Avatars   │    │ Virtual Board │    │  AI Chatbot   │
      │  Interaction  │    │ Collaboration │    │ Gemini API    │
      └───────┬───────┘    └───────────────┘    └───────┬───────┘
              │                                          │
              ▼                                          │
      ┌───────────────┐                                  │
      │  Photon PUN   │                                  │
      │ Real-Time Net │                                  │
      └───────┬───────┘                                  │
              │                                          │
              ▼                                          ▼
      ┌───────────────┐                         ┌────────────────┐
      │ Other Users   │                         │ AI Response    │
      │ / Participants│                         │   to Client    │
      └───────────────┘                         └────────────────┘

                         ┌─────────────────────┐
                         │  PlayFab / Azure    │
                         │ Backend Integration │
                         └─────────────────────┘
```

------------------------------------------------------------------------

## User Flow

``` text
Launch Application
        │
        ▼
Enter Virtual Environment
        │
        ▼
Join / Connect to Session
        │
        ▼
      ┌─┴───────────────────────────┐
      │                             │
      ▼                             ▼
Interact with Avatars        Use Virtual Whiteboard
      │                             │
      └──────────────┬──────────────┘
                     │
                     ▼
              Use AI Chatbot
                     │
                     ▼
        Collaborative Meeting /
           Learning Session
```

------------------------------------------------------------------------

## Getting Started

### Prerequisites

Before opening the project, install:

-   [Unity Hub](https://unity.com/download)
-   A Unity Editor version compatible with the project's
    `ProjectSettings/ProjectVersion.txt`
-   Git
-   A stable internet connection for networked and API-backed features

The project uses Unity, C#, Photon PUN, Gemini API, and PlayFab/Azure
services.

### Clone the Repository

``` bash
git clone https://github.com/sathwikchava/Aura-Expansion.git
cd Aura-Expansion
```

### Open the Project

1.  Open **Unity Hub**.
2.  Select **Add project from disk**.
3.  Select the cloned `Aura-Expansion` directory.
4.  Open the project using the Unity version specified by the project
    settings.
5.  Allow Unity to import packages and generate its local cache.
6.  Open the relevant scene from the `Assets` directory.
7.  Configure the external services before testing networked or
    AI-dependent features.

> Unity may take some time to import the project the first time it is
> opened.

------------------------------------------------------------------------

## External Service Configuration

Aura Expansion depends on external services for parts of its
functionality.

Depending on the feature being tested, configure:

-   **Photon PUN** for multiplayer networking
-   **Google Gemini API** for the AI chatbot
-   **PlayFab** for backend functionality
-   **Azure** services used by the project

### API Keys

Never commit real API keys or credentials to GitHub.

Use a local configuration mechanism appropriate for your Unity setup and
keep secret values outside version control.

Example:

``` text
GEMINI_API_KEY=your_api_key_here
PHOTON_APP_ID=your_app_id_here
```

The values above are placeholders only.

------------------------------------------------------------------------

## Project Structure

A simplified Unity project layout:

``` text
Aura-Expansion/
│
├── Assets/
│   ├── Scenes/
│   ├── Scripts/
│   ├── Prefabs/
│   ├── Materials/
│   └── ...
│
├── Packages/
│   └── packages-lock.json
│
├── ProjectSettings/
│   ├── ProjectSettings.asset
│   └── ProjectVersion.txt
│
├── Windows/
│
├── README.md
└── LICENSE
```

The exact contents of `Assets/` depend on the current project version.

### About Unity's `Library` Folder

Unity generates the `Library/` directory locally as an imported asset
and package cache. It can be very large and contains editor-generated
data.

For normal Unity source repositories, the project should generally be
reproducible from the tracked project files and package configuration
without relying on a machine-specific `Library/` cache.

------------------------------------------------------------------------

## Use Cases

### Virtual Classrooms

Teachers and students can interact in a shared 3D environment while
using collaborative teaching tools.

### Remote Meetings

Teams can use avatars and a shared virtual space to make remote meetings
more interactive.

### Workshops and Training

The environment can be adapted for remote training sessions and
demonstrations.

### Collaborative Learning

The combination of a shared environment, interactive tools, and AI
assistance provides a foundation for collaborative digital learning.

------------------------------------------------------------------------

## Project Goals

Aura Expansion focuses on four core areas:

  Goal                Implementation
  ------------------- --------------------------------------------
  **Presence**        3D avatars and shared virtual environments
  **Interaction**     Real-time multiplayer communication
  **Collaboration**   Virtual whiteboard and shared space
  **AI Assistance**   Gemini-powered chatbot

------------------------------------------------------------------------

## Future Enhancements

The project can be extended in several directions:

-   More realistic and customizable avatars
-   Improved avatar animations and expressions
-   AI-powered tutors
-   Additional virtual classroom environments
-   Mobile support
-   VR support
-   Additional collaborative tools
-   Expanded cloud/backend capabilities

These extensions can build on the existing Unity, networking, AI, and
cloud architecture.

------------------------------------------------------------------------

## Development Notes

When contributing to the project:

1.  Create a feature branch.
2.  Make focused changes.
3.  Test the Unity project locally.
4.  Avoid committing generated files and secrets.
5.  Write a clear commit message.
6.  Open a pull request with a description of the change.

Example:

``` bash
git checkout -b feature/new-feature
git add .
git commit -m "Add new feature"
git push origin feature/new-feature
```

------------------------------------------------------------------------

## Team

### Hack Street Boys

-   **A. Ganesh**
-   **M. V. Mourya Goud**
-   **C. Johith**
-   **Ch. Sathwik**

------------------------------------------------------------------------

## Acknowledgements

Built with:

-   [Unity](https://unity.com/)
-   [Photon](https://www.photonengine.com/)
-   [Google Gemini API](https://ai.google.dev/)
-   [PlayFab](https://playfab.com/)
-   [Microsoft Azure](https://azure.microsoft.com/)

------------------------------------------------------------------------

## License

This project is licensed under the **MIT License**.

See [`LICENSE`](LICENSE) for the complete license text.

------------------------------------------------------------------------

```{=html}
<p align="center">
```
`<strong>`{=html}Aura Expansion`</strong>`{=html}`<br>`{=html}
`<em>`{=html}Virtual spaces for more connected
collaboration.`</em>`{=html}
```{=html}
</p>
```
