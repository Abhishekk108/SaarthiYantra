# Eligify — Welfare Scheme Discovery Engine

An intelligent welfare scheme recommendation platform that helps persons with disabilities in India discover government schemes they are eligible for through rule-based eligibility matching and AI-powered multilingual explanations.

---

## Overview

Eligify simplifies access to government welfare schemes by matching users with relevant central and state schemes based on their disability profile, income, age, and location. It provides personalized recommendations, AI-generated explanations in multiple languages, downloadable document checklists, and application tracking.

---

## Features

* Rule-based eligibility matching for government welfare schemes
* Central and state scheme recommendations
* AI-generated multilingual scheme explanations using Groq
* Downloadable PDF document checklists
* Application status tracking
* Offline support using Service Workers
* Mobile-friendly user interface

---

## Tech Stack

### Frontend

* React (Vite)
* React Router
* React Context API
* jsPDF
* Service Worker

### Backend

* Node.js
* Express.js

### AI

* Groq SDK

### Storage

* localStorage

---

## Architecture

```
User Profile
      │
      ▼
Eligibility Matching
      │
      ▼
Scheme Filtering & Ranking
      │
      ▼
Groq AI Explanation
      │
      ▼
Multilingual Response
      │
      ▼
Document Checklist
      │
      ▼
Application Tracker
```

---

## Project Structure

```
/
├── src/
│   ├── components/
│   ├── pages/
│   ├── hooks/
│   ├── services/
│   ├── context/
│   ├── utils/
│   └── data/
│
├── server/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   └── data/
│
└── public/
```

---

## Getting Started

### Backend

```bash
cd server
npm install
cp .env.example .env
```

Add your `GROQ_API_KEY` to `.env`

```bash
node index.js
```

Backend runs on:

```
http://localhost:3001
```

### Frontend

```bash
npm install
npm run dev
```

Frontend runs on:

```
http://localhost:5173
```

---

## How It Works

1. User enters disability, age, income, and state.
2. The eligibility engine filters applicable welfare schemes.
3. Matching schemes are ranked using rule-based scoring.
4. Groq generates plain-language multilingual explanations.
5. Users can download required document checklists.
6. Application progress is tracked locally.

---

## Future Improvements

* Database integration for persistent storage
* Voice accessibility support
* DigiLocker integration
* Additional regional language support
* Real-time government scheme updates
* User authentication

---

## License

MIT
