# ⚡ Laser Studio

Logiciel web gratuit et open source de préparation et pilotage de laser GRBL — alternative libre à LightBurn.

## Fonctionnalités

- **Espace de travail vectoriel** : rectangles, ellipses, lignes, textes, zoom/pan, coordonnées en mm
- **Calques** coupe / gravure avec vitesse, puissance (%), passes et couleur par calque
- **Import SVG** par bouton ou glisser-déposer (paths Bézier aplaties, rect, circle, ellipse, line, polyline, polygon)
- **Génération de G-code GRBL** : `G21 G90`, mode laser dynamique `M4`, puissance `S` calculée d'après `$30`, export `.nc`
- **Pilotage machine** via Web Serial (Chrome/Edge) : connexion USB 115200 bauds, jog, homing `$H`, cadrage basse puissance, lancement et arrêt d'urgence, console GRBL en direct, position MPos temps réel
- **Projet** : enregistrement/chargement JSON, undo (Ctrl+Z)

## Utilisation

Aucune installation : ouvrez `index.html` dans **Chrome ou Edge** (desktop).

- **Sans machine** : dessinez, importez un SVG, cliquez « Générer G-code » et envoyez le `.nc` avec Candle, UGS, etc.
- **Avec machine** : branchez le GRBL en USB → « Connecter » → choisissez le port. Cadrage, jog, puis « Usinage ».

## Sécurité

⚠️ Portez toujours vos lunettes de protection. Ne quittez jamais la machine pendant un usinage.
Testez le cadrage et les premiers réglages à faible puissance. Logiciel fourni « tel quel », sans garantie.

## Limites connues (route map)

- Pas de remplissage raster (hatch) pour la gravure de surfaces
- Le texte n'est pas converti en G-code (aperçu uniquement)
- Pas de redimensionnement à la souris (passez par le panneau Propriétés)

Licence : MIT.
