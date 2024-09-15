
Module 1 : Les Fondamentaux
Qu'est-ce que Node.js ?
Imagine Node.js comme un environnement qui te permet d'exécuter du JavaScript côté serveur. Au lieu de simplement animer des pages web dans le navigateur, tu peux désormais créer des applications complètes, des API, et même des logiciels de bureau en utilisant ton JavaScript préféré.
Pourquoi Node.js ?
 * Asynchrone et non bloquant: Cela signifie que Node.js peut gérer plusieurs requêtes en même temps sans ralentir.
 * Événements: Tout dans Node.js est basé sur des événements, ce qui le rend très efficace pour les applications en temps réel.
 * V8: Il utilise le moteur JavaScript de Chrome, ce qui garantit des performances élevées.
 * npm: Un gestionnaire de packages très riche qui te donne accès à une multitude de modules pour étendre les fonctionnalités de tes applications.
Installation et environnement de développement
 * Installation de Node.js: Télécharge l'installeur officiel de Node.js depuis leur site web (https://nodejs.org/) et suis les instructions.
 * Éditeur de code: Choisis un éditeur comme Visual Studio Code, Sublime Text ou Atom. Ils offrent une syntaxe colorée, une auto-complétion et d'autres fonctionnalités utiles pour le développement JavaScript.
 * npm: Node.js vient avec npm (Node Package Manager) préinstallé. Tu l'utiliseras pour installer et gérer les dépendances de tes projets.
Les bases de Node.js
 * Module system: Chaque fichier JavaScript dans Node.js est un module. Tu peux exporter et importer des fonctionnalités entre ces modules.
 * Événements: Node.js est basé sur un modèle événementiel. Les événements sont des actions qui se produisent et auxquelles tu peux réagir.
 * Flux (streams): Les flux sont des interfaces pour lire ou écrire des données de manière séquentielle, comme lire un fichier ou écrire dans un fichier.
 * Callbacks, promesses et async/await: Ces mécanismes te permettent de gérer le code asynchrone de manière plus propre et plus lisible.
Exemple simple d'un serveur Node.js:
const http = require('http');

const hostname = '127.0.0.1';
const port = 3000;

const server = http.createServer((req, res) => {
  res.statusCode = 200;
  res.setHeader('Content-Type', 'text/plain');
  res.end('Hello World\n');
});

server.listen(port, hostname, () => {
  console.log(`Server running at http://${hostname}:${port}/`);
});

Explication:
 * require('http') : Importe le module HTTP de Node.js pour créer un serveur.
 * createServer : Crée un serveur HTTP.
 * req et res : Représentent respectivement la requête et la réponse.
 * res.statusCode, res.setHeader et res.end : Configurent la réponse et envoient du contenu.
Prêt à continuer ?
On peut approfondir un de ces points, ou passer directement à Express. Qu'en penses-tu ?
Possibles sujets pour la suite:
 * Les modules Node.js en détail
 * La programmation asynchrone avec les promesses et async/await
 * Le système de fichiers
 * Introduction à Express
N'hésite pas à poser toutes tes questions !
 * https://www.grouparoo.com/blog/node-js-and-ipv6
 * https://magnetoitsolutions.com/blog/node-js-serverless-framework-aws-lambda-tutorial
 
