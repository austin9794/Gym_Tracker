# GymTrack — Smart Gym Progress Dashboard

A local Flask web app to track your workouts and body stats, backed by SQLite.

## Setup

1. **Open in VS Code**
   ```
   code gym_tracker/
   ```

2. **Install dependencies** (in your terminal or VS Code terminal)
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the app**
   ```bash
   python app.py
   ```

4. **Open in your browser**
   ```
   http://localhost:5000
   ```

The SQLite database (`gym_tracker.db`) is created automatically on first run, pre-loaded with 2 weeks of example data so the dashboard looks good straight away.

## Features

- **Dashboard** — weekly session count, current weight, body fat %, live charts, PRs, recent workout log
- **Log Workout** — exercise name, sets, reps, weight, notes
- **Log Stats** — body weight, body fat %, notes
- **Charts** — body weight trend line + per-exercise strength bar chart (switchable)

## File Structure

```
gym_tracker/
├── app.py              # Flask routes + SQLite logic
├── requirements.txt
├── gym_tracker.db      # Auto-created on first run
└── templates/
    ├── base.html       # Nav, styles, shared layout
    ├── dashboard.html  # Main dashboard + charts
    ├── log_workout.html
    └── log_stats.html
```

