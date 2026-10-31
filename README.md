# AgroConnect — prototype 0.1

Prototype React + Vite, avec le logo fourni intégré.

## Installation sous Windows
1. Installer Node.js LTS depuis https://nodejs.org/
2. Fermer puis rouvrir PowerShell.
3. Décompresser ce dossier, puis exécuter :

```powershell
cd "$HOME\Downloads\AgroConnect"
npm install
npm run dev
```

4. Ouvrir l'adresse indiquée par Vite (généralement http://localhost:5173).

## Démonstration
- Créer un compte : il est placé « En attente ».
- Administration : `admin@agroconnect.demo`
- Mot de passe de démonstration : `AgroConnectDemo!`
- Valider un compte depuis l'espace administration.
- Déposer une annonce depuis un compte validé, puis la publier depuis l'administration.

## Limites importantes
Ceci est une maquette locale destinée à tester les écrans et les parcours. Les données sont conservées dans le navigateur (localStorage). Ne pas y saisir de vrais mots de passe ni de données sensibles.
Aucun serveur, base de données distante, paiement réel, messagerie ou livraison n'est activé. La connexion administrateur et les validations de cette maquette ne constituent pas une sécurité de production.

## Architecture cible
- Interface : React + Vite.
- Backend et base de données : Supabase / PostgreSQL.
- Authentification et droits : Supabase Auth + Row Level Security.
- Images : Supabase Storage.
- Paiements : Wave, Orange Money et carte, via des prestataires marchands à sélectionner et à valider avant toute intégration réelle.
- Zone : Afrique, avec pays et lieux renseignés sur les annonces.
- Livraison : à développer dans une version ultérieure.

## Étapes suivantes
1. Valider l'interface et les parcours.
2. Créer le schéma de base de données.
3. Mettre en place l'authentification et les autorisations côté serveur.
4. Intégrer les paiements en environnement de test après vérification des conditions des prestataires.
5. Préparer les versions française, anglaise et wolof avec validation des traductions.
