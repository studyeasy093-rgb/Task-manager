# Ledger — Time & Focus

A single-file, offline-first task and focus tracker that turns your day into a
points-based ledger. No build step, no server, no dependencies — open
`task-manager.html` in a browser and it just works. All data is stored
locally in `localStorage`.

## Features

- **Focus timer with a live countdown.** A persistent bar shows the
  running/paused task's remaining time and points on every tab, plus a
  per-task countdown on its row and a full-screen ring timer.
- **Points-based scoring.** Every task earns points based on time logged,
  scaled against a configurable minutes-to-100-points divisor.
- **6:30 AM day boundary.** Your "day" runs from 6:30 AM to 6:29 AM the next
  morning, so late-night sessions still count toward the previous day. Once a
  day ends, its total score is calculated and locked in as final.
- **22 built-in categories** (Daily Routine, Hygiene, Meals, Sleep, Health,
  Exercise, Commute, Work, Deep Work, Learning, Household, Errands, Finance,
  Family, Pets, Social, Digital, Mindfulness, Hobbies, Entertainment, Admin,
  Personal) — fully editable, plus your own custom categories.
- **Quick-pick activity chips.** Each category ships with a curated list of
  common chores and routines (brushing teeth, bathing, breakfast, commute,
  chores, workouts, etc.) — tap one to fill in a task's title and a sensible
  default duration.
- **Calendar, stats, and streaks.** Browse any past day, see a 7-day bar
  chart, current streak, and monthly averages.
- **Import / export.** Back up or move your data as a single JSON file.

## Getting started

1. Download `task-manager.html`.
2. Open it directly in any modern browser (Chrome, Safari, Firefox, Edge).
3. That's it — your data is saved locally in that browser on that device.

There's no build process and no external services; everything runs
client-side in one HTML file.

## Data & privacy

All tasks, settings, and daily score history are stored in your browser's
`localStorage` (keys prefixed `ledger_`). Nothing is sent anywhere. Use
**Settings → Export JSON** to back up your data, and **Import JSON** to
restore it (e.g., on a new device or browser).

## Customizing

- **Categories:** add, remove, or recolor them from Settings.
- **Scoring:** adjust the "points divisor" in Settings to change how many
  minutes of focused time equal 100 points.
- **Quick-pick activities:** edit the `PRESET_ACTIVITIES` object near the top
  of the `<script>` block in `task-manager.html` to add your own presets per
  category.

## License

Feel free to use, modify, and share.
