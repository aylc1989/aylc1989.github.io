# 🚀 REACH — Workout Tracker PWA

Reach your goals. A gamified workout tracking app built as a Progressive Web App (PWA) that installs directly on your Samsung Galaxy S24.

## Features

### Quick Logging
- **3×2 category grid** on the home screen for instant logging
- **6 categories**: Cardio, Upper Body, Lower Body, Yoga & Stretch, Wellness, Other
- **Multi-category sessions** — select multiple categories (e.g. Cardio + Upper Body) and time splits evenly between them
- **Duration presets**: 15, 30, 45, 60, 90, 120 minutes

### Calendar
- **Heatmap view** — days with workouts are highlighted, brighter = more workouts
- **Tap a date** to see that day's activities, then use the **"+ Log Activity"** button to log directly for that date
- **Export to .ics** — download all workouts as a calendar file for Google Calendar

### Stats Dashboard
- **Weekly / Monthly / All-time** toggle
- Workout count, total minutes, current streak, best streak, avg per week, total XP
- **Category breakdown** with visual bars
- **Focus balance** — Upper Body vs Lower Body, Cardio vs Wellness

### Gamification
- **XP system** — earn 10–60 XP per workout based on duration
- **Streak bonuses** — extra XP for maintaining 3/7/14/30+ day streaks
- **15 levels**: Beginner → Starter → Mover → Active → Committed → Dedicated → Disciplined → Warrior → Powerhouse → Champion → Elite → Legend → Mythic → Transcended → Immortal
- **30 achievements** across categories:
  - Workout milestones (1, 5, 10, 25, 50, 100, 250)
  - Streak achievements (3, 7, 14, 21, 30, 60, 100 days)
  - XP milestones (500, 1000, 2500, 5000)
  - Duration feats (Hour Power, Marathon Session, Time Lord, Time Master)
  - Variety (Well Rounded, Combo Master, Perfect Balance)
  - Special (Weekend Warrior, Early Bird, Night Owl, New Year Grind, Consistency King)
- **Milestone track** — visual progress toward 1/10/25/50/100/250/500 workouts
- **Weekly goals** — 4 rotating goals with progress bars on the home screen
- **This Week tracker** — visual dots showing which days you've been active
- **Level-up & achievement toasts** — pop-up notifications when you earn rewards

### Data
- All data stored locally on your device (localStorage) — no server, no account
- **Export/import** all data as JSON for backup
- **Auto-migration** from previous GRIND app data
- **Reset** option to clear all data

---

## 🚀 How to Get This on Your Galaxy S24

### Option A: GitHub Pages (Recommended — Free, 5 minutes)

1. **Create a GitHub account** (if you don't have one): https://github.com/signup

2. **Create a new repository**:
   - Go to https://github.com/new
   - Name it: `reach-tracker` (or whatever you like)
   - Set it to **Public**
   - Click **Create repository**

3. **Upload the files**:
   - Click **"uploading an existing file"** link
   - Drag & drop ALL 5 files:
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

5. **Your app is live at**: `https://YOUR-USERNAME.github.io/reach-tracker/`

6. **Install on your Galaxy S24**:
   - Open Chrome on your phone
   - Navigate to your GitHub Pages URL
   - Tap the **three-dot menu** (⋮) in Chrome
   - Tap **"Install app"** or **"Add to Home screen"**
   - The app icon will appear on your home screen!

### Updating the App

When you upload new files to GitHub:
- Your existing workout data is **safe** — it's stored in your browser's localStorage, separate from the app files
- Just replace the files in your repo and wait for Pages to rebuild
- Reload the app on your phone — the service worker will pick up the new version

### If "Install App" Doesn't Appear

1. Tap **⋮ → Settings → Site settings** in Chrome
2. Find your github.io site → **Clear & reset**
3. Revisit the URL — the install option should reappear
4. Alternatively, **⋮ → Add to Home screen** always works

### Option B: Local Testing

```bash
cd reach-tracker
python3 -m http.server 8000
```
Open `http://localhost:8000` in your browser.

---

## 📱 Using the App

### Logging a Workout
1. Tap any category card on the home screen, OR tap the **orange + button**
2. Select **one or more categories** — if you pick multiple, time splits evenly
3. Choose a duration, optionally add a name and notes
4. Hit **SAVE ACTIVITY** — earn XP!

### Calendar View
- Tap **Calendar** in the bottom nav
- Tap a day to see its activities
- Tap the highlighted date's **"+ Log Activity"** button to log for that specific date
- Use **Export to Calendar** to download an .ics file for Google Calendar

### Stats
- Tap **Stats** to see breakdowns by week/month/all-time
- Track upper vs. lower body balance and cardio vs. wellness focus

### Achievements & Levels
- Tap **Badges** to see your level, milestone track, and all 30 achievements
- Earn XP from every workout, with streak bonuses for consistency

---

## 📂 Files

| File | Purpose |
|------|---------|
| `index.html` | The complete app (HTML + CSS + JavaScript) |
| `manifest.json` | PWA configuration (icon, name, display mode) |
| `sw.js` | Service worker for offline caching |
| `icon-192.png` | App icon (192×192) |
| `icon-512.png` | App icon (512×512) |
