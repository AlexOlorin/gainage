# Gainage Grimpe

Toujours répondre en français. Règles communes : `D:\CODE\CLAUDE.md`. Proposer avant d'agir pour toute modification importante.

PWA de gainage pour l'escalade (un seul `index.html` + `sw.js`). Publiée sur https://alexolorin.github.io/gainage/ par GitHub Pages (`git push` sur `main` = mise en ligne en 1-2 min).

## Carte du code (`index.html`)
Données : `EXOS`, `ERREURS`, `PAL`, `ECHAUF`/`CALME`/`GRIMPE`. État : `charger`/`sauver` (clé `gainage:v1`). Séances : `seance()`, `lancer()`. Jours de grimpe : `typeDuJour`/`changerJour` (exceptions datées `S.exc`). Matériel : `MAT`, `REMPL` (exo → remplaçant sans matériel), `remplacant`, `choisirMateriel` (feuille avant la séance), `demarrer` (`S.mat`). Historique : `historique()`. Animations 3D : `moteur3D`, `PZ` (poses ; variantes sans matériel : `auSol`, `PLI_SOL`), `ANIM3`. Démarrage : `accueil()`. Chercher (Grep) plutôt que lire en entier.

## À chaque modification
- Changer `CACHE` dans `sw.js`, sinon le téléphone garde l'ancienne version.
- Tester en HTTP (le module Three.js ne charge pas en `file://`).
- Commit en français, puis `git push`.
- Détails techniques : `NOTES.md`.
