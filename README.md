# ProjetDMN

Projet universitaire : évaluer une table de décision **DMN** depuis une page web, via un serveur **WebSocket** en Java.

## Description

- Une page web (`PageWeb/`, TypeScript) envoie les valeurs d'entrée au serveur par WebSocket.
- Le serveur (`Serveur.java`, bibliothèque Java-WebSocket) reçoit le message et le transmet au parseur.
- `ParseurDMN.java` charge la table de décision `DMN/dmn.xml` avec le moteur **Camunda DMN**, l'évalue avec les variables reçues (`season`, `guestCount`) et renvoie le résultat.

## Technologies utilisées

Java · Maven · Camunda DMN Engine · Java-WebSocket · Gson · TypeScript / HTML / CSS

## Lancer le projet en local

```bash
mvn compile exec:java -Dexec.mainClass=org.example.App
```

Puis ouvrir `PageWeb/index.html` dans un navigateur.

## Contact

**Auteur :** resendecode
**GitHub :** [github.com/resendecode](https://github.com/resendecode)
