# TP 3 - Formulaire Symfony

## Rapport du travail réalisé

J'ai créé une page produit avec formulaire en Symfony en suivant ces étapes :

### 1. Création du contrôleur
J'ai fait un contrôleur `ProductController` avec une route `/`. Ce contrôleur :
- Affiche la page du produit
- Gère le formulaire d'ajout au panier
- Montre un message de confirmation après soumission

### 2. Création du formulaire
J'ai créé un `ProductType` dans le dossier `Form/Type/`. Ce formulaire contient :
- Un champ "quantity" (nombre) avec valeur par défaut 1
- Un champ "color" (liste déroulante) avec 3 couleurs
- Un bouton "Add to Cart" stylisé

### 3. Personnalisation de l'affichage
J'ai personnalisé le formulaire de deux manières :

**Configuration globale :**
Dans `twig.yaml`, j'ai dit à Symfony d'utiliser Bootstrap pour les formulaires.

**Thème personnalisé :**
J'ai créé `custom_theme.html.twig` qui modifie comment les champs s'affichent :
- Ajoute des marges entre les champs
- Applique les classes Bootstrap

### 4. Page produit
Le template `index.html.twig` contient :
- L'image du produit
- Toutes les informations du casque audio
- Le formulaire avec les champs créés
- L'intégration Bootstrap complète

### 5. Techniques utilisées
- **FormBuilder** : Pour créer le formulaire dans le code PHP
- **Helpers Twig** : `form_start()`, `form_row()`, `form_end()` pour afficher
- **Options de champs** : Classes CSS, valeurs par défaut, styles
- **Personnalisation** : Via les fichiers de configuration et les thèmes

### Résultat final
La page affiche exactement ce qui était demandé dans le TP :
- Le produit avec ses caractéristiques
- Un formulaire fonctionnel avec quantité et couleur
- Design identique à la maquette HTML
- Bootstrap 5.3 intégré

Le formulaire est entièrement géré par Symfony tout en gardant l'apparence demandée.
