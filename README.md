# 10x-cards

[![Version](https://img.shields.io/badge/version-0.0.1-blue)](#)
[![License: MIT](https://img.shields.io/badge/license-MIT-yellow.svg)](LICENSE)

## Table of Contents

1. [Project Description](#project-description)  
2. [Tech Stack](#tech-stack)  
3. [Getting Started](#getting-started)  
4. [Available Scripts](#available-scripts)  
5. [Project Scope](#project-scope)  
6. [Project Status](#project-status)  
7. [License](#license)  

---

## Project Description

**10x-cards** is a web application that empowers learners to generate and manage
spaced-repetition flashcards in seconds. By leveraging large language models via
Openrouter.ai, users can paste any text excerpt and receive AI-suggested
question-and-answer pairs. They can then accept, edit, or reject each card
before saving to their personal collection.

- Eliminates manual effort in creating high-quality flashcards  
- Supports manual creation, editing, and deletion of cards  
- Secure user authentication and GDPR-compliant data handling  

---

## Tech Stack

### Frontend
- **Astro** v5 – content-focused framework with minimal JavaScript  
- **React** v19 – for dynamic, interactive components  
- **TypeScript** v5 – static typing and enhanced IDE support  
- **Tailwind CSS** v4 – utility-first styling  
- **Shadcn/ui** – accessible React component library  

### Backend
- **Supabase** – PostgreSQL database, authentication, and BaaS SDK  

### AI
- **Openrouter.ai** – multi-model LLM access with financial controls  

### CI/CD & Hosting
- **GitHub Actions** – CI/CD pipelines  
- **DigitalOcean** (Docker) – container-based deployment  

---

## Getting Started

### Prerequisites

- **Node.js** v22.14.0 (managed via [`.nvmrc`](.nvmrc))  
- **npm** (bundled with Node.js)

### Configuration

Create a `.env` file in the project root with:

```bash
SUPABASE_URL=your_supabase_url
SUPABASE_ANON_KEY=your_supabase_anon_key
OPENROUTER_API_KEY=your_openrouter_api_key
```

### Installation

```bash
git clone https://github.com/<your-org>/10x-cards.git
cd 10x-cards

# Use correct Node version
nvm use

# Install dependencies
npm install
```

### Development

```bash
npm run dev
```

Open `http://localhost:3000` in your browser.

### Build & Preview

```bash
npm run build
npm run preview
```

---

## Available Scripts

From the project root:

```bash
npm run dev         # Start Astro dev server
npm run build       # Build for production
npm run preview     # Preview production build
npm run astro       # Run any Astro CLI command
npm run lint        # Lint .astro, .ts, .tsx files
npm run lint:fix    # Auto-fix lint issues
npm run format      # Format all files with Prettier
```

---

## Project Scope

### In-Scope (MVP)

- Automatic flashcard generation via LLM API (paste text → suggestions → accept/edit/reject)  
- Manual flashcard creation, editing, and deletion  
- User registration, login, and account deletion  
- Integration with an open-source spaced-repetition algorithm  
- Secure, scalable storage of users and flashcards  
- Basic AI generation metrics (accepted vs. rejected cards)  
- GDPR compliance (data access and deletion on request)  

### Out-of-Scope (for MVP)

- Custom spaced-repetition algorithm  
- Gamification features (points, badges)  
- Native mobile applications  
- Bulk document import (PDF, DOCX)  
- Public API endpoints for third-party apps  
- Flashcard sharing between users  
- Advanced notification or reminder system  
- Full-text keyword search and filtering  

---

## Project Status

🚧 **Active development (MVP stage)**  
Core features are defined and under implementation. Contributions and feedback are welcome!

---

## License

This project is licensed under the **MIT License**.  
See the [LICENSE](LICENSE) file for details. 