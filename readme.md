
## Team CACEIS

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
- [ ] `Monitoring` : monitorer chaque appels et leur durée<br/>
- [ ] `Logging` : centraliser les logs de l'application


## Accès au code source

```
git clone https://github.com/caceishack2018/

2 projets : 
- un containerbank pour le site en en hsql avec la majorité des fonctionnalités
- un site (advisorRest) exposant un service rest appelant un pod mysql avec base de données persistante.

Les fichiers de configurations sont sous le projet AdvisorRest :
- dck_container pour la partie FRONT.
- dck_advisorrest pour la partie API.
- dck_mysql pour la DB

```
## Reste à faire
- Sortir les autres services en REST (Customer, Card, Payment)
- Intégrer les services REST au site containerbank et supprimer le hsql.
- Gérer le monitoring et les logs : On a pensé à utliser la sortie standard avec un daemon syslog mais on n'a pas eu le temps de l'implémenter.

