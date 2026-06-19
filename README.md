# ⚡️ NeonDraw

A lightweight, zero-install browser overlay for video calls. Draw, diagram, and annotate directly on your screen while you talk using your mouse, voice commands, or **hand tracking**.

No more switching tabs to Excalidraw or fumbling with clunky built-in Zoom whiteboards. 

## ✨ Features

* **👋 Hand Tracking (MediaPipe):** Draw in thin air! Pinch your thumb and index finger together to draw, and release to stop. Includes EMA stabilization for buttery-smooth ink.
* **🎙️ Voice Commands:** Use your voice to spawn shapes or control the canvas. Just say *"circle"*, *"arrow"*, *"clear"*, or *"undo"*.
* **🖌️ Smooth Vector Ink:** Automatically converts jagged cursor/finger movements into smooth quadratic Bezier curves.
* **⚡️ Zero-Latency Overlay:** Runs entirely locally in your browser. No backend, no accounts, no lag.
* **💾 Export:** Download your annotated screen as a transparent PNG.
* **🎨 Customizable:** Quick color swatches, adjustable stroke weights, and draggable shapes.

## 🚀 How to Use It

Because this is a web app, there's nothing to install. 

1. Clone this repository or download the `index.html` file.
2. Open `index.html` in **Google Chrome** or **Microsoft Edge** (required for Voice Recognition).
3. Click **"Start Camera"** and grant camera/microphone permissions.

### Using it in Video Calls (Zoom, Google Meet, Teams)

**Option A: The Easy Way (Screen Share)**
Simply share your entire screen or the specific browser tab where NeonDraw is running.

**Option B: The Pro Way (OBS Virtual Camera)**
If you want to appear *behind* your drawings as your actual webcam feed:
1. Download and install [OBS Studio](https://obsproject.com/).
2. Add a **Window Capture** source and select your browser running NeonDraw.
3. Click **"Start Virtual Camera"** in OBS.
4. In Zoom/Meet, change your Camera source to "OBS Virtual Camera".

## 🎮 Controls

### Hand Tracking
* **Hover:** Open hand (shows cyan cursor).
* **Draw:** Pinch index finger and thumb together (shows green cursor).

### Voice Commands
Click the "Voice Commands" button and say any of the following:
* `"circle"` / `"round"` — Spawns a circle.
* `"square"` / `"rectangle"` — Spawns a rectangle.
* `"arrow"` — Spawns a directional arrow.
* `"triangle"` — Spawns a triangle.
* `"color"` — Cycles through the quick color palette.
* `"bigger"` / `"smaller"` — Adjusts the stroke weight.
* `"undo"` — Removes the last stroke or shape.
* `"clear"` / `"wipe"` — Erases the entire canvas.

### Keyboard Shortcuts
* `Delete` or `Backspace` — Remove the currently selected shape.
* `Ctrl/Cmd + Z` — Undo last action.
* `Esc` — Deselect current shape.
* `Double Click` — Deselect current shape.

## 🛠️ Built With

* **HTML5 Canvas** - Core drawing engine.
* **Tailwind CSS** - UI and styling.
* **Google MediaPipe** - Real-time hand landmark detection.
* **Web Speech API** - Native browser voice recognition.
* **FontAwesome** - Icons.

## 🛣️ Roadmap

- [ ] Chrome Extension to inject the overlay directly into Google Meet tabs.
- [ ] Two-handed gestures (e.g., pinch with both hands to scale shapes).
- [ ] Custom background blur/removal.

## 📄 License
MIT License - feel free to use, modify, and distribute this prototype!
