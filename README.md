# GymStats

A dark-mode training dashboard for tracking workouts, recovery, quality of effort, and long-term progress. It helps you answer the questions that matter most in the gym:

- Am I recovered enough to train?
- How fatigued am I right now?
- Which muscles are under the most stress this week?
- Is my training progressing in a healthy way?

## Features

- Training overview with readiness and fatigue scoring
- Recovery snapshot by muscle group
- Weekly training-load body map for front and back views
- Progressive overload tracking for exercises over time
- Support for GymKing-style exports, CSV, pasted raw data, and remote URLs
- Minimal dark UI focused on performance and recovery, not vanity metrics

## Project structure

- `index.html` — dashboard UI and logic
- `style.css` — custom styling and body-map visuals
- `data/` — example or local data files

## Running locally

Because the app loads data from local files and remote feeds, it is best served through a small local web server:

```bash
cd gymstats
python3 -m http.server 8000
```

Then open:

```text
http://localhost:8000/index.html
```

## Supported inputs

The app can load:

- `.gkdb` exports
- `.csv` files
- `.json` files
- raw pasted workout data
- remote URLs that return usable workout payloads

## Typical workflow

1. Upload or paste your workout export.
2. Use the date filters to focus on a training block.
3. Review readiness, fatigue, and recovery insights.
4. Check the weekly training-load map to see which muscle groups are taking the most work.
5. Open the Progress section to review progressive overload trends.

## Notes

This project is intentionally opinionated: it emphasizes training quality, recovery, and weekly stress management over equipment splits and generic gym stats.

## License

This project is for personal use and local analytics. See the repository license if one is included in your environment.
