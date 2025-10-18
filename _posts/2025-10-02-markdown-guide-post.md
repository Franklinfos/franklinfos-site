---
layout: post
title: "Guide complet du MarkDown"
date: 2025-10-02
author: "Claude.ai"
tags: ["tuto","site"]
image: "https://download.logo.wine/logo/Markdown/Markdown-Logo.wine.png"
---

# Bienvenue dans le monde du Markdown !

Vous vous demandez comment écrire du texte avec une belle mise en forme ? Pas de panique ! Le Markdown est là pour vous simplifier la vie. C'est un système d'écriture ultra-simple qui transforme votre texte brut en contenu joliment formaté.

Imaginez que vous écrivez un message, et qu'en ajoutant quelques symboles simples, votre texte devient automatiquement beau et bien organisé. C'est exactement ce que fait le Markdown !

## Pourquoi utiliser le Markdown ?

- **C'est simple** : pas besoin de cliquer sur des boutons, tout se fait en tapant
- **C'est rapide** : une fois que vous connaissez les symboles, c'est plus vite que d'utiliser une souris
- **C'est universel** : le Markdown fonctionne partout sur internet
- **C'est lisible** : même sans transformation, votre texte reste facile à lire

## Comment créer un article ?

Il faut créer un fichier Markdown, avec cet en-tête (ne pas oublier les trois tirets avant et après !):
```
---
layout: post
title: "Titre de l'article"
date: YYYY-MM-DD
author: "Auteur de l'article"
tags: ["tags éventuels", "tous entres guillemets", "listés comme ça"]
---
```
Si vous voulez rajouter une image qui s'affichera à côté du titre de l'article, il faut rajouter cette ligne :  
`image: "lien de l'image (voir plus bas)"`  
Ensuite, vous pouvez écrire votre article, mis en page grâce aux techniques suivantes :

## Les titres et séparateurs : structurer votre contenu

Pour créer des titres, utilisez le symbole dièse `#`. Plus vous en mettez, plus le titre est petit :

```
# Titre principal (très grand)
## Titre de section (grand)
### Sous-titre (moyen)
```

**Rendu :**

# Titre principal (très grand)
## Titre de section (grand)
### Sous-titre (moyen)

Pensez aux titres comme aux chapitres d'un livre : le titre principal pour votre article, les titres de section pour les grandes parties, et les sous-titres pour les détails.

---
Placer trois tirets ainsi `---` permet d'obtenir un séparateur (il faut penser à sauter une ligne avant).

## Mettre en valeur votre texte

### L'italique pour l'emphase

Entourez votre texte avec des astérisques ou des underscores :

```
*Ce texte est en italique*
_Celui-ci aussi_
```

**Rendu :** *Ce texte est en italique*, _celui-ci aussi_

Utilisez l'italique pour mettre en avant un mot important ou pour les titres d'œuvres.

### Le gras pour l'importance

Utilisez deux astérisques ou deux underscores :

```
**Ce texte est en gras**
__Celui-ci aussi__
```

**Rendu :** **Ce texte est en gras**

Le gras attire vraiment l'œil ! Utilisez-le pour les informations cruciales.

### Combiner les deux

```
***Ce texte est en gras ET en italique***
```

**Rendu :** ***Ce texte est en gras ET en italique***

## Les listes : organiser vos idées

### Liste à puces (non ordonnée)

Pour une liste sans ordre particulier, utilisez des tirets, des astérisques ou des plus :

```
- Première chose
- Deuxième chose
- Troisième chose
```

**Rendu :**

- Première chose
- Deuxième chose
- Troisième chose

Vous pouvez même créer des sous-listes en décalant avec des espaces :

```
- Fruits
  - Pommes
  - Bananes
- Légumes
  - Carottes
  - Tomates
```
**Rendu :**

- Fruits
  - Pommes
  - Bananes
- Légumes
  - Carottes
  - Tomates

### Liste numérotée (ordonnée)

Pour une liste avec un ordre précis, utilisez des chiffres :

```
1. Première étape
2. Deuxième étape
3. Troisième étape
```

**Rendu :**

1. Première étape
2. Deuxième étape
3. Troisième étape

Parfait pour des instructions ou un classement !

## Les liens : connecter votre contenu

Pour créer un lien cliquable, la syntaxe est :

```
[Texte du lien](adresse-du-site.com)
```

**Exemple :**

```
[Visitez Google](https://www.google.com)
```

**Rendu :** [Visitez Google](https://www.google.com)

Le texte entre crochets est ce que vos lecteurs verront, et l'adresse entre parenthèses est la destination.

## Les images : illustrer vos propos

Pour ajouter une image, c'est presque comme un lien, mais avec un point d'exclamation devant :

```
![Description de l'image](adresse-de-l-image.jpg)
```

**Exemple :**

```
![Un magnifique coucher de soleil](https://example.com/sunset.jpg)
```

La description entre crochets est importante : elle s'affiche si l'image ne charge pas, et aide les personnes malvoyantes à comprendre votre image.
L'image peut soit être enregistrée dans le répertoire GitHub, soit provenir d'un site Internet. Si l'image provient du répertoire GitHub, elle doit être enregistrée dans `/assets/images/votre-image.jpg`. Son lien sera alors le suivant : `{% raw %}{{ site.baseurl }}/assets/images/votre-image.jpg{% endraw %}`.

## Les citations : mettre en avant des passages

Pour créer une citation, utilisez le symbole "supérieur à" `>` :

```
> Ceci est une citation importante.
>
> Elle peut prendre plusieurs lignes. (Voir la section sur les paragraphes)
```

**Rendu :**

> Ceci est une citation importante.
>
> Elle peut prendre plusieurs lignes. (Voir la section sur les paragraphes)

Utilisez les citations pour les témoignages, les extraits d'un texte, ou pour mettre en valeur une information clé.

## Les tableaux : ordonner vos idées

Pour créer un tableau, il faut les recréer dans l'éditeur avec les symboles `|` et `-` :

```
| Titre 1       |     Titre 2     |        Titre 3 |
| :------------ | :-------------: | -------------: |
| Colonne       |Colonne          |Colonne         |
| Alignée à     |Alignée au       |Alignée à       |
| Gauche        |Centre           |Droite          |
```

**Rendu :**

| Titre 1       |     Titre 2     |        Titre 3 |
| :------------ | :-------------: | -------------: |
| Colonne       |Colonne          |Colonne         |
| Alignée à     |Alignée au       |Alignée à       |
| Gauche        |Centre           |Droite          |

## Les paragraphes et sauts de ligne

### Créer des paragraphes

Pour séparer deux paragraphes, laissez simplement une ligne vide entre eux :

```
Ceci est mon premier paragraphe.

Ceci est mon deuxième paragraphe.
```

### Forcer un retour à la ligne

Si vous voulez aller à la ligne sans créer un nouveau paragraphe, terminez votre ligne par deux espaces (invisibles mais importants !).

## Exercice pratique

Essayez de reproduire ce texte en Markdown :

---

**Mon premier article**

Bonjour ! Je découvre le Markdown et j'adore ça.

Voici ce que j'ai appris :

- Créer des titres
- Mettre en gras et en italique
- Faire des listes

> Le Markdown, c'est vraiment facile !

Pour en savoir plus, visitez [ce site utile](https://example.com).

---

## En résumé

Le Markdown n'a rien de compliqué ! Avec ces quelques symboles simples :

- `#` pour les titres
- `*` ou `_` pour l'italique et le gras
- `-` pour les listes
- `>` pour les citations
- `[texte](lien)` pour les liens
- `![texte](image)` pour les images
- `---` pour un séparateur
- Deux espaces après le texte pour un retour à la ligne, une ligne vide pour sauter une ligne

Vous pouvez créer des articles magnifiques et professionnels. L'essentiel est de pratiquer : plus vous utiliserez le Markdown, plus ce sera naturel.  
N'ayez pas peur d'essayer ! Le Markdown est fait pour être simple et intuitif. Alors lancez-vous, et amusez-vous bien !

**Bon courage dans vos futures créations !** 🚀