# Mori｜專注森林

A responsive Traditional Chinese Pomodoro + study dashboard, built as a dependency-free static web app.

## Run locally
Open `index.html` in a modern browser, or run `python -m http.server 8000` in this folder and visit `http://localhost:8000`.

## Included
- Responsive mobile/desktop dashboard
- Pomodoro, short break and long break timers; configurable durations
- Rain / cafe-style procedural ambient audio using Web Audio API (no audio assets required)
- Local to-do list
- Daily focus statistics and 7-day chart
- Custom companion avatar, name and encouragement style
- Local profile/demo sign-in
- LocalStorage persistence

## Important production notes
The current member sign-in is a local demo profile, not secure authentication. Data is stored in the current browser only and does not sync across devices. For production multi-device accounts, connect Supabase Auth + Postgres (or another backend), migrate tasks/stats/preferences to per-user tables, and protect server-side access with row-level security. The ambient sounds are synthesized approximations; replace them with licensed audio files if you want realistic recordings.

## Deploy
Create a GitHub repository and push this folder. Import the repository in Vercel. Framework preset: **Other**; Build Command: leave blank; Output Directory: `.`. Vercel will serve `index.html` as a static site.
