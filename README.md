 ⚙️ Background Task API Demo

This project demonstrates how to use the **Background Tasks API** (via `requestIdleCallback()`) to schedule low-priority operations during browser idle time without blocking the main thread. It ensures a smooth and responsive user experience by offloading non-critical tasks like logging, analytics, and deferred processing.

---

## 🧠 What is the Background Tasks API?

The **Background Tasks API** (powered by `window.requestIdleCallback()`) enables developers to queue low-priority work that executes when the browser is idle. It helps keep the event loop responsive and avoids performance hiccups caused by unnecessary DOM or JS operations during critical render or input events.

---

## 🚀 Features

- 📦 FIFO task queue with idle-time execution
- 🧠 Smart scheduling using `requestIdleCallback()` and `requestAnimationFrame()`
- 📊 Progress bar and live log view
- ⏳ Timeout fallback to ensure execution even under high load
- 🧼 Avoids unnecessary DOM reflows or blocking interactions

---

## 📁 Project Structure

/background-task-api-demo
│
├── index.html # HTML UI for progress and log
├── style.css # Clean, responsive styles
└── script.js # Task queue logic using requestIdleCallback



---

## 🖥️ Demo

> Open `index.html` in a browser that supports `requestIdleCallback()`.

---

## 💡 How It Works

1. User clicks "Start" to enqueue multiple simulated background tasks.
2. Tasks are run one by one when the browser is idle or after a timeout.
3. DOM updates (progress/logging) are deferred to `requestAnimationFrame()` to avoid layout shifts.
4. The UI shows which task is currently running and outputs messages to the log.

---

## 🛠️ Tech Stack

- HTML5
- CSS3 (Responsive Design)
- JavaScript (Vanilla)
- `requestIdleCallback()` API
- `requestAnimationFrame()` for DOM-safe updates
