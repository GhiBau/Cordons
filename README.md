# Jugement de cordon

Serious game 3D, dans le navigateur, pour former les arbitres de tir à l'arc au jugement d'une flèche « cordon » (tube très proche d'une ligne de séparation de zone).

## Principe

1. L'arbitre arrive à la cible. Deux dispositions au choix (réglage « Cible ») : salle 18 m avec 4 blasons de 40 cm et 3 flèches par blason (12 flèches), ou TAE avec un blason de 122 cm et 24 flèches. La flèche en litige est sur l'un des blasons, tirée au hasard.
2. Il enchaîne les actions de procédure dans le bon ordre : scores relevés, flèche désignée, accessoires retirés (casquette, sifflet, télécommande du Chronotir), puis mise sur le côté gauche et sur le côté droit (avec réglage de la hauteur des yeux) et regard à la loupe.
3. Il annonce le score (7, 8, 9, 10 ou X) avec la formulation de son choix.
4. Le bilan note la procédure (50), la décision (40) et la formulation (10), et explique l'écart réel mesuré entre le tube et la ligne.

Les actions « Se mettre sur le côté gauche » et « Se mettre sur le côté droit » ouvrent un petit jeu : l'arbitre choisit la hauteur de ses yeux (curseur « Se baisser / Se lever ») pour regarder dans l'axe de la ligne, avec une tolérance large (10°), puis valide. Chaque validation hors de l'axe coûte 2 points.

La loupe se sort avec le bouton en bas à droite de l'image. Le blason peut être neuf, abîmé ou criblé d'impacts (réglage « Blason ») : le niveau « criblé » ajoute plus de cent impacts, dont une vingtaine regroupés autour de la flèche en litige. Un blason abîmé porte déjà beaucoup d'impacts de flèches, dont quelques-uns juste à côté de la flèche en litige (à ne pas confondre avec le tube), parfois une déchirure, un coin arraché, des plis, des salissures et des lignes effacées. Quand la ligne rouge/jaune est effacée d'un côté de la flèche, il faut la prolonger à partir de la partie intacte.

La flèche en litige est près d'une des lignes 8/9, 9/10 ou 10/X (le petit cercle du X), toujours du côté de la zone de valeur inférieure : le tube frôle ou touche la ligne par en dessous (réglage « Ligne »). Sur un blason abîmé, des trous noirs sur la ligne gênent la lecture ; dans certains cas, un morceau du blason est arraché au contact : on peut alors accorder la valeur haute au bénéfice du doute, mais l’arbitre reste libre d’apprécier (les deux réponses sont acceptées). Trois niveaux de difficulté, l'arbitre n'étant appelé que pour une flèche très proche de la ligne (écart de 0,4–0,9 mm, 0,15–0,45 mm, 0,04–0,15 mm). Une case « Aide immédiate » donne le retour action par action.

Une seule flèche est litigieuse par partie : toutes les autres sont à plus d'un millimètre d'une ligne, clairement d'un côté ou de l'autre.

## Règle appliquée

Une flèche dont le tube touche une ligne de séparation de zone prend la valeur la plus haute (règlement II.02, art. B.6.2). Touche la ligne = valeur supérieure (9, 10 ou X selon la ligne), ne la touche pas = valeur inférieure.

## Hypothèses de modélisation

- Ligne de séparation de 0,8 mm de large (salle) ou 1,5 mm (TAE) ; le règlement impose 2 mm au maximum.
- Salle 18 m : blasons de 40 cm centrés à 1,60 m et 1,00 m du sol, 60 cm entre centres (II.02, B.2.2.1.2). TAE : blason de 122 cm centré à 1,30 m.
- Tubes de 5,5, 6,0 ou 6,5 mm de diamètre.
- La flèche en litige penche de 5 à 9° ; elle penche vers le centre dans 60 % des cas, ce qui peut masquer la ligne en vue de face.

## À valider avec les formateurs d'arbitres

- Les justifications affichées pour chaque action.
- Le jugement sur les formulations (« Elle est x » notée plus haut que « Je pense / Je crois »).
- Le barème de procédure et la pénalité d'ordre (−10) si l'arbitre se place avant d'avoir relevé les scores, fait désigner la flèche et retiré ses accessoires.
- La liste des mauvaises actions (toucher ou retirer la flèche, demander l'avis de l'archer ou d'un spectateur, demander à qui est la flèche, regarder de face).

## Utilisation

Ouvrir `index.html` dans un navigateur récent (Chrome, Edge, Firefox, Safari) avec WebGL. Une connexion internet est nécessaire : Three.js (r128) est chargé depuis cdnjs et les polices depuis Google Fonts.

Commandes : glisser pour tourner autour de la cible, molette pour zoomer.

## Publication sur GitHub Pages

1. Créer un dépôt GitHub public (par exemple `cordon`).
2. Y déposer `index.html`, `README.md` et `.nojekyll`.
3. Dans le dépôt : Settings, Pages, « Deploy from a branch », branche `main`, dossier `/ (root)`, Save.
4. Après une à deux minutes, le jeu est en ligne à l'adresse `https://<compte>.github.io/<dépôt>/`.

Pour modifier le jeu, éditer `index.html` et valider (commit) : la page se met à jour toute seule.
