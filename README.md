# EXERCICE n°3 :

Vous allez créer un nouveau projet sur votre dépot git.
Vous allez appeler votre projet “exercice3”.
***Attention :***
>Sur Github notre branch main correspondra à la branche main


***solution :***
>*Se rendre sur [Github](https://github.com) ou [Gitlab](https://about.gitlab.com/) est creer un nouveau repository (public) avec le nom exercice3*


Ci-dessous les étapes à effectuer :

● En local, vous allez créer un projet que vous allez appeler exercice3.

***solution :***
>Création du dossier exercice 3 et utilisation des commandes fournit par github pour lié notre repo local à notre repo distant
```
mkdir exercice3
echo "# exercice1" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin https://github.com/nom_utilisateur_github/exercice1.git
git push -u origin main
```

***Indice :***
● Dans cet exercice, vous aurez besoin d’utiliser :
○ git branch “nom de la branche” : pour créer une branche dans votre projet.
○ git checkout “nom de la branche” pour vous déplacer vers une branche.


● Vous allez créer un fichier texte qui va s’appeler “fichier_branche_master” et qui va contenir le texte, “bonjour, je suis le fichier de la branche master”.
● Vous allez ensuite pousser ce fichier sur votre dépôt distant sur la branche “master”.

***solution :***
>Création du fichier et envoi sur le repo distant
```
echo " bonjour, je suis le fichier de la branche main. " >> fichier_branche_main.txt
git add .
git commit -m "création du fichier branche main"
git push -u origin main
```

● Vous allez ensuite créer une branche que vous allez appeler avec “votre prenom” (avec la commande git branch).

***solution :***
>Création de la branch
```
git branch prenom
```

● Vous allez vous positionner sur cette branche (en utilisant la commande git checkout “nom de votre branche”).

***solution :***
>Positionnement sur la branch
```
git checkout prenom
```

● Vous allez créer un nouveau fichier qui va s’appeler“fichier_branche_votre_prenom”et qui va contenir le texte, “bonjour, je suis le fichier de la branche votre prenom”.

***solution :***
>Création du fichier
```
echo « bonjour, je suis le fichier de la branche votre prenom". » >> fichier_branche_votre_prenom.txt
git add .
git commit -m "création du fichier branche prenom"
```

● Vous allez ensuite pousser ce fichier sur votre dépot distant mais sur votre nouvelle branche “votre prenom”.

***solution :***
>Push de la nouvelle branch local sur le repo distant
```
git push -u origin prenom
```

A la fin, vous aurez, 2 branches, et chacune de ces branches devraient contenir un seul et unique fichier.

***solution :***
>Pour cela il nous faut supprimmer le fichier_branche.txt en etant positionner sur la branch prenom et mettre a jour nos repo
```
git chekout prenom
rm fichier_branche_main.txt
git add .
git push -u origin prenom
```

