# TP 0 — Application Web Jakarta EE

Application réalisée pour le TP 0. Elle utilise JSF pour l’interface Web, CDI pour relier les classes et PrimeFaces pour la liste des rôles.

## Fonctionnement

L’utilisateur choisit un rôle et saisit une question. Le serveur affiche la question en majuscules, son nombre de mots et l’historique de la conversation. Le bouton « Nouveau chat » réinitialise la conversation.

Il s’agit d’un traitement Java local : l’application n’interroge pas de modèle d’IA.

## Technologies

- Java 25
- Jakarta EE 11
- JSF, CDI et PrimeFaces 16.0.1
- Maven et Payara 7

## Exécution

Ouvrir le projet dans IntelliJ IDEA avec le JDK 25. Configurer Payara 7, puis lancer le déploiement de l’artifact `war exploded`.

Page : `http://localhost:8080/TP0-ALAMI_LOUATI-1.0-SNAPSHOT/`

## Structure

- `index.xhtml` : interface JSF
- `Bb.java` : état du chat et actions de la page
- `GenerateurReponse.java` : traitement de la question
- `web.xml` : ouverture automatique de `index.xhtml`
- `resources/css` et `resources/js` : style et fonctions de l’interface

`HelloServlet.java` et `index.jsp` sont conservés pour montrer les premières étapes du TP.
