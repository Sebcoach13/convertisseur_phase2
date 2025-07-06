# Convertisseur de vitesse (km/h ↔ m/s) – Version React

Convertisseur simple de vitesses entre **kilomètres par heure (km/h)** et **mètres par seconde (m/s)**, réalisé en **React**.  
Interface minimaliste et responsive, adaptée aux ordinateurs et mobiles.

## Sommaire

- [Utilisation](#utilisation)
- [Technologies utilisées](#technologies-utilisées)
- [Structure du code](#structure-du-code)
- [Formules](#formules)
- [Exemples](#exemples)
- [Fichiers](#fichiers)

## Utilisation

1. Ouvrez le fichier `index.html` dans votre navigateur.
2. Entrez une valeur de vitesse dans le champ prévu.
3. Cliquez sur le bouton **km/h → m/s** pour convertir de kilomètres par heure vers mètres par seconde.
4. Cliquez sur le bouton **m/s → km/h** pour convertir de mètres par seconde vers kilomètres par heure.
5. Le résultat s'affiche dans le champ en dessous.

## Technologies utilisées

- [React](https://react.dev/) et [ReactDOM](https://react.dev/) via CDN  
- [Babel](https://babeljs.io/) via CDN (pour transformer le JSX côté navigateur)  
- CSS responsive (dans le fichier `style.css`)

## Structure du code

- **Mono-page** : tout le code React (JSX) est dans le fichier `index.html` (balise `<script type="text/babel">`).
- **Aucun module** : pas d’import/export, pas de build, pas de dépendances à installer.
- **Composants React** : séparation logique entre l’entrée, les boutons et l’affichage du résultat.
- **Entrées contrôlées** : chaque champ `<input>` est lié à un état React (`useState`).
- **Résultat en lecture seule** : affiché dans un champ `<input>` en `readOnly`.
- **Style** : contenu dans le fichier séparé `style.css`.

## Formules

- **km/h → m/s** : `vitesse ÷ 3,6`
- **m/s → km/h** : `vitesse × 3,6`

## Exemples

| Entrée        | Conversion         | Résultat          |
|---------------|--------------------|-------------------|
| `100` (km/h)  | km/h → m/s         | `27.8 m/s`        |
| `10` (m/s)    | m/s → km/h         | `36.0 km/h`       |

## Fichiers

- `index.html` : la page principale (inclut tout le code React)
- `style.css` : le style responsive
- `README.md` : ce fichier d'explications

**Aucune installation requise. Ouvrez simplement `index.html` avec un navigateur moderne.**
> **Note :**
> - Les boutons, champs ou composants interactifs ne sont pas rendus dans le README.md.
> - Pour voir l’application en action, ouvrez le fichier `index.html` dans un navigateur.
