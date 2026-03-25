# Cover Letter Agent

Score and build cover letters against a 100-point rubric — powered by Claude AI.

**[→ View the site and setup guide](https://YOUR_GITHUB_USERNAME.github.io/cover-letter-agent/)**

---

## What it does

- **Score** — Paste a cover letter and get a visual 100-point evaluation across 10 categories with specific fixes
- **Build** — Upload your resume and a job description, answer a few questions, and get a letter designed to score 90+
- **Score then rebuild** — Score an existing letter, see the deductions, then generate an improved version

## Quick setup (2 minutes)

1. Go to [claude.ai](https://claude.ai) and sign in (free account works)
2. Click **Projects** → **Create Project**
3. Copy the contents of [`agent_instructions.md`](agent_instructions.md) and paste into the **Custom Instructions** field
4. Start a new chat inside the project and say "hi"

No coding. No API keys. No installation.

## Files

| File | What it is |
|---|---|
| `agent_instructions.md` | The agent brain — paste this into your Claude Project's custom instructions |
| `index.html` | The GitHub Pages site with the full guide |

## Model recommendations

| Model | Expected score range | Messages per 5hr | Best for |
|---|---|---|---|
| Free (Sonnet) | 75-85 | 15-30 | Trying the tool, scoring letters |
| Pro — Sonnet | 78-88 | ~45 | Regular applications, iterating |
| Pro — Opus | 85-92 | ~15 | High-stakes applications |
| Max | 85-92 | 225-900 | Active job searches |

## License

MIT — use it however you want.

Built by [Kevin Zentner](https://deuxcollectif.com).
