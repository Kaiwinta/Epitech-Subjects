## AutoDoc

Ce projet à pour but d'automatiser la création de README au norme de **Studio-17**

- [AutoDoc](#autodoc)
- [Requirements:](#requirements)
- [Execution](#execution)
- [Help du projet:](#help-du-projet)
- [Structure des sujets:](#structure-des-sujets)

## Requirements:
-

- Tkinter
- Selenium
- Pyperclip

*cf requirements.txt* 

## Execution

Il ya 4 mains différents en fonction du type de dossier à documenter, 
il faut bien faire attention à selectionner un dossier valide et du même type que le main


Lors de l'ouverture de la page web, ne rien faire

**Les types de README sont:**
- **Project**:
  - Le temps de travail
  - La taille du groupe
  - Les tests de MRVN
- **Module**:
  - Les détails du module de l'intra
  - Les détails de chaque projet (temps et nom)
- **Semestre**:
  - La liste des Modules du semestre et leurs crédits
  - La liste de projet dans chaque module
- **Global**:
  - La liste des Semestre
  - La liste des modules de chaque Semestre et leurs crédits

## Help du projet:
-

```
Usage:
    ./auto_doc.py -b e -url https://my.epitech.eu/index.html#d/2023/B-CPE-110/organized/5979804 -cp

Arguments:
    -b      => choix du Browser entre Edge (e) par défault, Chrome (c) et Firefox (f)
    -url    => url d'une mouli du projet / Module
    -p      => nombre de personnes sur le projet
    -t      => temps en semaines pour le projet
    -cp     => écriture du readme dans le clipboard

Permet de créer un Readme qui suis les normes établies
```

## Structure des sujets:

- Le Repo est composé de plusieurs semestres avec chacun un README.md

- Chaque semestre contient un ou plusieurs modules qui ont tous un README.md

- Chaque module contient plusieurs dossiers qui sont des projet et qui ont un README.md

- Chaque projet peut contenir n'importe quoi, si il y a un Bootstrap, il doit être dans un dossier dans le projet

Exemple d'un module dans un Semestre:

📂---Semestre-1

ㅤㅤ|\_\_\_Module-1

ㅤㅤㅤㅤ|\_\_\_Projet-1

ㅤㅤㅤㅤㅤ  |\_\_\_Bootstrap

ㅤㅤㅤㅤㅤㅤㅤㅤ|\_\_\_Fichier_Example.pdf

ㅤㅤㅤㅤㅤ  |\_\_\_Projet

ㅤㅤㅤㅤㅤㅤㅤㅤ|\_\_\_Fichier_Example.pdf

ㅤㅤㅤㅤㅤ  |\_\_\_**README.md** (Readme du projet avec les units tests)

ㅤㅤㅤㅤ|\_\_\_Projet-2

ㅤㅤㅤㅤㅤ  |\_\_\_Fichier_Example.pdf

ㅤㅤㅤㅤㅤ  |\_\_\_**README.md** (Readme du projet avec les units tests)

ㅤㅤㅤㅤ|\_\_\_**README.md** (Readme du Module avec la liste des projets, leurs durée et les détail de l'intra)

ㅤㅤ|\_\_\_**README.md** (Readme du Semestre avec la liste des Module et de chacun de leurs projets)

|\_\_\_**README.md** (Readme du Repo avec tout les Semestre et tous les modules)

---

Les PR et les issues sont les bienvenues en cas de problème ou de suggestion


Ce projet à été fait par [@Kaiwinta](https://github.com/Kaiwinta)