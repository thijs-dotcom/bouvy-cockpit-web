# bouvy-cockpit-web — deploy-artefact (nginx-static)

Statische build van de Bouvy Cockpit (`Projecten/Cockpit/` in de mainframe-repo), geserveerd via nginx
op **cockpit.slimverzekeren.ai** (Coolify). Backend = Convex (managed).

## Herdeployen na wijzigingen
In de mainframe-repo (`Projecten/Cockpit/`):
```
VITE_CONVEX_URL="https://academic-akita-864.convex.cloud" npm run build
```
Kopieer de nieuwe `dist/` hierheen, commit + push → Coolify redeployt automatisch.
