# Kosovo Explore — AI udhërrëfyes me hartë, mot dhe planifikues

## Çka ka
- Chat AI (vetëm Kosova) → tregon vendin në Google Maps (Hartë / Satelit / Street View)
- **Moti live** (Open-Meteo, pa API key): shirit me 7 qytete lart, panel me moti tani + 5 ditë,
  lindja/perëndimi i diellit, dhe këshillë "çka me bo sot" sipas motit. Moti edhe në çdo kartë.
- Info praktike: km dhe koha e vozitjes nga Prishtina, sezoni më i mirë, vendet afër
- Foto (Wikimedia Commons) + video (YouTube link ose embed me key)
- 29 vende must-visit me filtër sipas rajonit
- **Plani im**: shto vende, radhiten automatikisht, hape rrugën me waypoints në Google Maps,
  ose pyete AI-n për itinerar. Ruhet në browser.
- 🎲 "Befasoje" — vend i rastësishëm

## Deploy në Vercel
1. Ngarko `index.html`, `api/chat.js`, `README.md` në repo (GitHub).
2. Vercel → Add New Project → zgjedh repon → Deploy.
3. Settings → Environment Variables → `ANTHROPIC_API_KEY` → Redeploy. Lart shfaqet "AI aktiv".
   Pa key punon me bazën lokale (29 vende + moti + harta).

## Opsionale (falas)
- `GOOGLE_API_KEY` në index.html (Maps Embed API) → Street View brenda faqes
- `YOUTUBE_API_KEY` në index.html (YouTube Data API v3) → video brenda faqes
