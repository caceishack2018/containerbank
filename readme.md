# Bienvenue au Hackathon PackApp !

L’objectif principal est de conteneuriser et API-ser l’application containerbank afin de pouvoir la déployer sur le CaaS AWS. Vous l'avez compris, vous devrez découper l'application de la plus belle façon qui soit . Consignes générales : 
- :heavy_check_mark: **L’application doit être fonctionnelle**, c’est-à-dire couvrir tous les use cases exposés ci-après
- :computer: **Aucune restriction ne s’applique aucxw design de l’interface utilisateur** : libre à vous de la modifier du moment qu'elle permet de couvrir tous les use cases
- :wink: **Carte blanche** ! Modifiez, découpez, réarchitecturez, détruisez : l'application doit tourner sur le CaaS !  

## Use cases

- [x] `ViewAdvisors` : voir une liste de conseillers et leurs spécialités (none, savings, credits ou insurance)<br/>
- [x] `ViewCustomer` : voir les informations relatives à un client<br/>
- [x] `EditCustomer` : mettre à jour les informations relatives à un client<br/>
- [x] `AddCustomer` : ajouter un nouveau client au système<br/>
- [x] `ViewCard` : voir les informations relatives à une carte bleue<br/>
- [x] `EditCard` : mettre à jour les informations relatives à une carte bleue<br/>
- [x] `AddCard` : ajouter une nouvelle carte bleue au système<br/>
- [x] `ViewPayment` : voir des informations relatives à l'historique de paiement d’une carte bleue<br/>
- [x] `AddPayment` : ajouter des informations relatives à un paiement (nature du paiement)<br/>
- [] `Monitoring` : monitorer chaque appels et leur durée<br/>
- [] `Logging` : centraliser les logs de l'application


## Accès au code source

```
git clone https://github.com/caceishack2018/

2 projets : 
- un containerbank pour le site en en hsql avec la majorité des fonctionnalités
- un site (advisorRest) exposant un service rest appelant un pod mysql avec base de données persistante.

## Reste à faire
Sortir les autres services en REST
Intégrer les services REST au site containerbank et supprimer le hsql.
Gérer le monitoring et les logs

