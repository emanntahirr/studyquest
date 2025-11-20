# StudyQuest — AI-Powered Learning Assistant

StudyQuest is a full-stack intelligent learning assistant designed to help students understand, plan, and revise their modules efficiently using AI-driven difficulty analysis, visual dashboards, automated flashcards, and adaptive retrospective timetables.

---

## MVP

### 1. Module & Topic Input
- Add modules and their topics  
- Optional confidence & notes fields  

---

### 2. AI Topic Ranking
AI ranks topics based on:
- Conceptual difficulty  
- Estimated time demand 

Output is fully structured JSON.

---

### 3. Visual Dashboard
Interactive charts:
- Difficulty bar graph
- Time-demand heatmap
- Dependency tree
- Radar graph of difficulty vs confidence

---

### 4. AI Flashcard Generator
Automatically creates:
- Q/A cards  
- Multiple choice  
- Code snippet cards  

---

### 5. Retrospective Timetable Generator
Builds a dynamic exam timetable based on:
- Difficulty  
- Time available  
- Exam date  
- Missed sessions (auto-shift)

---

## Tech Stack

### Backend
- Node.js + Express  
- AI API Integration  
- PostgreSQL (via Prisma ORM)

### Frontend
- React  
- TailwindCSS  
- Recharts / D3  
- Zustand or Redux

---

## Documentation
- `docs/MVP.md` — full feature outline  
- `diagrams/uml.md` — system UML diagram  
- `prompts/` — AI prompt templates for ranking, flashcards & timetables  

---
