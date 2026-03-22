# Decision Journal - Specification

## Overview
A simple app to track decisions, record the reasoning, and review them later to learn from outcomes.

## Problem
People make decisions daily but forget why. Can't learn from past choices.

## Target Customer
- Product managers, founders, executives
- Self-improvement enthusiasts
- Anyone who wants to make better decisions

## Tech Stack
- Single page HTML/CSS/JS app
- LocalStorage for persistence
- No backend (MVP)

## Data Model
```javascript
{
  id: string,
  title: string,
  context: string,
  expectedOutcome: string,
  decisionDate: ISO timestamp,
  reviewDate: ISO timestamp,
  actualOutcome: string (filled on review),
  tags: string[]
}
```

## User Flows

### 1. Add Decision
- Enter title (required)
- Enter context (what was the situation)
- Enter expected outcome (what do you think will happen)
- Select review period (1 week, 1 month, 3 months)
- Save → stored in LocalStorage

### 2. Review Dashboard
- Show list of decisions awaiting review (past review date)
- Sort by how overdue (most overdue first)
- Show decision + expected outcome
- Allow user to enter actual outcome
- Mark as reviewed → moves to history

### 3. History
- All reviewed decisions
- Show expected vs actual outcome
- Can filter by tags

## UI/UX

### Pages
1. **Home/Dashboard** - Decisions needing review
2. **Add Decision** - Form to add new
3. **History** - Past decisions

### Design
- Clean, minimalist
- Card-based layout
- Clear typography
- Mobile-first

## MVP Milestones

- [ ] Day 1: Project setup, LocalStorage, Add Decision form
- [ ] Day 2: Review dashboard, marking decisions as reviewed
- [ ] Day 3: History view, polish, deploy

## Success Metrics
- Users sign up (or use locally)
- Decisions made
- Reviews completed
