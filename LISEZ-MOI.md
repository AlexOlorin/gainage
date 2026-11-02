# Gainage Grimpe

Application pour le téléphone (installable sur Android, utilisable hors ligne) : routine quotidienne de gainage pensée pour l'escalade. Fichiers : `index.html`, `manifest.webmanifest`, `sw.js`, icônes, `three.module.min.js`.

- **Thèmes** : gainage et L-sit, compression (monter les pieds haut), hanches et souplesse, épaules et poussée (pompes et dips), force des jambes (chaise, squat cosaque, pistol).
- **Niveaux** : Débutant, Intermédiaire, Expert, découpés en paliers. Après une séance réussie, l'appli propose le palier suivant.
- **Semaine** : jours de séance forte, de séance légère, de grimpe et de repos, réglables dans le menu ⋯. Les jours de grimpe, seulement un échauffement.
- **Lecteur mains libres** : la séance s'enchaîne toute seule (effort, repos, changement de côté) avec des bips, une voix et des vibrations. Touche l'écran pour la pause.
- **Animations** : un mannequin en 3D (Three.js) pour chaque exercice, avec son matériel (poignées, chaise, barres, mur, montant de porte). Le bon geste, puis les erreurs à éviter : la partie fautive en rouge, le bon geste en vert transparent. Dans la fiche d'un exercice, on tourne autour du mannequin au doigt.

Sauvegarde locale : clé `gainage:v1`.

## Publication

Site : https://alexolorin.github.io/gainage/ (GitHub Pages, branche `main`). Dépôt : https://github.com/AlexOlorin/gainage. Après chaque modification : changer `CACHE` dans `sw.js`, commit, `git push`. L'ancien artifact claude.ai n'est plus mis à jour. Historique antérieur au 2026-11-02 : dépôt For-Claude, dossier `gainage/`.
