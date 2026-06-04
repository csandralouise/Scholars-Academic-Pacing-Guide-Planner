# 📖 Scholar's Planner — Academic Pacing Guide

A single-file, offline-ready academic planning tool built for students who need structure, focus, and flexibility. No installations, no accounts, no subscriptions — just open the file in any modern browser and start planning.

---

## Features

### 🏠 Dashboard
The home screen gives you an at-a-glance view of your academic workload:

- **Stats row** — Live counts of Total Tasks, Completed, In Progress, and Overdue items, pulled dynamically from your curriculum map
- **Course cards** — Each course you've added shows its task count and a visual progress bar
- **Upcoming Deadlines** — The next 6 due dates sorted chronologically, with overdue items highlighted
- **Weekly Study Hours** — A visual bar chart showing your target study distribution across the week (Sunday-heavy, Saturday off)
- **Workload alerts** — Automatic warnings when 3 or more tasks are due within 7 days
- **Quick Add Task** — Add a task to any course directly from the dashboard without switching tabs

### 📅 Pacing Guide Generator
Distribute your study workload intelligently across the semester:

- Select a course, set semester start and end dates, and enter your topics
- Assign a difficulty level (Easy / Medium / Hard) to each topic
- Flag topics as exam or milestone markers
- Set weekly study hours and how many days per week you want to study
- The generator produces a full week-by-week schedule, weighted heavier on Sundays and lighter on weekdays
- Saturdays are always protected as rest days
- Saved pacing schedules persist across sessions

### 🗓️ Calendar
Visualize your schedule in Month or Week view:

- Click any weekday or Sunday to add a calendar event
- Events are color-coded by course
- Sundays are highlighted as primary study days
- Saturdays are locked as rest days
- Navigate forward/backward by month or return to today
- Weekly Reset button clears past events while preserving your curriculum and pacing data

### 📋 Curriculum Map
A structured table for tracking all your coursework:

- Columns for Course, Topic/Module, Learning Outcome, Assessment type, Due Date, and Status
- Inline editing — click any cell to update it
- Status options: Not Started, In Progress, Completed
- Filter by course using the filter bar
- Rows feed directly into the Dashboard's upcoming deadlines and stats

### ⏱️ Study Session (Pomodoro Timer)
A full-featured focus timer to power your study blocks:

- Configurable focus duration (default 50 min), short break, long break, and sessions before long break
- Visual countdown with an animated progress bar
- Session log with timestamps for every focus block and break
- Live stats: sessions completed, breaks taken, total focus minutes
- Select which course you're studying — displayed on the timer face
- Study Routine Recommendations with five built-in schedules:
  - 💼 Working Student (recommended) — weekday evenings + heavy Sundays
  - 🏫 After School — evenings after class
  - 🌙 Night Study — late-night deep work blocks
  - 📚 Weekend Study — balanced weekend sessions with social time
  - 🌅 Morning Study — early-morning full-day study sessions
- Applying a routine auto-sets the focus and break durations in the timer

---

## Getting Started

1. Open `New_Scholars_Pacing_Guide_Updated.html` in any modern browser (Chrome, Firefox, Safari, Edge)
2. The app loads with a clean slate — no sample data
3. Go to **Dashboard → Manage Courses** and add your courses with a course code and name
4. Head to **Curriculum Map** to add your topics, assessments, and due dates
5. Use the **Pacing Guide** to generate a week-by-week study schedule for each course
6. Check the **Calendar** to see everything laid out visually
7. Use the **Study Session** tab to run focused Pomodoro blocks when it's time to work

---

## Data & Privacy

All data is saved automatically to your browser's `localStorage` under keys prefixed `sp_`. Nothing is sent to any server — your academic data stays entirely on your device.

Since data lives in localStorage, it is tied to the browser and device you use. If you clear browser data or use a different browser, your data will not carry over. For backup, export or print your curriculum map and pacing guide using the Print/Export button (🖨️) in the header.

---

## Keyboard-Friendly Controls

| Action | How |
|---|---|
| Switch tabs | Click the tab buttons in the nav bar |
| Add a topic row | Click **+ Add Topic** in the Pacing Guide |
| Start/pause timer | Click **▶ Start** or **⏸ Pause** |
| Skip timer phase | Click **⏭ Skip** |
| Toggle dark mode | Click 🌙 / ☀️ in the header |
| Print or export PDF | Click 🖨️ in the header |
| Weekly reset | Click 🔄 in the header |

---

## Design

- **Font:** Inter (Google Fonts), sans-serif — clean and readable for long study sessions
- **Light mode:** Warm parchment tones — easy on the eyes in daylight
- **Dark mode:** Deep teal-tinted charcoal backgrounds with aqua/teal accents and orange-yellow CTA highlights — fresh, modern, and low fatigue for night study
- **Responsive:** Adapts to mobile screens; quote chip hidden on small viewports
- **Print styles:** Non-content elements hidden when printing; pacing guide optimized for landscape export

---

## File Structure

This is a single self-contained HTML file. Everything — HTML, CSS, and JavaScript — lives inside `New_Scholars_Pacing_Guide_Updated.html`. No external dependencies beyond the Inter font loaded from Google Fonts. The app works fully offline once the font has cached.

---

## Customization

The color scheme is defined entirely through CSS custom properties at the top of the `<style>` block. Both light and dark mode palettes can be adjusted there without touching any logic. Course colors (`--c1` through `--c4`) are also CSS variables and can be changed to match your school or personal preference.

---

## Browser Support

Works in any browser released after 2019. Requires JavaScript enabled and localStorage available (not blocked by private/incognito mode restrictions in some browsers).

---

*Scholar's Planner — built for students who take their academics seriously.*
