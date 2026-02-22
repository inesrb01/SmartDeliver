Diagramme de cas d’utilisation

Ce diagramme montre les différents acteurs du système (Client, Livreur, Administrateur, Service de paiement) et les fonctionnalités principales du projet SmartDeliver.

On a utilisé :
- <<include>> pour montrer que le paiement fait partie du processus de commande.
- <<extend>> pour la réinitialisation du mot de passe.

---

 Diagramme de séquence – Connexion

Ce diagramme montre le processus de connexion d’un utilisateur.

Le client entre son email et mot de passe.
Le Frontend envoie la demande au Backend.
Le Backend vérifie dans la base de données.
La base retourne le résultat.
Ensuite le Backend envoie la réponse au Frontend.
Finalement, le Frontend affiche le message au client.

Ce diagramme montre bien la communication entre les différentes couches du système.

---

 Diagramme de classes – Authentification

Ce diagramme représente le composant d’authentification que nous avons implémenté.

Il contient trois classes :

- User : contient les informations de l’utilisateur.
- UserRepository : gère l’accès à la base de données.
- AuthService : contient la logique de connexion et d’inscription.

On a utilisé le Repository Pattern pour séparer la logique métier de l’accès aux données.

---

 Diagramme de composants

Ce diagramme représente l’architecture globale du système.

On voit :
- Le Frontend
- Le Backend
- La base de données
- Le service de paiement externe

Il montre la séparation claire entre les différentes parties du système.
