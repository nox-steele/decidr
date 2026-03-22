# Decidr

A simple app to track decisions, record the reasoning, and review them later to learn from outcomes.

## Problem

People make decisions daily but forget why. Can't learn from past choices.

## Solution

Decidr helps you:
- Log decisions with context and expected outcomes
- Set review dates (1 week, 1 month, 3 months)
- Review later and record what actually happened
- See patterns in your decision-making

## Tech Stack

- Single HTML file with embedded CSS/JS
- LocalStorage for persistence
- No backend required

## Getting Started

1. Open `index.html` in any browser
2. Start logging decisions
3. Review when prompted

## Features

- Add decisions with context and expected outcomes
- Automatic review reminders
- Track expected vs actual outcomes
- History of all decisions

## Demo

Open `index.html` directly in browser — no server needed.

## Rollback

If something breaks, rollback to the last working version:

```bash
cd project-folder
git log --oneline          # find the last good commit
git reset --hard <commit>  # reset to that commit
git push --force           # push the rollback
```

Example (rollback to commit `abc1234`):
```bash
git reset --hard abc1234
git push --force
```

## License

MIT
