---
inclusion: always
---

# Kiroween Rebrand Context

## Project Background
This is a rebrand of an existing horror game (Data_Bleed) for the Kiroween competition. The goal is to replace ChromaBot branding with Kiro ghost assets while maintaining all functionality.

## Key Constraints
- **Budget**: $0/month (Vercel free tier only)
- **No Backend**: Game must work with client-side fallbacks
- **Asset Locations**: Kiro frames in `chroma-bot/assets/img/Chroma_Org_Logo_No_Background/`
- **Deployment**: Vercel with cache-busting required

## Code Style Preferences
- Use timestamp-based cache-busting: `?v=${Date.now()}`
- Maintain existing file structure (don't rename files)
- Keep all game mechanics identical
- Focus on visual asset replacement only

## Competition Category
**Costume Contest**: The UI itself is the "costume" - it transforms based on player decisions (trust score). Clean Kiro ghost → Corrupted nightmare.

## Development Approach
- Vibe coding for creative solutions (corruption animation timing)
- Spec-driven for structured tasks (asset replacement, deployment)
- Iterative debugging (cache issues, Vercel config)
