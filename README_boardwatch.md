# BoardWatch

Arbiter-facing web app for live illegal move tracking and result entry during MCC chess tournament rounds.

## How it works

1. **TD** opens the app → uploads SJSON file → shares PIN with arbiters
2. **Arbiters** open the app on their phones → enter PIN → tap boards to record illegal moves and results
3. **TD** exports updated SJSON when all games are done

All data syncs through Supabase (PostgreSQL) in real time.

## Setup

The app is a single `index.html` file — no build step needed.

### GitHub Pages deployment

1. Clone this repo
2. Push to `main` branch
3. In GitHub repo settings → Pages → Source: "GitHub Actions"
4. The workflow deploys automatically on every push

### Access

- **URL**: `https://gerhardtrippen.github.io/BoardWatch/`
- **PIN**: `1444`
