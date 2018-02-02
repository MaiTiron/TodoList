# TodoList
Projet de cours basé sur le site todomvc.com

## User stories
Définition des actions de l'utilisateur :
- [ ] User peut ajouter une tâche
- [ ] User peut valider une tâche
- [ ] User peut supprimer une tâche
- [ ] user peut afficher les tâches réalisées
- [ ] User peux afficher les tâches à réaliser
- [ ] User peux supprimer toutes les tâches réalisées

## Mise en place du projet
Etapes à suivre pour préparer le projet TodoList
- [ ] Initier un serveur Nodejs
- [ ] Créer la base de données MongoDB
- [ ] Créer une route `front` pour afficher un fichier `index` dans le dossier `www`
- [ ] Créer une route `api` qui renvoie en `json` l'objet `{msg: 'Hello API'}`

## Configurer la base de données
Le but est de définir les modèles de données à utiliser pour l'application
- [ ] Combien d'informtaions faut-il enregistrer pour une tâche ?
- [ ] Comment une tâche est-elle validée ?
- [ ] Comment une tâche est-elle supprimée?
- [ ] Comment les tâches sont filtrées ?

### 1. Combien d'informations daut-il pour enrefgistrer pour une tâche
Il faut trois informations :
- _id: String
- state: boolean
- content: String

### 2. Comment une tâche est-elle validée ?
Quand l'état est égale à `true`.

### 3. Comment une tâche est-elle supprimée ?
Chaque tache présente un bouton qui, au clic, permet de supprimer l'objet de la base de données :
- Connaître l'`_id` de l'objet
- Créer une route `API` pour supprimer l'objet de la bdd

### 4. Comment les tâches sont filtrées ?
Sélectionner tous les objets et n'afficher que ceux dont la propriété `state` est égale à `true` (ou `false`)
- [ ] Créer une route `API` pour sélectionner les tâches