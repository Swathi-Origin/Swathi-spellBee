# Word Adventure - Kids Spelling Game

A fun spelling game for children ages 6-7, built with **NestJS** (backend) and **React** (frontend).

## Features

- **4 game sections** with 20 questions each:
  1. Fill in the missing letters
  2. Choose the correct spelling
  3. Unscramble the word
  4. Write the word correctly

- **5 levels** by word length (3-4, 4-5, 5-6, 6-7, 7-8 letters)

- Kid-friendly UI with large buttons and encouraging feedback

- Local progress saving with star ratings (stored in browser localStorage)

- Level unlock when all 4 sections score 15+ in a level

## Getting Started

### Prerequisites

- Node.js 18+

### Run the Backend (NestJS)

```bash
cd backend
npm install
npm run start:dev
```

The API runs at `http://localhost:3000`

### Run the Frontend (React)

```bash
cd frontend
npm install
npm run dev
```

The app opens at `http://localhost:5173`

## API Endpoints

| Endpoint | Description |
|----------|-------------|
| `GET /api/config` | Game configuration (levels, sections, thresholds) |
| `GET /api/levels` | List of word levels |
| `GET /api/sections` | List of game sections |
| `GET /api/questions/:level/:section` | 20 questions for a level/section |

## Star Ratings

- 3 stars: 90%+ correct (18-20)
- 2 stars: 75%+ correct (15-17)
- 1 star: 50%+ correct (10-14)
- 0 stars: below 50%

## Tech Stack

- **Backend:** NestJS, TypeScript
- **Frontend:** React, Vite, TypeScript, React Router
