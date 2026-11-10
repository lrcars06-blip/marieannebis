# Marie-Anne Becq — l'atelier sur mesure

Tapissière, couture d'ameublement — Rampont (Meuse).

## Structure (18 fichiers, aucun build)
```
index.html    le site : intro, accueil, atelier mobilier, atelier pièce, mon projet
media/        2 films, 11 grandes photos, 1 fichier .js regroupant les 90 petites images
vercel.json   durée de cache des médias
```

## Déployer
1. GitHub : nouveau dépôt, « uploading an existing file », glisser le CONTENU de ce dossier (pas le dossier lui-même), « Commit changes ».
2. Vercel : « Add New… → Project », importer ce dépôt, Framework Preset « Other », ne rien mettre dans Build Command, Output Directory ni Root Directory, « Deploy ».
Chaque nouvel envoi sur la branche `main` redéploie le site.

## Tester en local
`npx serve .` puis http://localhost:3000/ — ne fonctionne pas en double-cliquant sur le fichier.

## Dépendances (CDN)
Three.js 0.160 (jsdelivr), Google Fonts (Fraunces, Instrument Sans, Pinyon Script).

## À brancher
Formulaire : `CONFIG.ENDPOINT` en haut du script de `index.html` (Formspree ou route API). Vide = mail pré-rempli.
