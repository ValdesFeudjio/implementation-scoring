## Notation sur la base de données
Dans cette base, nous avons environ **16 000 personnes**, et nous devons sélectionner **2 000 personnes** pour la campagne marketing.


## Ciblage aléatoire

L’objectif du projet est d’identifier les clients ayant le plus d’appétence de souscrire à nouveau un
crédit, et leur proposer une offre afin qu’ils concrétisent cette souscription.
Un ciblage simpliste peut être fait en tirant aléatoirement 2000 clients dans la base.
Il est évident que ce ciblage ne donnera pas de résultat satisfaisant, il ne rentrera d’ailleurs
logiquement pas dans la notation, mais il va permettre :
• De se fixer une référence à dépasser par la suite en utilisant des techniques de ciblage de
plus en plus perfectionnées
• Et de bien maîtriser le processus de construction et de livraison du fichier au bon format
afin de pouvoir en tester la performance

## Ciblage métier
Le but est d'identifier la règle de sélection des **2 000 clients** les plus susceptibles de souscrire un nouveau crédit.

### Variables et Justifications

- **revenu** : Un revenu plus élevé peut permettre une nouvelle souscription.    
- **mt_credits_actuel** : Un montant de crédit élevé peut indiquer un bon profil bancaire.  
- **duree_remboursement_actuel** : Une courte durée restante peut suggérer un besoin imminent d’un autre crédit.  
- **anc_dernier_credit** : Si le dernier crédit est récent, il y a plus de chances qu'un nouveau soit demandé.  
- **canal_dernier_credit** : Certains canaux (ex: en ligne) peuvent être plus favorables à la souscription rapide.  

## Ciblage sur profiling

Le but de cette méthode est d'utiliser intégralement la statistique bivariée sur la base de donnée de l'année précédente pour detecter les caractéristiques des profiles qui souscrivent au crédit et d'appliquer ces caractéristiques la à la base de 2024 pour determiner les profiles les plus aptes à souscrire. 
les différentes étapes à executer sont :


Le montant du credit actuel doit etre inferieur à 3000
Ancienneté du dernier credit inferieur à 700 jours
Le nombre de credit actuel est inférieur ou égal à 3
La duréé du remboursement actuel doit est dans {2,3,5,6}
Le montant du crédit total est inférieur à 10 000


