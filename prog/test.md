# Introduction

## Mise en place

1. Synchronisez votre compte OneDrive sur l'ordinateur
2. Ouvrez l'application `Thonny`

[Mémento](https://perso.limsi.fr/pointal/_media/python:cours:mementopython3.pdf){:target="_blank"}

## Exemple 1

Voici un exemple d’un tout petit programme en Python qui ne contient qu’une seule instruction:
```python
print("bonjour")
```
En anglais, "print" signifie “imprime". En Python, l’instruction print demande à l’ordinateur d’afficher à l’écran le contenu de la parenthèse qui vient après.

## Exercice 1

Ecrivez et exécutez le programme ci-dessus sur `Thonny`.
Changez le texte pour que l’ordinateur écrive autre chose, par exemple "au revoir !"

## Exemple 2

Il est souvent utile de mettre des commentaires dans un programme, pour expliquer ce qu’il fait.
En Python un commentaire est introduit par le caractère \#. 
Tout ce qui vient après et jusqu’à la fin de la ligne, n’est pas lu par l’ordinateur.
Cela sert uniquement à l’humain qui va lire le programme.
```python
# un tout petit programme
print("bonjour") # salutations
```

### Multiplication

Que va imprimer le programme suivant ?

```python
a = 6
b = 7
print(a * b)
```

<details><summary markdown="span">Solution</summary>

```bash
42
```

</details>

1. Sur l'éditeur `Thonny`, copiez ce programme et enregistrez-le sous `/OneDrive - Education Vaud/informatique/tp-11/multiplication.py`
2. Pour exécuter le programme, cliquez sur le bouton vert ▶ et le résultat s'affichera dans la `console` en bas de la fenêtre
3. Pour vérifier votre programme, allez sur [le vérificateur](https://gymnase-checker.onrender.com/?exercises=multiplication,circle_perimeter){:target="_blank"} et téléversez le fichier sur l'application sous le bon exercice

Sauvegardez les prochains exercices dans le dossier `/OneDrive - Education Vaud/informatique/tp-11/` avec le nom donné. 
Puis vérifiez votre résultat sur [le vérificateur](https://gymnase-checker.onrender.com/?exercises=multiplication,circle_perimeter){:target="_blank"}. 

### Périmètre d'un cercle

Complétez le programme `circle_perimeter.py` suivant :

```python
PI = 3.14
rayon = 7
perimetre = ...

print(perimetre)
```

<details><summary markdown="span">Solution</summary>

```python
PI = 3.14
rayon = 7
perimetre = 2 * PI * rayon

print(perimetre)
```

</details>

## Saisie & Conversion

[Vérificateur](https://gymnase-checker.onrender.com/?exercises=hello,age){:target="_blank"}

### Bonjour

Ecrivez un programme `hello.py` qui demande à l'utilisateur son nom puis qui lui répond `Bonjour, <nom> !` :

```
Comment vous appelez-vous ? John
Bonjour, John !
```

<details><summary markdown="span">Solution</summary>

```python
nom = input("Comment vous appelez-vous ? ")
print(f"Bonjour, {nom} !")
```

</details>

### Âge

Ecrivez un programme `age.py` qui demande à l'utilisateur son année de naissance puis qui lui répond `Vous avez <age> ans cette année !` :

```
Quelle est votre année de naissance ? 2006
Vous avez 16 ans cette année !
```

<details><summary markdown="span">Solution</summary>

```python
annee = int(input("Quelle est votre année de naissance ? "))
print(f"Vous avez {2022 - annee} ans cette année !")
```

</details>

## Exercices Papier

Voir les exercices distribués. 

---

[Retour à l'accueil](../README.md)