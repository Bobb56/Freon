# Langage Freon

## Freon

**Freon** est un fork de **Neon** dont le but est de se rapprocher le plus possible de la programmation en langage naturel ou pseudo-code.  
Freon reprend toutes les fonctionnalités de **Neon**, mais avec un redesign complet de l'interface console, des noms de fonctions, des mots-clés, des opérateurs, des messages d'erreurs, des noms de types et des constantes prédéfinies.

### Voici une liste complète des changements apportés par Freon :

#### Mots-clés :

- `for` → `Pour`
- `while` → `TantQue`
- `if` → `Si`
- `elif` → `SinonSi`
- `else` → `Sinon`
- `end` → `Fin`
- `function` → `Fonction`
- `method` → `Methode`
- `return` → `Renvoyer`
- `import` → `Importer`
- `local` → `Locale`
- `continue` → `Continuer`
- `break` → `Sortir`
- `pass` → `NeRienFaire`

#### Noms de fonctions :

- `print` → `Afficher`
- `input` → `Demander`
- `nbr` → `nbr`
- `str` → `chaine`
- `len` → `longueur`
- `sub` → `souschaine`
- `exit` → `Quitter`
- `append` → `Ajouter`
- `remove` → `Enlever`
- `insert` → `Inserer`
- `type` → `type`
- `reverse` → `retourner`
- `eval` → `evaluer`
- `clear` → `Effacer`
- `help` → `aide`
- `randint` → `entAleat`
- `failwith` → `QuitterAvec`
- `time` → `temps`
- `assert` → `Verifier`
- `output` → `Ecrire`
- `chr` → `car`
- `ord` → `ascii`
- `list_comp` → `compDeListe`
- `create_exception` → `CreerErreur`
- `exception` → `Erreur`
- `int` → `ent`
- `index` → `indice`
- `replace` → `remplacer`
- `count` → `compter`
- `list` → `lister`
- `sort_asc` → `Trier_croiss`
- `sort_desc` → `Trier_decroiss`
- `sin` → `sin`
- `cos` → `cos`
- `tan` → `tan`
- `deg` → `deg`
- `rad` → `rad`
- `sqrt` → `racine`
- `ln` → `ln`
- `exp` → `exp`
- `log` → `log`
- `log2` → `log2`
- `round` → `arrondir`
- `abs` → `abs`
- `ceil` → `partEntSup`
- `floor` → `partEntInf`
- `readFile` → `lireFichier`
- `writeFile` → `EcrireFichier`

#### Opérateurs :

- `and` → `et`
- `or` → `ou`
- `not` → `non`
- `xor` → `oux`
- `del` → `suppr`
- `in` → `dans`
- `%` → `mod` #modulo
- `=` → `<-` #affectation
- `<-` → `:=` #affectation par nom de variable

#### Constantes prédéfinies :

- `True` → `Vrai`
- `False` → `Faux`
- `None` → `Rien`

#### Noms de types :

- `Bool` → `Booleen`
- `String` → `Chaine`
- `Number` → `Nombre`
- `Built-in function` → `Fonction de base`
- `List` → `Liste`
- `Function` → `Fonction`
- `Method` → `Methode`
- `Exception` → `Erreur`
- `AnyType` → `N'importe quel type`

### Autres choses traduites :

Messages d'erreurs et noms d'exceptions prédéfinies.

### Autres nouveautés :

Afin de pouvoir créer des programmes dont le format ressemble plus à du pseudo-code, le caractère `|` a été banalisé : l'interpréteur ignore ce caractère comme il ignore un espace. Ainsi, le programme suivant est un programme Freon parfaitement valide, et affichant 120 :

```freon
Fonction Factorielle(n) faire
| Si (n <= 1) alors
| | Renvoyer (1)
| Sinon
| | Renvoyer ( Factorielle(n-1) * n )
| Fin
Fin
Afficher (Factorielle(5))
