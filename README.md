# Steve Octets

La vitrine : <https://steveoctets.github.io>

Ce dépôt ne contient que le site d'accueil. Chaque application a le sien, dans son
propre dépôt, avec ses versions publiées et son flux de mises à jour.

| Application | Dépôt                                                 | Site                                 |
| ----------- | ----------------------------------------------------- | ------------------------------------ |
| Kodama      | [steveoctets/kodama](https://github.com/steveoctets/kodama) | <https://steveoctets.github.io/kodama/> |
| Kumoji      | [steveoctets/kumoji](https://github.com/steveoctets/kumoji) | <https://steveoctets.github.io/kumoji/> |

Les plugins Omarchy n'ont pas de site à eux : leur carte mène à leur dépôt GitHub, dont le
README tient lieu de documentation.

| Plugin Omarchy | Dépôt                                                              | Installation                                                                   |
| -------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------ |
| Agenda         | [snouhaud/omarchy-agenda](https://github.com/snouhaud/omarchy-agenda) | `omarchy plugin add https://github.com/snouhaud/omarchy-agenda.git --enable` |
| rclone mounter | [snouhaud/rclone-mounter](https://github.com/snouhaud/rclone-mounter) | `omarchy plugin add https://github.com/snouhaud/rclone-mounter.git --enable` |

## Ajouter une application

1. Créer son dépôt, sur le modèle de `steveoctets/kodama` : `docs/` pour le site servi par
   GitHub Pages, `docs/appcast.xml` pour le flux de mises à jour, les archives en pièces
   jointes de release.
2. Déposer son icône dans `images/`, en PNG de 256 pixels.
3. Copier le bloc `<a class="application">` de `index.html`, et l'adapter.
4. Ajouter une ligne au tableau ci-dessus.

## Ajouter un plugin Omarchy

1. Déposer son icône dans `images/` (PNG de 256 pixels, ou SVG).
2. Copier une carte de la section « Plugins Omarchy » de `index.html` et de `en/index.html`,
   la faire pointer vers le dépôt, et ajouter sa commande d'installation dans la `.note`.
3. Ajouter une ligne au tableau des plugins.

`style.css` est commun à tous les sites, mais chacun en garde sa copie : un site doit
pouvoir vivre sans l'autre.
