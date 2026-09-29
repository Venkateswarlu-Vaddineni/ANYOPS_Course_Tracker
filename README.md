# Course Tracker Pro · Ultra Modern Local Learning Hub 🚀

An ultra-modern, privacy-first, local course tracker and learning studio designed for power learners. Built for local offline video courses, tutorials, and certifications with **zero build step**, instant launch, and rich analytics.

![UI Design](https://img.shields.io/badge/UI-Ultra%20Modern%20Glassmorphism-00f2fe?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-100%25%20Local%20%7C%20Zero%20Cloud-10b981?style=for-the-badge)
![Storage](https://img.shields.io/badge/Storage-IndexedDB%20%2B%20LocalStorage-6366f1?style=for-the-badge)

---

## ✨ Features & Architecture

### 1. 🎨 Ultra-Modern Glassmorphic UI
- **Cyber-Slate Aesthetics**: Deep `#07090e` dark theme with ambient luminous glows, frosted glass cards (`backdrop-filter: blur(20px)`), and subtle neon gradients.
- **Typography**: Paired Google Fonts: **Plus Jakarta Sans** for modern headings and UI text, **JetBrains Mono** for metrics, timestamps, and percentages.
- **Collapsible Sidebar Navigation**: Instant tab switching between **Curriculum**, **Analytics**, **Second Brain Notes**, **Focus Studio (Pomodoro)**, **Study Targets**, and **Course Library**.
- **Responsive & Crisp**: 100% scalable vector SVG icons throughout, with support for mobile and desktop screens.

### 2. ⚡ Fast Command Palette (`Ctrl + K` / `⌘ + K`)
- Press `Ctrl+K` from anywhere in the app to summon the instant spotlight palette.
- Fuzzy search across all **lessons**, **courses**, **notes**, and **system actions** (e.g., *"Start 25m Focus"*, *"Download Backup"*, *"Rescan Folder"*, *"View Heatmap"*).
- Full keyboard navigation with `↑`, `↓`, `Enter`, and `Esc`.

### 3. ⏱️ Focus Studio (Integrated Pomodoro Timer)
- Built-in study timer supporting **25m Focus**, **50m Deep Work**, **5m Short Break**, and **15m Long Break**.
- **Live Circular Progress Ring** with active time ticker in the top navigation bar.
- **Web Audio API Synthesizer**: Gentle, pure two-tone audio chimes on session completion (100% zero external audio files needed).
- Automatically records flow-state study minutes into your course's daily study velocity!

### 4. 🧠 Second Brain & Timestamped Notes Hub
- Take timestamped notes, code snippets, and takeaways during video playback.
- Centralized **Notes Hub** displaying all notes across all courses, searchable by keyword or course.
- **1-Click Timestamp Seek**: Click any timestamp badge (`▶ 12:45`) to immediately open the lesson at that exact second.
- **Export to Markdown (`.md`)**: Download your notes in clean GitHub-flavored markdown to bring directly into **Obsidian**, **Notion**, or **Logseq**.

### 5. 🎬 Cinema Video Player 2.0
- Dark cinema overlay with responsive aspect ratio.
- **In-Player Playlist Drawer**: Switch between sections and lessons without leaving the player.
- **In-Player Notes Drawer**: Add notes stamped to the exact current playback second.
- **Smart Auto-Advance**: 5-second countdown banner on lesson completion with `[Play Now]` and `[Cancel]` controls.
- **Speed Controls**: `0.5x` to `2.5x` with fine steps and memory.
- **Native PiP & Fullscreen**: Multi-task with picture-in-picture mode.

### 6. 📊 Analytics, Velocity & 70-Day Heatmap
- **Trend Curve**: Interactive high-DPI canvas cubic spline with area gradient and exact time hover tooltips.
- **70-Day Activity Heatmap**: GitHub-style continuous calendar tracking daily study habits.
- **Daily Progress Inspector**: Pick any date to inspect exactly which lessons were finished and total hours watched.
- **Pace & Graduation Forecaster**: Calibrates your 14-day average study pace and calculates your estimated course graduation date.

### 7. 💾 Zero-Data-Loss Safety Engine
- **Local File System Access API**: Connect directly to local video folders (`.mp4`, `.mkv`, `.webm`, `.avi`, `.mov`, `.mp3`).
- **1-Click Session Reconnect**: Seamlessly re-authorizes folder permissions when reopening your browser.
- **Automated Rolling Snapshots**: IndexedDB rolling backups store your last 10 session states.
- **JSON Backup Export & Drag-and-Drop Import**: Full backup export and instant drag-and-drop restore.

---

## 🚀 Getting Started

### Option 1: Direct Double Click (Fastest)
Simply double-click `The_Course_Tracker.html` or `index.html` to open it in **Google Chrome**, **Microsoft Edge**, **Brave**, or **Opera**.

### Option 2: Local Static Server (Recommended)
You can serve the directory using any static web server:

```bash
# Using Node.js npx serve
npx.cmd serve .

# Or using Python
python -m http.server 8080
```
Then navigate to `http://localhost:8080/The_Course_Tracker.html`.

---

## ⌨️ Keyboard Shortcuts

| Shortcut | Action |
| :--- | :--- |
| `Ctrl + K` / `Cmd + K` | Open Spotlight Command Palette |
| `Space` | Play / Pause video |
| `←` / `→` | Seek 5 seconds backward / forward |
| `J` / `L` | Seek 10 seconds backward / forward |
| `↑` / `↓` | Volume up / down |
| `M` | Mute / Unmute audio |
| `N` | Play next lesson |
| `P` | Picture-in-Picture mode |
| `F` | Toggle Fullscreen |
| `<` / `>` | Decrease / Increase playback speed |
| `C` | Mark active lesson as completed |
| `Esc` | Close video player, modals, or command palette |
| `?` | Open keyboard shortcuts reference |

---

## 📂 Data Storage & Privacy

All your progress, course names, and timestamps remain **100% on your machine**:
- **`localStorage`**: Keeps real-time app settings, completed statuses, and goals.
- **`IndexedDB`**: Stores persistent File System Directory Handles and automated rolling snapshots.
- **`Course_Tracker_Backup.json`**: An exportable JSON file that can be committed to your private GitHub repo for cloud sync across machines.
