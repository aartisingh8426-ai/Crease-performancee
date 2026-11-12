# Crease Performance — Cricket Tracker

A mobile-first, offline-capable cricket batting, training and recovery tracker.

## Included
- Home dashboard with readiness estimate, weekly volume, sessions and performance chart
- Batting session logging, editing, deleting, date filters and interactive calendar
- Past-date session entry: open Batting → choose any date → Log
- Recovery check-ins with a transparent readiness estimate
- Workload trends and caution flags for rapid increases / rising fatigue
- Skill ratings and trend summaries
- Weekly report, personal records and data-grounded local Coach insights
- Profile, weekly targets, JSON backup/restore and CSV export
- Local browser storage; no account or cloud service required

## Run
Open `index.html` in a modern browser. For best Android install/offline support, serve this folder over HTTPS (or localhost), open it in Chrome, then use **Add to Home screen / Install app**.

A simple local server:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000` on the same device/network.

## Important limitations
- This package is a working Progressive Web App source, not a compiled Android APK.
- Data is stored locally in the browser on that device. Use Export Backup regularly; clearing browser data can erase records.
- Coach insights are rule-based and use only saved app data. They are not a connected generative AI service.
- Readiness is a simple wellness/training estimate, not a medical assessment or diagnosis.
- Biometric/HRV integrations, coach cloud sync, video biomechanics and verified AI analysis are not included because they require external services or hardware permissions.
