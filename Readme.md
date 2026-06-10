---
title: Dojo Python
description: 'Quiz Game'
layout: tic-tac
---

# Quiz Game

![Header](assets/image/riddler.PNG)
{: .text-center }

## Instructions
- Le quiz doit contenir exactement 3 questions, et donc 3 réponses.
- Le joueur aura 3 essais par question.
- Si le joueur répond correctement, ses essais sont réinitialisés lors de la question suivante.
- Afficher des messages quand il perd, gagne, quand son nombre d’essais évolue.
- Arrêter le jeu si l’utilisateur perd tous ses essais.
- **Bonus** : Mettre en place un compteur de points à chaque bonne réponse et lui afficher.

## Spécifications
- Utiliser, à minima, une collection de données pour stocker les questions et réponses attendues.
- Utiliser des boucles.
- Utiliser des conditions.
- Permettre au joueur de saisir ses réponses.
- Arrêter le jeu quand il ne lui reste plus d’essais (`break`) ou quand il a gagné.
- Le guider dans le jeu.
- Réduire le nombre d’essais à chaque mauvaise réponse et les réinitialiser après chaque bonne réponse.
- **Bonus** : Faire gagner des points pour chaque bonne réponse et afficher le nombre de points total en fin de partie.

## Extensions pour les plus rapides (Boss Final)
Si votre groupe a terminé l'exercice principal en avance et que le code est propre (sans copier-coller de blocs de code), choisissez l'un des défis suivants pour pimenter votre jeu :

### Option 1 : Le Boss "Mort Subite" (Facile)
Ajoutez une 4ème question spéciale à la fin de votre code (hors de la boucle principale). 
- **Règle :** C'est la question du Boss. Le joueur n'a le droit qu'à **un seul essai** (pas de reset à 3). Si la réponse est bonne, elle rapporte le double de points, sinon la partie est instantanément perdue.

### Option 2 : Le Boss à Points de Vie (Moyen)
Après les 3 questions, le joueur affronte le Boss final dans un duel de logique.
- **Règle :** Le Boss possède 3 Points de Vie (PV). Le jeu continue tant que le Boss a des PV ET que le joueur a encore des essais. Chaque bonne réponse retire 1 PV au Boss. Chaque mauvaise réponse retire un essai au joueur. 

### Option 3 : Le Boss Chronométré (Difficile)
Pour l'ultime question, le temps est compté.
- **Règle :** Faites des recherches sur le module `time` de Python. Le joueur doit donner sa réponse en moins de 10 secondes, sinon le Boss gagne automatiquement et la partie s'arrête.
