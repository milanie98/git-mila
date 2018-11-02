## 2.Installer git
---
#### 2.1 Introduction 

Ce cours t'introduira à Git et Github, deux fantastiques outils qui permettent de faire des sauvegardes efficaces d'un projet, et de travailler à plusieurs sur le même dossier.

Dans cette leçon, nous allons te montrer comment installer Git, comment s'en servir , et comment le faire marcher .
Pour ceci, nous allons nous aider de l'excellent [openclass](https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-githubsur)
OpenClassrooms de Marc Gauthier; sur Git et Github

 ####  2.1.1 Ce que tu vas apprendre dans cette ressource 

 #### 2.2 Historique 

 Git est un outil de versonning c=de code , c'est à dire que c'est une commande qui permet de faire des sauvegardes , avec commentaires d'un projet. Ainsi, il est facile de revenir d'une version de sauvegarde à l'autre, et c'est même optimisé pour les projets où tout le monde travaille sur le même fichier !

 En gros , c'est la même chose quand vous faîtes une grosse présentation PPT. Vous faites tellement de modifications dessus que vous retrouvez à la fin avec le nom "VF_avec8retours_jeans01_final.ppt". Le versonning vous permet d'avoir toutes les versions sauvegardees, et de revenir à celles que vous voulez à tout moment, et de nous éviter ces tracas. 

 Voilà à quoi Git sert : à mieux gérér ses versions entre les fichiers d'un projet ( bonus :Git marche pour tous les fichiers d'un dossier concerné , donc c'est encore plus puissant que  
 `<CTRL>` + `<S>`. t Github permet de mettre en ligne ton projet , comme ça vous pourrez travailler facilement  en équipe dessus.

 Pour information , Git a été crée en 2005 par Linus Torvald , qui ( entres autres) crée le système d'exploitation Linux.

 ## 2.3 Le Cours 
 ---

 2.3.1 Installer Git

 Avant de pouvoir se servir de Git , il faut l'installer . Cela tombe bien , il y a [chapitre ](https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github/2433596-installez-gi)
 dans le cours sur OC.

 2.3.2 Première introduction à Git 

 j'ai fait une petite vidéeo d'introduction à Git , que tu pourras retrouver ci-bas [THP-Git/GitHub](https://www.youtube.com/watch?time_continue=5&v=ggaMadCKjko )
 Ensuite tu peux suivre le cours de Marc Gauthier jusqu'à la partie [Récupérez des modifications](https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github/2433686-recuperez-des-modifications). Nous verrons dans la formation THP  comment faire les branches et autres joyeusetés :) 

 ## 2.4 Points importants à retenir
 ---

#### 2.4.1 les commandes pratiques 

Voici un récap des commandes de base : 

* `[$ git init]` : il faut TOUJOURS commencer git avec cette commande , le répértoire courants est considée comme un repository git 

* `[ $ git add [fichier]]` : ajoute aux sauvegardes le fichier metionné **Protip**: si tu as plussieurs fichiers à ajouter , tu peuxutiliser `[git add]` qui ajoute au repisotory tous les fichiers du dossier

* `[$git commit -m][commentaire]` : crée un commit ( commit = sauvegarde suivie d'un commentaire).

* `[git status]` : te dit le status actuel de git . 

#### 2.4.2 Lire l'historique et de voir tous les commits. Les commits sont rangés avec : 

* SHA : liste de chiffres et lettres qui identifient de façon unique le commit.
* Auteur
*Date
*Message donné durant el commit : avec ce message , tu vas comprendre ce que faisait le commit. C'est pour cela qu'il est important df'avoir un bon nom . 

##### **Pour quitter le loog il faut appuyer sur `[Q]`

#### 2.4.3 Se positionner sur un commit donné 

#### **Imaginons que veut vous voulez vérifier un truc sur un vieux commit. On va utiliser la commade `[ $ git checkout]`, utilsée comme ceci :

* `[$ git checkout 45581cebd2cae494f80f44010af9e4a86c9b8fa]`: on dit à git de se positionner sur ce sha précis

* `[$ git master checkout master] ` : une fois que l'on a fini de se balader , il faut revenir à la version présente de notre repository avec cette commande

#### ALERTE ERREUR COMMUNE 
---
`[git checkout]` ne marche que si u n'as pas de modification non sauvegardée. Si tu est entre deux commits , git checkout ne marchera pas . Du coup il te faudra soit faire une sauvegarde (== faire un commit) soit effacer tout pour revenir au commit d'avant.

`[$ git checkout]` n'est pas une commande pour revenir en arrière et faire des modifications sur les anciens commits. Si tu fais ça , tu vas te retrouver avec une erreur qui a donné [l'un des treads](https://stackoverflow.com/questions/5772192/how-can-i-reconcile-detached-head-with-master-origin) les plus célèbres de Stack Overflow . Pour tout effacer et revenir en arrière , le chapitre suivant sera là pour toi.

#### 2.4.4 Revenir en arrière 
---
J'ai fait des trucs , mais cela ne me convient pas . Comment revenir en arrière ? (inspiré par [cette excellente](https://stackoverflow.com/questions/4114095/how-to-revert-a-git-repository-to-a-previous-commit/4114122#4114122) réponse de Stack Overflow)

#### 2.4.1.1 Effacer pour revenir au commit d'avant
---

`[ $ git reset-- hard ]` permet de reveir au commit précédent , en effaçant tout. C'est une commande pratique quand on veut essayer de nouvelles choses à la volée, puis de revenir en arrière comme si de rien n'était (smiley)

#### 2.4.4.2    Tout effacer et revenir à un ancien commit
---

On peut faire ceci avec `[ $ git reset --hard 45581cebdd2cae494f80f44010af9e4q86c9b8fa]`
,avec 45581c le SHA sur lequel tu veux revenir.

#### 2.5 Pour aller plus loins
---
 Au vu des apologies que l'on lui donne, [le cours de OpenClassrooms](https://openclassrooms.com/fr/courses/2342361-gerez-votre-code-avec-git-et-github) sur Git est un très bon point pour aller plus loins . Il explique notamment la notion de branches et de fusions.
 
  Aussi , voici un [cours](https://www.vikingcodeschool.com/web-development-basics/getting-to-know-git) sur Git de la Viking Code School . Il explique bien les bases de Git et est une bonne alternative au notre.



