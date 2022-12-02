# Les structures conditionnelles

[Mémento Python](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3.pdf){:target="_blank"}

Les structures de contrôle sont un élément central de la programmation.
Elles permettent de moduler l’exécution d'un programme selon la valeur de ses variables.
Les structures de contrôle se retrouvent de façon presque identique dans les autres langages de programmation.

## L'instruction if

L’instruction `if` (si, en anglais) permet d’effectuer une liste d’instructions uniquement si une valeur booléenne (appelée la condition) est True (vraie) et une autre liste d’instruction sinon.
```python
ok = True
if ok:
	print("la variable ok est vraie")
else:
	print("la variable ok est fausse")
```

Dans l’exemple ci-dessus, on définit la variable booléenne `ok` à True (vrai).
L’instruction `if` teste cette variable. 
Si elle est vraie, le bloc d’instructions (décalé à droite) qui vient après les deux points est exécuté. 
Le bloc `else` (sinon, en français) est exécuté si la condition du `if` n’est pas respectée.
Notez que le bloc `else` n'est pas obligatoire.

L’indentation du texte (le décalage à droite) est importante.
Elle permet à l’ordinateur de savoir quelles sont les instructions qui appartiennent au bloc du `if` et quelles sont celles qui appartiennent au bloc du `else`.
(L'indentation se fait de préférence avec la touche tabulation du clavier.)

> ### <span style="background-color:#c6d9f7">  Exercice 15 - Jeune ou vieux ?
> 
> Ecrivez un programme qui demande son âge à l’utilisateur. 
> Si l’utilisateur donne un nombre inférieur à 20, le programme écrit "Comme vous êtes jeune !", sinon il écrit "Comme vous êtes vieux !".

> ### <span style="background-color:#c6d9f7">  Exercice 16 - Maximum
> 
> Ecrivez la fonction maximum(a, b) qui prend 2 nombres en argument et retourne le plus grand.

Le bloc `elif` peut être ajouté après le bloc `if` pour tester des conditions supplémentaires.
Notez que `elif` est la contraction de else if (sinon si, en français).
L'exemple suivant démontre son utilité quand on a 4 situations possibles:
```python
il_est_tard = False
je_suis_fatigue = False

if il_est_tard and je_suis_fatigue:
	print("Je vais dormir")
elif il_est_tard and not je_suis_fatigue:
	print("Je joue à la console")
elif not il_est_tard and je_suis_fatigue:
	print("Je fais une sieste")
else:
	# Il ne reste plus qu'une seule possibilité
	print("Je vais courir dehors")
```

> ### <span style="background-color:#c6d9f7">  Exercice 17 - Gagné, perdu ou match nul ?
> 
> Ecrivez un programme qui demande à l'utilisateur d'entrer les buts de l'équipe domicile et de l'équipe extérieur.
> Le programme affiche ensuite quelle équipe a gagné le match (ou match nul en cas d'égalité).
>
> **Exemples d’exécution :**
> ```
> Buts marqués par l'équipe domicile : 1
> Buts marqués par l'équipe extérieur : 2
> L'équipe extérieur a gagné !!
>
> Buts marqués par l'équipe domicile : 0
> Buts marqués par l'équipe extérieur : 0
> Match nul !
> ```

## L'instruction while

L’instruction while (qui signifie "tant que" en anglais) permet de répéter
un bloc d’instructions tant qu’une condition est remplie.

```python
a = 1
while a < 100:
	print(a)
	a = a*2
print(f"Maintenant a vaut {a} !")
```
Dans cet exemple, on initialise la variable `a` à 1.
Puis, tant qu’elle est inférieure à 100, on l’affiche à l’écran et on la double. 
Ainsi, `a` passera de 1 à 2 à 4 à 8, etc. 
Le programme imprime donc toute les puissances de deux inférieures à 100.

> ### <span style="background-color:#c6d9f7">  Exercice 18 - La puissance du 10
> 
> Modifier le programme ci-dessus pour qu’il imprime toutes les puissances de 10 inférieures ou égales à 10000.

> ### <span style="background-color:#c6d9f7">  Exercice 19 - Comment ça va ?
> 
> Ecrivez un programme qui demande en boucle à l'utilisateur comment il va tant qu'il ne répond pas "Bien merci et toi ?".
> Rappel: la fonction `input()` permet de demander à l'utilisateur d'entrer du texte.
>
> **Exemple d’exécution :**
> ```
> Comment tu vas ? Bien
> Comment tu vas ? Bof
> Comment tu vas ? Nickel !
> Comment tu vas ? Bien merci et toi ?
> Très bien, merci de demander !
> ```

La fonction `randint(min, max)` du module `random` permet de tirer un nombre entier aléatoire entre `min` et `max` (compris).
Voici un exemple où le programme tire un nombre aléatoire entre 1 et 100.
```python
import random

n = random.randint(1, 100)
print(a)
```

> ### <span style="background-color:#c6d9f7">  Exercice 20 - Devine mon nombre
> 
> Ecrivez un programme qui permet de jouer à "Devine mon nombre":
> 1. Laissez le programme tirer un nombre aléatoire entre 1 et 50.
> 2. Demandez à l'utilisateur de proposer un nombre tant qu'il n'a pas trouvé le bon.
> 3. A chaque proposition de nombre, le programme affiche "Plus grand" ou "Plus petit" pour aider le joueur.
> 4. (Facultatif) Comptez le nombre de coups nécessaires pour trouver le bon nombre.
> 
> **Exemple d’exécution :**
> ```
> Devine mon nombre: 32
> Plus grand
> Devine mon nombre: 43
> Plus petit
> ...
> Devine mon nombre: 38
> Gagné, c'était bien 38 ! (Il vous a fallu 6 coups)
> ```


---

[Retour à l'accueil](../README.md)