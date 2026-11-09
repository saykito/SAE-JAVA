# Le village des Schtroumpfs, jeu de gestion en JavaFX

SAE Java du BUT Informatique 1re année, IUT de Marne-la-Vallée, Université Gustave Eiffel (2025 - 2026).

Jeu de gestion au tour par tour : le joueur dirige un village pendant 12 mois et doit éviter que ses ressources tombent à zéro.

## Principe du jeu

- **7 ressources** : baies, salsepareille, or, outils, moral, défense, savoir.
- **8 personnages** (Grand Schtroumpf, Schtroumpfette, Schtroumpf à lunettes, bricoleur, mineur, gourmand, farceur, magicien), chacun avec ses propres actions (réparer les maisons, cueillir des baies, consulter le grimoire, négocier avec les villages...).
- Chaque mois : production, consommation, événement aléatoire, choix des actions.
- Une ressource à zéro déclenche une **crise** (famine, épidémie, révolte, attaque massive, oubli des recettes).
- **Victoire** si le village finit l'année avec moins de 3 crises en cours.

En plus : sauvegarde et chargement de partie, tableau des scores, boutique, musique et effets sonores, modes d'affichage pour daltoniens (deutéranopie, protanopie, tritanopie, achromatopsie).

## Technologies

Java 21, JavaFX 21 (FXML + CSS), Maven, programmation orientée objet avec une organisation modèle / vue / contrôleur.

## Structure

```
src/
├── lanceur/MainApp.java      Point d'entrée JavaFX
├── modele/                   Logique du jeu (village, ressources, personnages, événements, crises, sauvegarde, boutique)
├── vue/                      Contrôleurs des écrans FXML, sons, mode daltonien, affichage console
├── controleur/               Déroulement d'une partie (version JavaFX et version console)
└── resources/                Fichiers FXML, CSS, images et musiques
saves/                        Sauvegardes, achats et tableau des scores
pom.xml                       Configuration Maven
```

## Lancer le jeu

Prérequis : JDK 21 et Maven.

```
mvn javafx:run
```

Maven télécharge JavaFX automatiquement. Les sauvegardes sont écrites dans le dossier `saves/`.

## Mentions

Les personnages des Schtroumpfs appartiennent à leurs ayants droit. Ce projet est un exercice scolaire sans but commercial.
