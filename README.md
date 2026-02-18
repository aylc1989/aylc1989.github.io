# 🔥 GRIND — Workout Tracker PWA

A gamified workout tracking app built as a Progressive Web App (PWA) that installs directly on your Samsung Galaxy S24.

## Features
- **Quick Log** — Tap a category to instantly log workouts
- **6 Categories** — Cardio, Upper Body, Lower Body, Yoga & Stretch, Wellness, Other
- **Calendar Heatmap** — See your active days at a glance
- **Stats Dashboard** — Category breakdowns, upper/lower body balance, cardio vs. wellness
- **Gamification** — XP system, 10 levels, 15 achievements, streak tracking
- **Calendar Sync** — Export all workouts as .ics file for Google Calendar
- **Offline Support** — Works without internet after first load
- **Data Backup** — Export/import all data as JSON

---

## 🚀 How to Get This on Your Galaxy S24

### Option A: GitHub Pages (Recommended — Free, 5 minutes)

1. **Create a GitHub account** (if you don't have one): https://github.com/signup

2. **Create a new repository**:
   - Go to https://github.com/new
   - Name it: `grind-tracker`
   - Set it to **Public**
   - Click **Create repository**

3. **Upload the files**:
   - Click **"uploading an existing file"** link
   - Drag & drop ALL files from the `workout-tracker` folder:
     - `index.html`
     - `manifest.json`
     - `sw.js`
     - `icon-192.png`
     - `icon-512.png`
   - Click **Commit changes**

4. **Enable GitHub Pages**:
   - Go to **Settings** → **Pages** (in left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Branch: **main**, folder: **/ (root)**
   - Click **Save**
   - Wait 1-2 minutes for deployment

5. **Your app is live at**: `https://YOUR-USERNAME.github.io/grind-tracker/`

6. **Install on your Galaxy S24**:
   - Open Chrome on your phone
   - Navigate to your GitHub Pages URL
   - Tap the **three-dot menu** (⋮) in Chrome
   - Tap **"Add to Home screen"** or **"Install app"**
   - The app icon will appear on your home screen!

### Option B: Local Testing (Immediate)

1. Put all files in a folder
2. Use any local server to test. For example with Python:
   ```bash
   cd workout-tracker
   python3 -m http.server 8000
   ```
3. Open `http://localhost:8000` in your browser

---

## 📱 Using the App

### Logging a Workout
- Tap any category card on the home screen, OR
- Tap the **orange + button** in the bottom navigation
- Select category, duration, add optional name/notes
- Hit **SAVE ACTIVITY** — earn XP!

### Viewing Your Calendar
- Tap **Calendar** in the bottom nav
- Days with workouts are highlighted (brighter = more workouts)
- Tap any day to see details
- Use **Export to Calendar** to sync with Google Calendar

### Checking Stats
- Tap **Stats** to see breakdowns by week/month/all-time
- Track your upper vs. lower body balance
- Monitor cardio vs. wellness focus

### Achievements & Levels
- Tap **Badges** to see your level progress and achievements
- Earn XP from every logged workout
- Unlock 15 achievements from streaks, milestones, and variety

### Calendar Sync
- Go to Calendar tab → **Export to Calendar (.ics)**
- Open the downloaded file — it imports directly into Google Calendar
- Each workout appears as an all-day event with details

---

## 📂 Files

| File | Purpose |
|------|---------|
| `index.html` | The complete app (HTML + CSS + JavaScript) |
| `manifest.json` | PWA configuration (icon, name, display mode) |
| `sw.js` | Service worker for offline caching |
| `icon-192.png` | App icon (192×192) |
| `icon-512.png` | App icon (512×512) |

All data is stored locally on your device using localStorage. No server, no account needed.
# workouttracker
