# Notes détaillées : gainage

(Déplacées de CLAUDE.md pour alléger le contexte ; à chercher par mot-clé.)

### Gainage Grimpe (`index.html`)

- PWA : `manifest.webmanifest`, `sw.js` (changer `CACHE` à chaque version), icônes PNG, `three.module.min.js` (Three.js 0.170 en local pour le hors-ligne, repli sur le CDN). Sauvegarde locale : clé `gainage:v1`.
- Données clés : `EXOS` (chaque exercice renvoie à une animation par `anim`), `ERREURS` (textes des erreurs par animation), `PAL` (paliers par thème), `seance()` (composition selon le jour).
- Animations 3D (section 11, `moteur3D(THREE)`, appelée une fois Three.js chargé) : squelette à longueurs fixes et cinématique inverse pour les appuis. `PZ` contient les poses (angles en degrés, `ancre`, `vise`, `sol`, `ik`) et `ANIM3` les animations (caméra, accessoires, séquence, erreurs). Un seul contexte WebGL (`M3`) passe d'une vue à l'autre ; les vignettes sont rendues en images.
- Poses : angle de la cuisse depuis la verticale basse vers l'avant = `h − rot` ; angle du tibia = angle de la cuisse − `g`.
- Tester avec Playwright en servant `gainage/` en HTTP (sinon l'import de Three.js échoue).
- Publication : GitHub Pages (voir LISEZ-MOI.md). L'artifact claude.ai n'est plus mis à jour.
