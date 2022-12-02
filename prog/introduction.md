# Introduction

[Mémento Python](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3.pdf){:target="_blank"}

## Votre tout premier programme

Lors de ces travaux pratiques, vous allez écrire des petits programmes Python sur l’IDE **Thonny** qui est déjà installé sur les machines de l’école.

Voici un exemple d’un tout petit programme en Python qui ne contient qu’une seule instruction:
```python
print("bonjour")
```
En anglais, "print" signifie “imprime". En Python, l’instruction `print` demande à l’ordinateur d’afficher à l’écran le contenu de la parenthèse qui vient après.

> ### <span style="background-color:#c6d9f7"> Exercice 1 </span>
>
> Ecrivez et exécutez le programme ci-dessus sur `Thonny`.  
> Changez le texte pour que l’ordinateur écrive autre chose, par exemple "au revoir !".  
> Sauvegardez le fichier exercice1.py dans votre dossier personnel.

## Les commentaires

Il est souvent utile de mettre des commentaires dans un programme, pour expliquer ce qu’il fait.
En Python un commentaire est introduit par le caractère \#. 
**Tout ce qui vient après et jusqu’à la fin de la ligne n’est pas lu par l’ordinateur**.
Cela sert uniquement à l’humain qui va lire le programme.
```python
# un tout petit programme
print("bonjour") # salutations
```

> ### <span style="background-color:#c6d9f7"> Exercice 2 </span>
> 
> Enlevez les guillemets autour de "bonjour". Qu’est-ce qui se passe ?
> 
> <details><summary markdown="span">Solution</summary>
> 	Le programme n’est plus compris par la machine car si "bonjour" était un texte pouvant être affiché sans problème, bonjour désigne une variable ayant pour nom bonjour.
> 	Cette variable n’existant pas au moment de son appel, l’ordinateur ne sait pas quoi afficher. Du texte s'écrit toujours entre guillemets ou apostrophes ("" ou '').
> </details>

## Exercices Turtle (facultatif)

`turtle` est un module Python permettant de faire du **dessin en codant**. La tortue peut se déplacer et dessiner une trace avec les 4 fonctions:
1. `forward(d)` pour avancer d’une distance `d` (en pixels).
2. `backward(d)` pour reculer.
3. `left(a)` pour tourner à gauche d’un angle `a` (en degrés).
4. `right(a)` pour tourner à droite

Ce code permet de dessiner un carré, testez-le !
```python
import turtle # Importe le module

turtle.forward(100) # Avance de 100 pixels
turtle.left(90) # Tourne a gauche de 90 degres
turtle.forward(100)
turtle.left(90)
turtle.forward(100)
turtle.left(90)
turtle.forward(100)
turtle.left(90)

turtle.done() # Termine le dessin
```
Si vous êtes curieux, la plateforme [Modulo](https://apprendre.modulo-info.ch/prog1/dessiner.html) propose beaucoup d’autres exemples et exercices dans son chapitre **Programmation**.

> ### <span style="background-color:#A8D6C2"> Exercice Turtle 1 </span>
>
> Ecrivez un programme qui dessine un triangle équilatéral avec chaque côté ayant une longueur de 100 pixels. (Rappel : chaque angle d’un triangle équilatéral fait 60 degrés).


---

[Retour à l'accueil](../README.md)