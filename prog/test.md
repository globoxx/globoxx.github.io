# Introduction

[Mémento](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3.pdf){:target="_blank"}

### Exemple 1

Voici un exemple d’un tout petit programme en Python qui ne contient qu’une seule instruction:
```python
print("bonjour")
```
En anglais, "print" signifie “imprime". En Python, l’instruction print demande à l’ordinateur d’afficher à l’écran le contenu de la parenthèse qui vient après.

### <span style="background-color:#c6d9f7"> Exercice 1 </span>

Ecrivez et exécutez le programme ci-dessus sur `Thonny`.
Changez le texte pour que l’ordinateur écrive autre chose, par exemple "au revoir !"

### Exemple 2

Il est souvent utile de mettre des commentaires dans un programme, pour expliquer ce qu’il fait.
En Python un commentaire est introduit par le caractère \#. 
Tout ce qui vient après et jusqu’à la fin de la ligne, n’est pas lu par l’ordinateur.
Cela sert uniquement à l’humain qui va lire le programme.
```python
# un tout petit programme
print("bonjour") # salutations
```

### <div style="background-color:#c6d9f7"> Exercice 2

Enlevez les guillemets autour de "bonjour". Qu’est-ce qui se passe ?

<details>
	<summary markdown="span">Solution</summary>
	Le programme n’est plus compris par la machine car si "bonjour" était un texte pouvant être affiché sans problème, bonjour désigne une variable ayant pour nom bonjour.
	Cette variable n’existant pas au moment de son appel, l’ordinateur ne sait pas quoi afficher. **Du texte s'écrit toujours entre guillemets ou apostrophes ("" ou '')**.
</details>

</div>
---

[Retour à l'accueil](../README.md)