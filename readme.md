
# Database Exercise

## Déroulé de l'exercice

Nous allons réaliser une application permettant de gérer des dépenses entre amis. 
A partir d'un thème donné, vous devez modéliser la base de données et alimenter l'ensemble des bases par des données fictives.

Forkez ce dépot.
Travaillez au sein de votre dépot. Puis lorsque vous êtes prêts à livrer le code produit, réalisez un pull request.

## Exercice

Semblable à tricount ou encore à moneybuster. Cette application permettra à un utilisateur de centraliser les dépenses lors de vacances ou d'évènements privés.

 Chaque personne peut avoir son compte utilisateur et être associé à plusieurs groupes d'utilisateurs. 

 Un groupe d'utilisateurs sera identifié par un nom de groupe.

 Chaque utilisateur peut ajouter une dépense.
 Cette dépense concernera un groupe. 
 Lorsqu'un utilisateur ajoute une dépense il définit : 
 
  - celui qui a payé
  - ceux concernés par la dépense
  - le montant de la dépense
  - un label précisant le motif de la dépense

 Un utilisateur peut avoir un avatar
 
 Une fois que vous aurez réussi à modéliser la base de données et à y incorporer un peu de donnée fictive, ajoutez des triggers ou des procédures stockées pour les besoins suivants : 

  - il est possible de modifier une dette. La modification réalisée est historisée.
  - il est possible d'avoir un rapport automatiquement retourné par la base de données avec pour chaque groupe: chaque utilisateur avec son solde
  - avoir une procédure stockée qui retourne la personne qui est la plus endettée. Afin que ce soit cette personne là qui fasse les prochaines courses.
 - il est possible de modifier son avatar. Ce qui va impacter que l'ancien avatar n'est plus référencé sur le serveur. Faites en sorte que cette image soit automatiquement retirée sur serveur. 

## Livrables attendsu
 
Stockez au sein de ce dépot :

  * Le fichier SQL de la génération de la BDD
  * Le script permettant d'importer des données en masse
  * Le fichier SQL pour les triggers et procédures stockées.