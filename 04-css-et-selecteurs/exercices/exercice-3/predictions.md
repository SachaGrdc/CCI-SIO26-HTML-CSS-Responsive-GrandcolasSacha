# Partie B - Prédictions et vérification

| Élément            | Couleur | Taille                   | Graisse       | Règle gagnante (couleur) et raison                           | Constaté dans l'inspecteur           |
| :----------------- | :------ | :----------------------- | :------------ | :----------------------------------------------------------- | :----------------------------------- |
| h1                 | navy    | défaut navigateur (32px) | bold (défaut) | .titre (0, 1, 0) bat h1 (0, 0, 1).                           | Identique (navy, 32px, bold)         |
| 1er paragraphe     | orange  | 20px                     | bold          | .intro et .texte ont la même spécificité (0, 1, 0), mais .intro est écrit après. Pour la graisse, p.texte (0, 1, 1) bat .texte (0, 1, 0). | Identique (orange, 20px, bold)       |
| em (dans le 1er p) | orange  | 20px                     | bold          | Héritage du <p> parent (aucune règle ne cible em).           | Identique (orange, 20px, bold)       |
| 2e paragraphe      | purple  | 16px                     | bold          | p#special (1, 0, 1) bat .texte (0, 1, 0). Graisse : p.texte bat .texte. | Identique (purple, 16px, bold)       |
| 3e paragraphe      | gray    | 16px                     | normal        | Erreur : j'avais pensé à p { color: gray; } car il est à la fin, mais c'est div p { color: green; } qui gagne. | Écart : couleur green (16px, normal) |

## Explication des écarts

3e paragraphe : div p a une spécificité de (0, 0, 2) alors que p tout seul vaut (0, 0, 1). Même si p { color: gray; } est écrit plus bas dans le fichier il est moins spécifique donc green gagne

.conteneur { color: brown; } : Cette règle tout en bas ne s'applique qu'en héritage. Comme tous les éléments ont déjà une règle directe (même faible comme p ou h1) la couleur marron n'apparaît nulle part