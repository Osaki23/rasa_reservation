Un ChatBot permettant aux utilisateurs de réserver une table dans un restaurant à une date et une heure précise, afficher les infos d'une réservation ou annuler sa réservation.

Guide d'utilisation:

Ouvrir un terminal dans le repository du projet et lancer le serveur d'actions avec la commande suivante:
- rasa run actions 

Ouvrir un deuxième terminal et lancer la commande pour entrainer le modèle:
- rasa train

ensuite:
  pour chatter avec le bot lancer:
- rasa shell

  Vous pouvez débuter la conversation par "bonjour" ou bien demander directement la réservation d'une table.

  Remarques:

  - format de la date de réservation: le xx mois à xxhxx
    exemple: le 20 mai à 19h00

  - format du nombre de personnes: x personnes
    exemple: 2 personnes

  - Les réservations sont enregistrées dans un fichier json nommé reservation.json

  Quelques petits problèmes:
  
  - Le bot pourrait ne pas comprendre votre nom et vous redemander un autre, il faudrait alors peut-être choisir un nom dans la liste du intent "nom" dans nlu.yml
  - Reformuler les phrases si jamais il ne comprend pas
