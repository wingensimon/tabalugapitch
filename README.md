# Grünflügel × Tabaluga Pitch — Railway Deploy

Statische Seite (eine self-contained HTML-Datei, alle Bilder eingebettet).

## Deploy auf Railway

1. Diesen Ordner als Git-Repo hochladen (GitHub o. ä.):
   ```
   git init && git add . && git commit -m "pitch"
   git remote add origin <dein-repo>
   git push -u origin main
   ```
2. Railway → **New Project → Deploy from GitHub repo** → Repo wählen.
3. Railway erkennt Node automatisch (package.json) und startet `npm start`
   → statischer Server auf dem von Railway gesetzten PORT.
4. Unter **Settings → Networking → Generate Domain** den öffentlichen Link erzeugen.

Kein Build-Schritt nötig — `index.html` funktioniert komplett offline.
