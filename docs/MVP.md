```markdown
# StudyQuest — MVP Specification

## Objective
Build an AI-powered study assistant that ranks topics, visualises difficulty, generates flashcards, and creates adaptive retrospective timetables based on difficulty + time demand.

---

## Core MVP Features

### 1. Module & Topic Management
- Create modules
- Add topics to each module
- Optional: student confidence input
- Optional: notes field

---

### 2. AI Topic Ranking
Input:
- topics
- optional notes
- optional confidence

AI outputs JSON with:
- difficultyScore (0–100)
- timeDemand (hours)
- importance (0–100)
- dependencies[]

---

### 3. Dashboard Visualisation
Charts (via Recharts or D3.js):
- Difficulty bars
- Time-demand heatmap
- Radar chart
- Dependency graph

---

### 4. Flashcard Generator
AI generates:
- 5 Q/A cards
- 3 MCQs
- 2 code-based cards (if relevant)

All stored per topic.

---

### 5. Retrospective Timetable
Inputs:
- exam date  
- difficulty  
- time demand  
- available hours per day  

Algorithm outputs a dynamic, self-adjusting schedule.

---

## Out of Scope (MVP)
- Authentication
- Spaced repetition engine
- Gamification (XP, levels)
- Lecture note ingestion

---

## Future Expansion
- Practice exam generator
- Study streaks
- Notebook/lecture PDF ingestion
- AI personalisation model
