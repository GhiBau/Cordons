# Jugement de cordon

Serious game 3D, dans le navigateur, pour former les arbitres de tir à l'arc au jugement d'une flèche « cordon » (flèche dans le rouge, tube proche de la ligne rouge/jaune).

## Principe

1. L'arbitre arrive à la cible (tir à 18 m, blason de 40 cm).
2. Il enchaîne les actions de procédure dans le bon ordre : scores relevés, flèche désignée, accessoires retirés (casquette, sifflet, télécommande du Chronotir), puis placement sur le côté, à la tangente gauche et droite, et regard à la loupe.
3. Il annonce le score (8 ou 9 pour un cordon rouge/jaune) avec la formulation de son choix.
4. Le bilan note la procédure (50), la décision (40) et la formulation (10), et explique l'écart réel mesuré entre le tube et la ligne.

Trois niveaux de difficulté (écart de 1,2–2,4 mm, 0,4–1,2 mm, 0,12–0,4 mm). Une case « Aide immédiate » donne le retour action par action.

## Règle appliquée

Une flèche dont le tube touche une ligne de séparation de zone prend la valeur la plus haute (règlement II.02, art. B.6.2). Pour le cordon rouge/jaune : touche la ligne = 9, ne la touche pas = 8.

## Hypothèses de modélisation

- Ligne de séparation de 0,8 mm de large.
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
