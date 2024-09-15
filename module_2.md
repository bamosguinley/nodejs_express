Module 2 : Express.js
Qu'est-ce qu'Express.js ?
Express.js est un framework minimaliste et flexible pour Node.js qui facilite la création d'applications web et d'API. Il offre une couche d'abstraction au-dessus de Node.js, en simplifiant la gestion des requêtes HTTP, des routes, des vues et bien plus encore.
Pourquoi utiliser Express ?
 * Simplicité: Express est conçu pour être facile à apprendre et à utiliser.
 * Flexibilité: Il ne vous impose pas une structure rigide, ce qui vous permet de personnaliser votre application.
 * Performance: Express est très performant et est largement utilisé dans des applications à forte charge.
 * Grande communauté: Une communauté active fournit de nombreux modules et ressources.
Installation:
npm install express --save

Création d'un serveur Express basique:
const express = require('express');
const app = express();
const port = 3000;

app.get('/', (req, res) => {
  res.send('Hello, Express!');
});

app.listen(port, () => {
  console.log(`Server listening on port ${port}`);
});

Explication:
 * require('express') : Importe le module Express.
 * app.get('/') : Définit une route GET pour la racine (/) de l'application.
 * res.send() : Envoie une réponse au client.
Les routes:
Express utilise un système de routes pour définir les différentes URL que votre application peut gérer. Chaque route est associée à une méthode HTTP (GET, POST, PUT, DELETE) et à un gestionnaire de requête.
Les middlewares:
Les middlewares sont des fonctions qui s'exécutent avant les gestionnaires de route. Ils peuvent être utilisés pour :
 * Logger les requêtes: Enregistrer les informations sur chaque requête.
 * Authentifier les utilisateurs: Vérifier si un utilisateur est connecté.
 * Parser le corps des requêtes: Convertir les données envoyées dans le corps de la requête en un format utilisable.
Exemple de middleware:
app.use((req, res, next) => {
  console.log('Time:', Date.now());
  next();
});

Les vues:
Express peut utiliser différents moteurs de templates pour générer du HTML dynamique. Les plus populaires sont Pug, EJS et Handlebars.
Prêt à aller plus loin ?
Nous pouvons explorer en détail :
 * Les différentes méthodes HTTP
 * Les paramètres de route
 * Les moteurs de templates
 * La gestion des erreurs
 * Les bases de données avec Express
Quelle partie d'Express souhaites-tu approfondir ?
N'hésite pas à poser toutes tes questions !
 * https://www.atatus.com/blog/express-vs-hapi/
 * 
