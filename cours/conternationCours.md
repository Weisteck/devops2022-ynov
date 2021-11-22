# Cours de conteneurisation

## Virtualisation 

 - Technologie
 - Representation virtuelle d'un serveur

 Embarque tous les composants d'un serveur de maniere virtuelle


## Conterneurisation

 - Methode de stockage
 - Methode de transport

 Espace d'execution, n'embarque que ce qui est demande


 ### Docker, c'est quoi ?

 Logiciel
 Permet la conteneurisation
 Multi plateforme


### Pourquoi l'utiliser ?

- Pour conteneuriser une ou plusieurs application
- Pouvoir partager / tester localement une application quelque soit l'environnement de depart
- Pouvoir s'assurer de la bonne compatibilite differents environnements


### Comment l'executer ?

- En ligne de commande
- Graphique

### Comment l'utiliser ?

Documentation :
``` 
Version web : https://docs.docker.com
Version cli : docker --help
```

Build : `docker build`
Tag : `docker tag`
Run : `docker run`

### Concept d'une image docker

```dockerfile
# file : base
ARG {variable}
FROM 

ENV
RUN
WORKDIR

ENTRYPOINT
CMD
```

Commande lancee :
```
docker build -t base .
docker run base
```


#### Diff entre ARG et ENV

Dans le build : ARG + ENV
Run : ENV



## Organisation

### Minicube

Commande utile :
- lancer le serveur :
``` minikube start ```
- etat :
``` minikube status ```
- se connecter a la vm :
``` minikube ssh ```
- logs :
``` minikube logs ```
- recuperer de l'adresse ip
``` minikube ip ```
