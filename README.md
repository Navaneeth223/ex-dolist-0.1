# 🚀 Enhanced Task Tracker

A sleek, performance-oriented task management tool featuring a built-in **Daily Streak Engine** and local data persistence. This version is optimized for responsiveness and provides instant visual feedback for user accomplishments.

---

## ✨ Features

* **Daily Streak Engine:** Tracks consecutive days of productivity. 
    * Automatically detects "yesterday" to increment streaks.
    * Resets to 1 if a day is missed.
* **Animated Goal Feedback:** A custom CSS-driven "Success Checkmark" triggers on completion to provide dopamine-driven positive reinforcement.
* **Data Persistence:** Uses `localStorage` to ensure your tasks and streak count remain intact even after closing the browser.
* **Responsive UX:** * **Desktop:** Side-by-side task management and actions.
    * **Mobile:** Stacked layout with touch-friendly buttons and increased hit zones.
* **Clean Interface:** Utilizes the **Inter** typeface for maximum legibility and a professional aesthetic.

---

## 🏗️ Technical Implementation

### 1. Streak Logic Flow
The tracker implements a "Lookback" validation method. When a task is marked as complete, the app checks the timestamp of the last recorded completion.



### 2. Animation Pipeline
The success animation is achieved through a multi-stage CSS animation sequence:
* **`fadeInScale`**: Handles the entry transition from $0\%$ to $100\%$ size.
* **`pulse`**: Adds a subtle bounce effect once the checkmark is fully visible.

### 3. DOM Component Breakdown
| Component | Function |
| :--- | :--- |
| **`addTask()`** | Validates input string and pushes to the state array. |
| **`toggleTaskCompletion()`** | Manages completion status and triggers the streak update. |
| **`renderTasks()`** | An efficient list-rebuilding function that ensures UI stays synced with data. |

---

## 🚀 How to Launch

1.  **Save the Code:** Copy the source into a file named `tracker.html`.
2.  **Open in Browser:** Double-click the file to open it in Chrome, Firefox, or Safari.
3.  **Start Tracking:**
    * Enter a task in the top input.
    * Click "Complete" to start your 1-day streak!

---

## 🛠️ Tech Stack

* **HTML5:** Structured document outline.
* **CSS3:** Flexbox layouts, media queries, and `@keyframes` animations.
* **JavaScript (ES6+):** Logical state handling and browser storage APIs.
* **Fonts:** Inter via Google Fonts API.

---

## 🚧 Roadmap
- [ ] **Multi-Select:** Delete or complete multiple tasks at once.
- [ ] **Task Prioritization:** Color-coded urgency levels (High, Medium, Low).
- [ ] **Dark Mode:** Re-integration of the dark-themed UI toggle.

---
*Stay consistent, stay productive.*
