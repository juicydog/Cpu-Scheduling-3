# CPU Scheduling Visualizer

An interactive, single-page visualizer for classic CPU scheduling algorithms:

- Round Robin
- Priority Scheduling (Preemptive & Non-Preemptive)
- Shortest Job First (Non-Preemptive)
- Shortest Remaining Time First (SRTF)

Built with plain HTML, CSS, and vanilla JavaScript — no build step, no dependencies.

## Project structure

```
.
├── index.html      # The entire app (markup, styles, and logic)
├── vercel.json      # Vercel static-hosting config
└── README.md
```

## Running locally

No install needed — just open the file in a browser:

```bash
open index.html        # macOS
start index.html        # Windows
xdg-open index.html    # Linux
```

Or serve it locally with any static server, e.g.:

```bash
npx serve .
```

## Deploying to Vercel

### Option A: Vercel CLI

```bash
npm install -g vercel
vercel
```

Follow the prompts (accept the defaults — this is a static site, no build command needed).

### Option B: GitHub + Vercel dashboard

1. Push this folder to a GitHub repository:
   ```bash
   git init
   git add .
   git commit -m "Initial commit: CPU scheduling visualizer"
   git branch -M main
   git remote add origin <your-repo-url>
   git push -u origin main
   ```
2. Go to [vercel.com/new](https://vercel.com/new), import the repository.
3. Framework Preset: **Other** (static site) — Vercel will serve `index.html` automatically.
4. Click **Deploy**.

No environment variables or build steps are required.

## Notes

Internal scheduling functions use themed names (e.g. `ricksRoundRobin`, `buildPortal`, `mortyColor`) — purely cosmetic, doesn't affect behavior.
