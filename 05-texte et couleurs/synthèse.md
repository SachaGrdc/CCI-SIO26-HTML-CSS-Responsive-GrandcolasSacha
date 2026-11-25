## Formalisation (20 min)

Synthèse : propriétés étudiées avec exemple, formats de couleurs, tableau comparatif `px`/`em`/`rem`, règles de lisibilité.



### 1. Propriétés étudiées

- `color` : couleur du texte. Ex : `color: #2c3e50;`
- `background-color` : couleur de fond. Ex : `background-color: #f4f4f4;`
- `font-family` : police. Ex : `font-family: Arial, sans-serif;`
- `font-size` : taille du texte. Ex : `font-size: 1.25rem;`
- `font-weight` : épaisseur (normal, bold). Ex : `font-weight: bold;`
- `font-style` : inclinaison. Ex : `font-style: italic;`

### 2. Formats de couleurs

On peut utiliser différentes méthodes :

- Nom : `blue`
- Hexadécimal : `#ff6347`
- RGB : `rgb(255, 99, 71)`
- RGBA (avec transparence) : `rgba(255, 99, 71, 0.5)`
- HSL : `hsl(9, 100%, 64%)`

### 3. Comparatif `px` / `em` / `rem`

| Unité | Référence                                      | À retenir                               |
| ----- | ---------------------------------------------- | --------------------------------------- |
| `px`  | taille fixe                                    | précise mais ne s'adapte pas            |
| `em`  | taille de police du parent                     | se cumule dans les éléments imbriqués   |
| `rem` | taille de police de `<html>` (16px par défaut) | prévisible, à privilégier pour le texte |

### 4. Règles de lisibilité

- Contraste suffisant entre texte et fond (au moins 4,5:1).
- Ne pas utiliser la couleur seule pour donner une information.
- Police simple et lisible, 2 polices maximum.
- Taille de texte d'au moins 16px (1rem).