#  MoBotSim - Simulation de Robot Mobile
### *Pour un aperçu plus complet de mon travail, visitez mon portfolio sur [imonge.es](https://imonge.es/proyecto/4?lang=fr).*
> **Remarque** : Ceci est la première phase d'un projet plus large, avec l'objectif ultime d'implémenter ces fonctions sur un vrai robot d'ici la fin de l'année.
---
##  Aperçu
MoBot vise à aider à analyser l'environnement du robot et à répondre aux commandes textuelles de l'utilisateur, tout en simulant ses mouvements. Nous utilisons une base de données d'images fournie dans les spécifications. Le programme a besoin d'une image .png et d'une conversion de cette image en .txt (vérifiez le dossier images)
###  Fonctionnalités Principales
MoBot offre trois fonctionnalités principales :
1. **Traitement d'Image**
   - Détecte une balle dans l'image et retourne :
     - Les coordonnées de son centre
     - Sa couleur
     - Son diamètre
     - Sa superficie
2. **Traitement de Texte**
   - Interprète les commandes textuelles de l'utilisateur et déduit les actions correspondantes à effectuer par le robot.
      -  Langues : Français, Espagnol
      -  Envoi d'une matrice d'actions et de paramètres à la partie "simulation de mouvement" du programme
3. **Simulation de Mouvement du Robot**
   - Simule les mouvements du robot dans un environnement virtuel basé sur les données d'entrée d'image et de texte.
---
## 🛠️ Installation
Pour commencer avec MoBot, suivez ces étapes :
1. **Cloner le Dépôt** :
   ```bash
   git clone https://github.com/IsmaTIBU/MobotSim.git
   cd mobot
2. **Installer les Bibliothèques Python** : Assurez-vous d'avoir Python 3.x installé. Turtle est une bibliothèque de base pour ces versions.
---
##  Utilisation
1. **Compiler et exécuter l'exécutable** :
   ```bash
   make
   ./main
   
---
##  Documentation
Pour plus d'informations techniques, veuillez vous référer au [dossier de documentation](https://github.com/IsmaTIBU/MobotSim/blob/main/Documentation_G4.zip)
 dans ce dépôt. Il suffit d'extraire et d'ouvrir index.html.
---
## Quelques résultats
1.**Traitement d'image** : Nous avons regroupé tous les tests ensemble dans une seule photo [photo](images/Modélisations.png.JPG) 
Toutes les balles sont détectées quel que soit le nombre, les cas nuls sont fonctionnels. Les diamètres sont également assez bons, sauf sur quelques photos. Pour aller plus loin, l'utilisation de bibliothèques d'apprentissage profond nous permettrait d'ajuster considérablement les résultats, mais dans les spécifications du projet, je ne peux utiliser que le C de base pour le traitement d'image.
2.**Traitement de texte** :
Fonctionne très bien sur beaucoup de phrases en français et espagnol par exemple :
Français
- compte le nombre de boules puis tourne de 180 degrés vers la gauche puis recule de 1000 mètres
- avance de 1000 mètres puis tourne de cent quatre vingt dix neuf degrés vers la droite puis avance de deux cent mètres
Espagnol
- gira de 50 grados hacia la izquierda luego avanzar de doscientos metros
- avanza a la pelota azul luego gira de sesenta grados luego avanza de 126 metros
3.**Simulation** :
Fonctionne parfaitement
Vidéo de résultats : [Ici](https://github.com/IsmaTIBU/MobotSim/blob/main/Presentation.mp4)
