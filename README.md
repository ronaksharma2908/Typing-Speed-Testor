# ⌨️ Typing Speed Tester

<div align="center">

### 🚀 A fast, interactive, and responsive typing test application

Measure your **typing speed, accuracy, errors, and overall performance** in real time.

<br>

[![Project](https://img.shields.io/badge/Project-Typing%20Speed%20Tester-blue?style=for-the-badge)](https://github.com/your-username/typing-speed-tester)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge\&logo=html5\&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge\&logo=css3\&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge\&logo=javascript\&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)
[![Responsive](https://img.shields.io/badge/Responsive-Yes-success?style=for-the-badge)](#-responsive-design)

<br><br>

### 🌐 [**Live Demo →**](https://your-live-demo-url.com)

</div>

---

## 📑 Table of Contents

* [✨ Features](#-features)
* [📸 Preview](#-preview)
* [🎮 How It Works](#-how-it-works)
* [🧮 WPM Calculation](#-wpm-calculation)
* [🎯 Accuracy Calculation](#-accuracy-calculation)
* [🏆 Best Score](#-best-score)
* [🛠️ Technologies](#️-technologies)
* [📂 Project Structure](#-project-structure)
* [⚙️ Installation](#️-installation)
* [🎮 How to Use](#-how-to-use)
* [⌨️ Keyboard Shortcuts](#️-keyboard-shortcuts)
* [📊 Performance Metrics](#-performance-metrics)
* [📱 Responsive Design](#-responsive-design)
* [🔒 Privacy](#-privacy)
* [⚡ Performance](#-performance)
* [🧪 Testing](#-testing)
* [🚀 Roadmap](#-roadmap)
* [🏗️ Future Architecture](#️-future-architecture)
* [🤝 Contributing](#-contributing)
* [🐛 Bug Reports](#-bug-reports)
* [💡 Feature Requests](#-feature-requests)
* [📜 License](#-license)
* [👨‍💻 Author](#-author)

---

# ✨ Features

## ⏱️ Typing Test

* ⏱️ 60-second typing challenge
* 🔄 Random typing passages
* ⏰ Real-time countdown timer
* 🛑 Automatic test completion
* 🔁 Restart functionality

## 📊 Performance Tracking

* ⚡ Real-time **Words Per Minute (WPM)**
* 🎯 Real-time **accuracy**
* ❌ Typing error tracking
* 📝 Characters typed
* ✅ Correct characters
* 🏆 Personal best WPM

## 🎨 Interactive Interface

* 🟢 Correct character highlighting
* 🔴 Incorrect character highlighting
* 🔵 Current character indicator
* 📱 Responsive layout
* ✨ Clean user interface
* ⚡ Instant feedback

## 💾 Persistent Score

Your highest WPM score is automatically saved using browser:

```javascript
localStorage
```

Your best score remains available even after refreshing the browser.

---

# 📸 Preview

<div align="center">

<img src="./assets/preview.png" alt="Typing Speed Tester Preview" width="850">

</div>

> 💡 Add your application screenshot to `assets/preview.png`.

### 🎥 Demo GIF

<div align="center">

<img src="./assets/demo.gif" alt="Typing Speed Tester Demo" width="850">

</div>

---

# 🎮 How It Works

The application follows this workflow:

```text
                 ┌──────────────────┐
                 │    START TEST    │
                 └────────┬─────────┘
                          │
                          ▼
                ┌──────────────────┐
                │ Random Passage   │
                │     Loaded       │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ User Starts      │
                │    Typing        │
                └────────┬─────────┘
                         │
                         ▼
             ┌─────────────────────────┐
             │    REAL-TIME TRACKING   │
             │                         │
             │ ⚡ WPM                  │
             │ 🎯 Accuracy             │
             │ ❌ Errors               │
             │ 📝 Characters           │
             └───────────┬─────────────┘
                         │
                         ▼
                ┌──────────────────┐
                │   Timer = 0      │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ Final Results    │
                └────────┬─────────┘
                         │
                         ▼
                ┌──────────────────┐
                │ Best Score Saved │
                └──────────────────┘
```

---

# 🧮 WPM Calculation

The application uses the standard typing-speed formula:

```text
WPM = Correct Characters / 5 / Time in Minutes
```

### Example

Suppose a user types:

```text
250 correct characters
```

in:

```text
1 minute
```

Then:

```text
WPM = 250 / 5 / 1
    = 50 WPM
```

Therefore:

```text
Typing Speed = 50 WPM
```

---

# 🎯 Accuracy Calculation

Accuracy is calculated using:

```text
Accuracy =
Correct Characters / Total Typed Characters × 100
```

### Example

If the user types:

```text
100 characters
```

and:

```text
95 characters are correct
```

Then:

```text
Accuracy = 95 / 100 × 100
         = 95%
```

---

# ❌ Error Tracking

Every incorrectly typed character is tracked and visually highlighted.

### Example

```text
Target:
Hello World

Typed:
Hella World
```

The incorrect character is immediately detected.

### Visual Indicators

| Indicator | Meaning             |
| --------- | ------------------- |
| 🟢 Green  | Correct character   |
| 🔴 Red    | Incorrect character |
| 🔵 Blue   | Current character   |

---

# 🏆 Best Score

The application stores the user's highest WPM using browser Local Storage.

### Save Score

```javascript
localStorage.setItem("bestWPM", bestWPM);
```

### Retrieve Score

```javascript
const bestWPM = localStorage.getItem("bestWPM");
```

### Benefits

* 🚫 No database required
* 🚫 No login required
* 💾 Persists after refresh
* ⚡ Lightweight
* 🔒 Stored locally
* 🌐 Works completely on the client side

---

# 🛠️ Technologies

| Technology       | Purpose                       |
| ---------------- | ----------------------------- |
| HTML5            | Application structure         |
| CSS3             | Styling and responsive design |
| JavaScript       | Application logic             |
| DOM Manipulation | Dynamic UI updates            |
| Local Storage    | Persistent score storage      |

---

# 📂 Project Structure

```text
typing-speed-tester/
│
├── index.html
├── style.css
├── script.js
├── README.md
│
└── assets/
    ├── preview.png
    └── demo.gif
```

### `index.html`

Responsible for the application's structure and UI elements.

### `style.css`

Responsible for:

* Layout
* Colors
* Typography
* Animations
* Responsive design

### `script.js`

Responsible for:

* Timer
* Typing engine
* WPM calculation
* Accuracy calculation
* Error detection
* Passage generation
* Local Storage
* Restart functionality

---

# ⚙️ Installation

## 1. Clone the repository

```bash
git clone https://github.com/your-username/typing-speed-tester.git
```

## 2. Navigate into the project

```bash
cd typing-speed-tester
```

## 3. Open the application

Open:

```text
index.html
```

in your browser.

### Recommended Development Setup

Use **VS Code + Live Server** for easier development.

---

# 🎮 How to Use

1. Open the application.
2. Click **Start Test**.
3. A random passage will appear.
4. Start typing.
5. Type as quickly and accurately as possible.
6. Monitor your WPM and accuracy.
7. Continue until the timer reaches zero.
8. View your final performance.
9. Your best WPM is automatically saved.

---

# ⌨️ Keyboard Shortcuts

| Shortcut | Action               |
| -------- | -------------------- |
| `Enter`  | Start / Restart Test |
| `Esc`    | Reset Test           |
| `Tab`    | Navigate controls    |

> 💡 More keyboard shortcuts can be added in future versions.

---

# 📊 Performance Metrics

The application tracks:

```text
┌──────────────────────────┐
│       PERFORMANCE        │
├──────────────────────────┤
│ ⚡ WPM                   │
│ 🎯 Accuracy              │
│ ❌ Errors                │
│ 📝 Characters Typed      │
│ ✅ Correct Characters    │
│ 🏆 Best Score            │
└──────────────────────────┘
```

These metrics provide a complete overview of typing performance.

---

# 📱 Responsive Design

The application is designed for:

```text
💻 Desktop
💻 Laptop
📱 Tablet
📱 Mobile
```

Responsive CSS ensures the interface adapts to different screen sizes.

---

# 🔒 Privacy

This application:

* Does not require an account.
* Does not require a backend.
* Does not send typing data to a server.
* Processes typing data locally.
* Stores the best WPM locally in the browser.

Your typing activity remains on your device.

---

# ⚡ Performance

The project is intentionally lightweight.

### Current Architecture

* Vanilla JavaScript
* No frontend framework
* No backend
* No database
* Minimal dependencies
* Client-side calculations
* Local Storage

This keeps the application:

```text
⚡ Fast
🪶 Lightweight
🔒 Private
🌐 Easy to deploy
```

---

# 🧪 Testing

Before releasing a new version, verify:

* [ ] Timer starts correctly
* [ ] Timer stops at zero
* [ ] WPM updates correctly
* [ ] Accuracy updates correctly
* [ ] Errors are counted correctly
* [ ] Correct characters are highlighted
* [ ] Incorrect characters are highlighted
* [ ] Current character is visible
* [ ] Random passages load correctly
* [ ] Restart functionality works
* [ ] Best WPM is saved
* [ ] Best WPM persists after refresh
* [ ] Mobile layout works
* [ ] Desktop layout works
* [ ] No console errors occur

---

# 🚀 Roadmap

## 🎯 Version 1.1

* [ ] Multiple test durations
* [ ] Difficulty levels
* [ ] More typing passages
* [ ] Custom passages
* [ ] Dark mode
* [ ] Sound effects
* [ ] Improved animations

## 📊 Version 1.2

* [ ] Typing history
* [ ] WPM history
* [ ] Accuracy history
* [ ] Performance graphs
* [ ] Statistics dashboard
* [ ] Average WPM
* [ ] Best accuracy
* [ ] Personal records

## 🏆 Version 2.0

* [ ] Global leaderboard
* [ ] User profiles
* [ ] Authentication
* [ ] Cloud score synchronization
* [ ] Multiplayer typing races
* [ ] Real-time competitions
* [ ] Friends and challenges

## 🤖 Advanced AI Features

* [ ] AI-generated typing passages
* [ ] AI typing-performance analysis
* [ ] Personalized difficulty
* [ ] Weak-key detection
* [ ] Typing improvement recommendations
* [ ] AI-generated practice sessions
* [ ] WPM prediction
* [ ] Personalized learning paths

---

# 🏗️ Future Architecture

As the application grows, the architecture can evolve from a simple frontend project into a complete typing platform.

```text
                    ┌─────────────────────┐
                    │   TYPING TESTER     │
                    └──────────┬──────────┘
                               │
              ┌────────────────┼────────────────┐
              │                │                │
              ▼                ▼                ▼
       ┌─────────────┐  ┌─────────────┐  ┌─────────────┐
       │Typing Engine│  │  Analytics  │  │    UI/UX    │
       └──────┬──────┘  └──────┬──────┘  └─────────────┘
              │                │
       ┌──────┼──────┐         │
       ▼      ▼      ▼         ▼
      WPM  Accuracy Errors   History
                              │
                              ▼
                            Graphs
                              │
                              ▼
                       ┌──────────────┐
                       │Local Storage │
                       └──────┬───────┘
                              │
                              ▼
                       Future Backend
                              │
                   ┌──────────┴──────────┐
                   ▼                     ▼
               Database              User Auth
                   │                     │
                   └──────────┬──────────┘
                              ▼
                         Leaderboard
```

---

# 🌟 Why This Project?

Typing speed is an important productivity skill for:

* 👨‍💻 Programmers
* 🎓 Students
* 🧑‍💼 Professionals
* ✍️ Writers
* ⌨️ Developers
* 🏢 Office workers

The goal of this project is to provide a simple, fast, and accessible platform for measuring and improving typing performance.

---

# 🤝 Contributing

Contributions are welcome!

### 1. Fork the repository

### 2. Create a feature branch

```bash
git checkout -b feature/new-feature
```

### 3. Make your changes

Implement your feature or fix.

### 4. Commit your changes

```bash
git add .
git commit -m "Add new feature"
```

### 5. Push your branch

```bash
git push origin feature/new-feature
```

### 6. Create a Pull Request

Explain:

* What you changed
* Why you changed it
* How it improves the project
* Any screenshots or demos

---

# 🐛 Bug Reports

Found a bug?

Please open an issue and include:

```text
Bug Description:
Steps to Reproduce:
Expected Behaviour:
Actual Behaviour:
Browser:
Operating System:
Screenshots:
```

This makes it easier to investigate and fix problems.

---

# 💡 Feature Requests

Have an idea?

Create an issue and describe:

```text
Feature:
Why is it useful?
How should it work?
Possible implementation:
```

Innovative ideas are always welcome!

---

# 📈 Future Vision

The long-term goal is to transform this project into a complete typing-performance and learning platform.

```text
        PRACTICE
           ↓
        MEASURE
           ↓
        ANALYZE
           ↓
   IDENTIFY WEAKNESSES
           ↓
 PERSONALIZED PRACTICE
           ↓
         IMPROVE
           ↓
        COMPETE
```

The ultimate goal is not just to measure typing speed, but to help users **understand their weaknesses and improve consistently.**

---

# 📜 License

This project is licensed under the **MIT License**.

You are free to:

* ✅ Use the project
* ✅ Modify the project
* ✅ Distribute the project
* ✅ Use it for educational purposes

See the [LICENSE](LICENSE) file for details.

---

# 👨‍💻 Author

<div align="center">

## Ronak Sharma

🎓 **B.Tech CSE | AI & ML**

💻 **Aspiring Software Developer & AI/ML Engineer**

<br>

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge\&logo=github\&logoColor=white)](https://github.com/your-username)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge\&logo=linkedin\&logoColor=white)](https://linkedin.com/in/your-username)

</div>

---

# ⭐ Support

If you found this project useful:

⭐ **Star the repository**

🍴 **Fork the repository**

🐛 **Report bugs**

💡 **Suggest features**

🤝 **Contribute**

Your support motivates further development!

---

<div align="center">

## ⌨️ Happy Typing! 🚀

**Built with ❤️ using HTML, CSS & JavaScript**

⭐ If you enjoyed this project, consider giving it a star!

</div>
