# Cortex => (Gemini UI)

A modern **AI assistant interface replica** built using React that mimics the design and user experience of Gemini. This project demonstrates how to build a **production-style frontend UI** for AI-based applications using component-based architecture and state-driven rendering.

---

## Overview =>

** Cortex ** is a React-based frontend application that focuses on replicating the interface of modern AI assistants.

It leverages :-

* **React Functional Components** for modular UI development
* **useState Hook** for dynamic UI behavior (sidebar toggle)
* **Custom CSS Styling** for clean and responsive design
* **Asset Management System** for handling icons and UI elements

It solves a key frontend challenge :-

> *Designing scalable, clean, and responsive UI similar to real-world AI products*

By structuring the UI into reusable components, the project becomes **maintainable, extensible, and production-ready (frontend level)**.

---

## Features =>

* 1.Gemini-inspired clean UI interface
* 2.Interactive sidebar with expand/collapse functionality
* 3.Predefined prompt suggestion cards
* 4.Structured chat input section with icons
* 5.Component-based architecture
* 6.Responsive and user-friendly layout
* 7.Conditional rendering using React state

---

## Project Architecture =>

```
User Interaction (UI Click / Input)
        ↓
React Components (Main + Sidebar)
        ↓
State Management (useState)
        ↓
 ┌───────────────────────────────┐
 │ Sidebar Toggle (extended)     │
 │ Conditional Rendering         │
 └───────────────┬───────────────┘
                 ↓
        UI Update (Re-render)
                 ↓
        Display Updated Layout
```

---

## Tech Stack =>

| Technology | Purpose                 |
| ---------- | ----------------------- |
| React.js   | Frontend framework      |
| JavaScript | Logic and interactivity |
| CSS3       | Styling and layout      |

---

## Installation & Setup =>

```bash
# Clone the repository
git clone https://github.com/Akshay-Deshmane/cortex-ui.git

# Navigate to project directory
cd cortex-ui

# Install dependencies
npm install

# Run the project
npm run dev
```

---

## WorkFlow Of Cortex =>

### 1.User Interaction :-

User interacts with UI elements:

```
- Click menu icon
- Enter prompt
- Select suggestion cards
```

---

### 2.State Management :-

React manages UI behavior:

```js
const [extended, setExtended] = useState(false);
```

* Controls sidebar expansion
* Drives conditional rendering

---

### 3.Conditional Rendering :-

UI dynamically updates based on state:

```js
{extended ? <p>New Chat</p> : null}
```

---

### 4.UI Rendering :-

* Components re-render automatically
* Sidebar expands/collapses
* UI updates instantly

---

## Key Engineering Decisions =>

### 1.Component-Based Architecture :-

* Separation of UI into `Main` and `Sidebar`
* Improves readability and scalability

---

### 2.State-Driven UI :-

* Used `useState` for dynamic behavior
* Enables real-time UI updates

---

### 3.Conditional Rendering :-

* Prevents unnecessary DOM elements
* Keeps UI lightweight and optimized

---

### 4.Asset Centralization :-

* Icons managed via a single `assets` file
* Improves maintainability

---

## Project Structure =>

```
src/
├── components/
│   ├── Main/
│   │   ├── Main.jsx
│   │   ├── Main.css
│   │
│   ├── Sidebar/
│   │   ├── Sidebar.jsx
│   │   ├── Sidebar.css
│
├── assets/
│   ├── icons/
│   └── images/
│
├── App.jsx
├── index.js
└── README.md
```

---

## Example Usage =>

```
User opens application
→ Sidebar collapsed by default

User clicks menu icon
→ Sidebar expands

User views suggestions
→ Selects prompt ideas (static UI)

User enters input
→ Ready for future AI integration
```

---

## Limitations Of Cortex =>

* UI-only (no AI functionality yet)
* No backend or API integration
* Static prompt system
* No chat history or message rendering

---

## Future Enhancements / Future Scope =>

* 1.AI integration (OpenAI / Gemini API)
* 2.Dynamic chat system with message rendering
* 3.Chat history storage
* 4.Dark mode support
* 5.Authentication system
* 6.Backend integration (Node.js / Firebase)
* 7.Real-time streaming responses

---
