# Courses Hebdo

Page web (un seul fichier, sans serveur) pour choisir chaque vendredi midi les repas de la semaine et préparer les courses du Drive Carrefour du samedi matin. Famille de 4, dont deux ados.

- **Menu** : semaine du samedi au vendredi, petit-déjeuner tous les jours, midi le mercredi, samedi et dimanche, dîner tous les soirs. Une proposition est faite automatiquement ; chaque repas peut être changé.
- **Courses** : liste regroupée par rayon, quantités additionnées et ajustables au nombre de personnes, lien de recherche Carrefour par produit, cases à cocher et copie de la liste.
- **Recettes** : 30 plats et 10 petits-déjeuners simples, avec ingrédients et étapes.

Les choix sont gardés dans le navigateur (localStorage). Ouvrir `index.html` suffit.

## Panier Drive automatique

Ouverte dans Claude avec le connecteur Carrefour, la page ajoute un bloc « Remplir mon panier Drive » dans l'onglet Courses :

1. choix du magasin Drive (ville ou code postal) ;
2. recherche de chaque produit non coché dans ce magasin ;
3. choix du meilleur rapport qualité/prix : le coût le plus bas pour couvrir la quantité voulue (nombre de paquets × prix, promos comprises), avec une pénalité de 15 % sur les gammes premier prix (Classic', Simpl…) ;
4. vérification produit par produit (les produits du placard sont décochés par défaut), puis ajout au panier en un clic et lien pour finaliser la commande sur carrefour.fr.

Ouverte hors de Claude, la page garde les liens « Chercher » vers carrefour.fr.
