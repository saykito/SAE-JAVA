# SAE JAVA, le village des Schtroumpfs

Projet de SAE, BUT Informatique 1re année, IUT de Marne-la-Vallée (2026).

Jeu de gestion au tour par tour en Java et JavaFX : le joueur dirige un village de Schtroumpfs, gère ses ressources et fait face à des événements et des crises aléatoires. Chaque personnage a des actions qui lui sont propres.

## Fonctionnalités

- Personnages aux capacités différentes : Grand Schtroumpf, Schtroumpfette, Schtroumpf à lunettes, bricoleur, farceur, gourmand, magicien, mineur
- Gestion des ressources du village
- Événements et crises générés aléatoirement à chaque tour
- Boutique, sauvegarde de partie et tableau des scores (dossier `saves/`)
- Mode daltonien et gestion audio

## Architecture MVC

```
src/modele/       logique du jeu (village, personnages, ressources, événements, sauvegarde)
src/vue/          interfaces FXML, feuille de style, contrôleurs de vue
src/controleur/   lien entre la vue et le modèle
src/lanceur/      MainApp, point d'entrée
```

## Lancer

Prérequis : JDK 21 et Maven.

```
mvn clean javafx:run
```
