# Note de synthèse


## Étapes du projet
1. [X] Mettre en place l'environnement de développement
2. [X] Découper la maquette
3. [X] Intégrer le header du projet
4. [X] Ajouter le formulaire de recherche
5. [X] Ajouter la partie Filtres
6. [X] Réaliser la "card" présente dans "Hébergements à Marseille"
7. [X] Gérer l'affichage des "cards" du conteneur "Hébergements à Marseille"
8. [X] Intégrer le conteneur "Activités à Marseille"
9. [X] Implémenter le footer
10. [X] Mettre en place le responsive design
11. [X] Vérifier la qualité du code


## Spécifications fonctionnelles

### Fonction recherche
- Les usagers pourront rechercher des hébergements dans la ville de leur choix.
- Le champ de recherche est un champ de saisie, le texte doit donc pouvoir être édité par l'utilisateur.
- Il faut englober ce champ dans un formulaire. La partie Recherche ne doit pas être fonctionnelle - il s'agit d'une première version pour valider l'interface.

### Liens "Hébergements" et "Activités"
Les textes "Hébergements" et "Activités", situés dans l'en-tête, sont des liens. Ils doivent mener respectivement vers la section "Hébergements à Marseille" et "Activités à Marseille".

### Cartes hébergements et activités
- Chaque carte d'hébergement ou d'activité devra être cliquable dans son intégralité (pas uniquement le titre).
- Pour l'instant, les liens sont vides. On peut utiliser un attribut 'href="#"' pour simuler la présence d'un lien.

### Filtres de recherche
- Les hébergements peuvent être filtrés par thématique, comme le budget ou l'ambiance.
- Les filtres doivent changer de couleur au survol de la souris.
- Les filtres ne doivent pas être fonctionnels - il s'agit juste d'une première version pour valider l'interface.


## Spécifications techniques

### Maquettes
Trois maquettes ont été réalisées : desktop, tablette et mobile.

### Breakpoints
Nous avons convenu avec le designer UI d'utiliser 1024 px et 768 px :
- supérieur à 1024 px pour les écrans d’ordinateurs ;
- supérieur ou égal à 768 px pour les tablettes ;
- inférieur à 768 px pour les téléphones portables.

### Largeur min - max
Pour éviter d'étirer la page web sur la largeur de façon excessive, il va falloir déterminer une largeur maximum de 1440 px. Au-delà, une marge blanche doit apparaître sur les côtés et le contenu doit se limiter à 1440 px de large.
La largeur minimum est fixée à 320 px, en-deçà de cette largeur, le comportement n'est pas garanti.

### Desktop first
Il faut d'abord réaliser l'intégration pour les ordinateurs (autrement dit, en desktop first), puis les tablettes et enfin les téléphones. L'utilisation des Media Queries nous permettra de réaliser l'intégration pour les différents supports.

### Bibliothèque d'icônes
Les icônes proviennent de la bibliothèque Font Awesome.

### Couleurs
Les couleurs de la charte sont le bleu (#0065FC), le bleu clair (#DEEBFF) et le gris pour le fond (#F2F2F2).

### Police
La police du site est Raleway. Nous pouvons passer par Google Fonts pour importer facilement cette police dans le code : https://fonts.google.com/specimen/Raleway.

### Mise en page
Il est recommandé d'utiliser Flexbox.

### Balises sémantiques
Il est important d'utiliser des balises sémantiques, au minimum "header", "nav", "h1-h2-h3", "main", "section", "article" et "footer".

### Validité du code
- Aucun IDE ou éditeur de code particulier n’est imposé pour le développement.
- Le code doit être valide aux validateurs W3C HTML et CSS.
- Le code HTML ne doit pas contenir de propriété CSS.
- Lors du passage du desktop au mobile et à la tablette, ne pas dupliquer le code HTML (exception faite dans le formulaire avec le mot "Rechercher" et l'icône de la loupe).
- Privilégier l'utilisation des classes CSS pour cibler un élément, plutôt que d'utiliser le nom de l'élément lui-même.
- Ne pas dupliquer des classes CSS inutilement. Exemple : si 4 éléments sont identiques du point de vue de la mise en forme, alors utiliser une seule et même
classe CSS, et non pas 4.

### Compatibilité navigateurs
La maquette doit être compatible avec les dernières versions de Google Chrome et de Mozilla Firefox. Il faudra tester la page web sur ces deux navigateurs.

### Restrictions
Aucun framework CSS (type BootStrap ou Tailwind CSS) ou préprocesseur CSS (type Sass ou Less) ne doit être utilisé.
Aucun autre langage ne doit être utilisé (comme JavaScript, par exemple).