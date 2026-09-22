# Driftsradar

Statusoverblik over de services vi bruger (Puzzel, Splashtop, Microsoft 365 og Azure).

Siden: https://madsfj.github.io/Driftsradar/

## Sådan virker det

- `index.html` er selve siden.
- `services.json` er den fælles liste over services.
- `scripts/hent-status.mjs` henter statussider og feeds fra en server og skriver `status.json`, så browseren ikke bliver blokeret af CORS.
- `.github/workflows/driftsradar.yml` kører scriptet hvert 10. minut (og ved push til `main`) og udgiver siden på GitHub Pages.

## Opsætning

Settings → Pages → Source skal stå på **GitHub Actions**.
