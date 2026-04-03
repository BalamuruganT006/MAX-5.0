# MAX-5.0

MAX-5.0 is an advanced **AI assistant** designed to interact with your computer via a futuristic UI, a central **AI Orchestrator**, and a modular tool/action system. This repository contains a generated, chapter-based tutorial that explains how the system works end-to-end.

## ✨ Key Features

- **Futuristic UI (Tkinter):** conversation log, command input, mute/state indicator, and animated “face”.
- **Main AI Orchestrator:** interprets user input, selects tools, executes actions, and reports results.
- **Agent Task Management:** handles complex, multi-step goals using planning, execution, retries, and replanning.
- **Toolset / Action System:** a catalog of callable tools (e.g., open apps, web search, weather, file control).
- **Long-Term Memory:** stores and retrieves context across sessions.
- **Configuration Management:** manages API keys and environment configuration.
- **Vision Module:** enables image/screen understanding (where supported).

---

## 🧭 Visual Overview

```mermaid
flowchart TD
    A0["Main AI Orchestrator"]
    A1["Toolset / Action System"]
    A2["Agent Task Management"]
    A3["Long-Term Memory"]
    A4["User Interface (UI)"]
    A5["Configuration Management"]
    A6["Vision Module"]

    A0 -- "Controls and receives from" --> A4
    A0 -- "Executes tools in" --> A1
    A0 -- "Manages" --> A3
    A0 -- "Delegates complex tasks to" --> A2
    A0 -- "Invokes" --> A6

    A1 -- "Retrieves API keys from" --> A5
    A1 -- "Accesses data in" --> A3

    A2 -- "Utilizes tools from" --> A1
    A2 -- "Retrieves API keys from" --> A5

    A3 -- "Uses API keys from" --> A5
    A4 -- "Manages API key setup in" --> A5
    A6 -- "Retrieves API keys from" --> A5
```

---


