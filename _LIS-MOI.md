# Dossier prêt pour GitHub Pages

Ce dossier contient **tout le nécessaire** pour mettre la démo en ligne… sauf **un seul fichier** que je ne pouvais pas générer ici (le gros HTML n'était pas accessible à jour depuis mon environnement).

## ⚠️ Étape unique à faire toi-même
Copie ton fichier de jeu **à jour** dans ce dossier et nomme-le `index.html` :

- Depuis le dossier parent `Stars racers`, copie `stars_racers_3d.html` ici, puis renomme la copie en **`index.html`**.
- PowerShell (depuis `Stars racers`) :
  ```powershell
  Copy-Item "stars_racers_3d.html" "github-deploy\index.html"
  ```

C'est important de copier **ta** version (elle a tous les derniers correctifs : tunnel, sons, physique). Les `*_data.js` et audios ici sont déjà à jour.

## Contenu du dossier (déjà prêt)
`three.min.js` · `tex3d_data.js` · `underroad_data.js` · `boost_data.js` · `buildings_data.js` · `city_data.js` · `helice_data.js` · `engine_data.js` · `idle_data.js` · `scrape_data.js` · `ground_data.js` · `collision_data.js` · `Sound/circuit_music.mp3` · `Sound/engine_loop_v3.ogg`
→ + **`index.html`** (à ajouter, étape ci-dessus)

## Mettre en ligne
Dans ce dossier `github-deploy/` :
```bash
git init
git add .
git commit -m "Stars Racers 3D — demo"
git branch -M main
git remote add origin https://github.com/TONPSEUDO/stars-racers-demo.git
git push -u origin main
```
Crée d'abord le dépôt **Public** vide sur https://github.com/new (ex. `stars-racers-demo`).

Puis sur le dépôt : **Settings → Pages → Source : Deploy from a branch → `main` / root → Save**.
~1 min après : ton lien `https://TONPSEUDO.github.io/stars-racers-demo/` — à partager. ✅

Pas besoin de `.gitignore` ici : ce dossier ne contient déjà que le strict nécessaire.
