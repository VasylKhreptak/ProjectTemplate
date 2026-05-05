# 🧩 Project Template

A reusable Unity project template designed to provide a solid architectural foundation for new projects.

This template focuses on **structure, scalability, and clean separation of concerns**, allowing fast project setup with minimal boilerplate.

---

## 🚀 Overview

The template is built around a **state-driven architecture** combined with dependency injection and scoped contexts.

It helps organize project flow, scene logic, and UI in a consistent and extendable way.

---

## 🧠 Core Concepts

### 🔄 State Machines
The project flow is controlled through layered state machines:

- **ProjectStateMachine** — global application flow
- **MainMenuStateMachine** — main menu logic
- **GameplayStateMachine** — in-game logic

Each state machine handles:
- Context-specific initialization
- Loading logic for its scope

---

### 🧱 Scoped Architecture
- **Project Scope** — global systems and services
- **Scene Scopes** — isolated dependencies per scene

This separation ensures:
- Clear lifetime management
- Better modularity
- Easier testing and extension

---

### 🪟 UI Window System
- Centralized window management
- Handles opening/closing UI screens
- Designed to be easily extendable

---

### 🔌 Dependency Injection
- Uses **VContainer** as the DI framework
- Promotes:
    - Loose coupling
    - Better testability
    - Clean dependency management
