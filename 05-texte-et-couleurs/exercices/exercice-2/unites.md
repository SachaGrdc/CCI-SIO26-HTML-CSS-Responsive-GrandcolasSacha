### Exercice 2 — Comparer les unités

**Objectif** : observer les différences entre `px`, `em` et `rem`.
**Durée indicative** : 25 min



| Unité | Racine | Niveau 1 | Niveau 2 | Niveau 3 |
| ----- | ------ | -------- | -------- | -------- |
| em    | 16 px  | 24       | 36       | 54       |
| rem   | 16 px  | 24       | 24       | 24       |
| em    | 20 px  | 30       | 45       | 67,5     |
| rem   | 20 px  | 30       | 30       | 30       |



Aucun écart attendu. En em, la taille se calcule à partir de celle du parent, donc elle se multiplie à chaque niveau : 16 x 1,5 = 24, puis 24 x 1,5 = 36, puis 36 x 1,5 = 54.

En em il n'y a aucun écart puisque la taille se calcule à partir de celle du parent donc pour la racine a 16px il fallait faire 16 x 1.5 = 24 puis 24 x 1.5 = 36 et enfin 36 x 1.5 = 54

Pour la racine a 20px : 20 x 1.5 = 30 puis 30 x 1.5 = 45 et enfin 45 x 1.5 = 67.5



En rem il n'y a aucun écart non plus puisque la taille se calcule à partir de celle de la racine et pas de celle du parent donc les trois niveaux ont la même taille. 

Pour la racine à 16px il fallait faire 16 x 1.5 = 24 pour chaque niveau (niveau 1, niveau 2 et niveau 3).
Pour la racine à 20px : 20 x 1.5 = 30 pour chaque niveau.





- px : taille fixe pour les détails qui ne doivent pas bouger
- em : relative au parent, pour qu'un élément s'adapte à son contexte en faisant attention au cumul.
- rem : relative à la racine, à privilégier pour les tailles de texte