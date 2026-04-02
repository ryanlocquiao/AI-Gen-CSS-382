# ModKit — AI-Powered Car Mod Finder

ModKit is a web app that generates personalized car modification suggestions based on your vehicle's make, model, and year. Enter your car, pick a category, and get AI-curated mod recommendations complete with descriptions, cost estimates, difficulty ratings, and step-by-step installation guides.

---

## Features

- **AI-generated mod suggestions** tailored to your specific car
- **Category filtering** — Performance, Suspension, Exhaust, Intake, Brakes, Exterior, Interior
- **Difficulty ratings** — Easy, Medium, or Hard per mod
- **Cost estimates** for each modification
- **Step-by-step install guides** with tools required
- **Safety warnings** specific to your car and mod combination

---

## Tech Stack

- **Frontend** — Vanilla HTML, CSS, JavaScript
- **Backend** — Vercel Serverless Functions
- **AI** — Groq API (`llama-3.3-70b-versatile`)

---

## Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) installed
- A free [Groq API key](https://console.groq.com)
- A [Vercel](https://vercel.com) account

### Project Structure

```
modkit/
├── index.html      # Frontend UI
├── api/
│   └── chat.js     # Serverless function (Groq API proxy)
└── README.md
```

### Local Development

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/modkit.git
   cd modkit
   ```

2. Install the Vercel CLI:
   ```bash
   npm install -g vercel
   ```

3. Create a `.env` file in the root:
   ```
   GROQ_API_KEY=gsk_your_key_here
   ```

4. Run locally:
   ```bash
   vercel dev
   ```

5. Open [http://localhost:3000](http://localhost:3000)

### Deploying to Vercel

1. Push your project to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → **Add New Project** → import your repo
3. Under **Settings → Environment Variables**, add:
   ```
   GROQ_API_KEY = gsk_your_key_here
   ```
4. Hit **Deploy** — Vercel handles the rest

Any future `git push` to `main` will automatically redeploy.

---

## Usage

1. Enter your car's **Make**, **Model**, and **Year**
2. Optionally select a mod **category** (defaults to All)
3. Click **Find Mods**
4. Click any mod card to expand the full installation guide

---

## Notes

- AI results are generated dynamically and may vary between searches
- Always verify part compatibility with your specific vehicle before purchasing
- Difficulty ratings are general estimates — your experience may vary

---

### Netid
jlocqu16

### Name
Ryan Locquiao

### GitHub Repository
https://github.com/ryanlocquiao/AI-Gen-CSS-382

### Deployed Site
https://ai-gen-css-382.vercel.app/

### Idea
Make a website that allows you to input your car's make, model, and year and it will find and suggest mods for your car and explain to you how to install them.