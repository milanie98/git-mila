## 1. Cours sur le terminal

---
### 1.1 introduction
Dans cette ressource, tu vas découvrir les bases du terminal, un outil très puissant qui permet de "parler" à son ordinateur. Nous allons voir les bases : comment intéragir avec le terminal, comment jouer avec ses premiers fichiers, et bien d'autres.

#### 1.1.1 Ce que tu vas apprendre dans cette ressource

Voici la liste des questions auquelles tu vas pouvoirs répondre avec cette ressource :

* Qu'est-ce que le terminal ?

* Que veut dire GUI et CLI ?

* Comment lancer un terminal ?

* Comment exécuter ses premières fonctions avec un terminal ?

* Pourquoi la notion de géographie est très importante dans un terminal ?

* Qu'est-ce que VIM et comment s'en servir ?

### 1.2 Historique

Le terminal est ce que l'on appelle plus communément un interpréteur de commande (ou command-line interpreter (CLI) en anglais), est un outil qui permet d'interpréter les commandes qu'un utilisateur tape au clavier dans l'interface en ligne de commande.

 A la base, les ordinateurs tournaient sanss interface graphique, donc les utilisateurs passaient exclusivement par les CLI. Avec l'arrivée des système d'exploitation graphiques ( Windowns , Apple , Linux), le CLI n'a pas perdu en popularité , puisqu'il permet de faire des tâches extrêmement précises. 

 En gros, c'est une version texte de l'explorateur de fichier: on peut ouvrir des dossiers , créer des fichiers, les lancer; les renommer; installer des programes , et bien d'autre choses. On dit que c'est une **CLI** ( Command Line Interface) , comparée à la **GUI** (Graphical User Interface) de l'explorateur normal. Tout est fait via clavier , donc pas besoin de souris dans le terminal.

 ### 1.3 Le terminal

 #### 1.3.1 Qu'est ce que le terminal ?

Le terminal est un outil intimidant aux premiers abords, mais au final se rélève pas compliqué . J'ai réalisé une vidéo qui explique le terminal : [Introduction au terminal](https://www.youtube.com/watch?v=myz_6xrDwR4&feature=youtu.be) 

### 1.3.2  Comment le lancer ?
Sur Linux : `[CTRL]` + `[ALT]`+ `[T]`

Sur macOS : `[CMD]`+ `[SPACE]` , puis écrire `[Terminal]` ( ou iTerm), Enter

### ALERTE BONNE ASTUCE 

Si tu utilises Linux ,passe ton terminal en anglais . Quand ce dernier te renverra une erreur , c'est bien mieux qu'elle soi e anglais . L'anglais de la landue d'internet , donc la majorité des gens qui ont eu ton peoblèmz vont le poster en anglais . Et ainsi tu auras 100 fois plus de résultats sur Google que si tu postais ton erreur en français.

### 1.3.3 Premières fontions ?

Pour faire marcher le terminal , rien de plus : il suffit de rentrer le texte correspond à la fonction et cela s'exécutera . Par exemple si dans l'explorateur en GUI il suffit de double cliquer sur `[mon_fichier.txt]` pour l'ouvrir , il faudra faire dans le terminal `[open mon_fichier.txt]` (sur macOS) ou `[xdg-open mon_ fichier.txt]` ( sur Linux) pour l'ouvrir avec le terminal. On va tester avec notre première fonction :

 `[ $ echo "Hello word !"`

 (Je commence toutes les commandes du terminal avec `[$]` c'est une convention, et c'est plus facile à reconnaitre comme ceci)

 Si tu exécutes cette commande le terminal devrait te renvoyer `[Hello world !]` ( cette phrase est un [grand classique de la progammation](https://fr.wikipedia.org/wiki/Hello_world))
 Et là , tu viens d'exécuter ta première commande de terminal . Maintenant nous allons voir les premières commandes de base.

 ### 1.3.3.1 PWD

 `[pwd]` est l'acronyme de Print Workin Directory , une commande qui affiche le dossier dans lequel tu es actuellement.

`[$ pwd]` 

Pour moi `[pwd]` me renvoie : `[Users/felix/]`
c'est comme dans l'explorateur en GI , qund tu double-cliques sur `[felix]` , il te déplace dans le dossier`[felix]` qi est dans le dossier `[Users]`

### ALERTE BONNE ASTUCE 

`[pwd]` est génralement la première commande que l'on tape quand on arrive dans le terminal de quelqu'un : c'est idéal pour s'y retrouver 
 
 ###
 1.3.3.2 LS

`[ls]` est le diminutif le dimunitif pour _list_ , cette fonction ffiche les fichiers et dossiers qu'ils y'a dans mon dossier actuel.

`[$ ls]`

Pour moi `[ls]` me renvoie : 

` [ Applications/                     Dropbox/           Music/     Desktop/      Pictures/           Documents/      Library/      Public/     Downloads /       Movies/   ]`

Dans le terminal , nous pouvons donner des otions aux fonctions , en faisant `[ $ fonction-option]` . Par exemple , je peux faire  `[ls - a]` , ce qui a pour effet d'afficher aussi les fichiers commençant par un `[.]` ( fihciers de devs en général), ou je peux même combiner les deux en faisant `[ls-al]`
Pour afficher aussi les fichiers commençant par un `[.]`, tout au format long.

### 1.3.3 MAN

`[man]`est le diminutif de _manual_. Man lance un programme qui permet de lire le manuel d'une fonction précise . Pratique pour savoir toutes ses spécificités . Pour s'en servir il suffit de tapper : `[man fonction`]` . Par exemple pour afficher le manuel de ls, je dois taper :

`[ $man ls ]

Ce qui m'ouvrira son manuel , qui je peux quitter ç tout moment en tapant `[q]` 

### 1.3.4 Ou somme- nous ?

Une notion **fondammentale$$ pour le terminal : la notion de géographie . Comme dans l'explorateur en GUI , on se déplace , on se déplace de dossiers dans le terminal. Si jamais tu veux ouvrir un fichier en tappant  `[open file.txt]`
( sur macOS) ou ` [xdg-open file.txt]` ( sur linux) et que tu ne te retrouve pas dans le bon dossier , le terminal te renverra une erreur. Un peu comme si tu essayais de double-clique su file.txt dans le mauvais dossier : impossible car il n'y est pas.

Tu vas devoir te déplacer donc de dossiers en dossiers pour ouvrir et interagir avec les bons fichiers. 

### 1.3.5 CD 
`[cd]` est l'acrononyme de Change _Directory_, qui te permet de naviguer entre dossiers. L'équivalent d'un double clic sur un dossier en quelque sorte 

`[ $ cd nomdudossier]`

Tu te déplaceras dans le dossier nommé `[nomdudossier]`
(S'il existe dans le dossier dans lequel tu te trouves).

Tu peux aussi te déplacer vers le dossier parent en faisant `[ $cd ..]`

##ALERTE BONNE ASTUCE 

Utiliser  la touche `[TAB]` permet de faire de l'autocompletion, très pratique pour cette méthode . Aussi, faire `[cd]` + [ ESPACE] + `[TAB]+ [TAB]
affiche les dossiers disponibles 

## 1.3.6 Autres fonctions 

### 1.3.6.1  Créer un fichier

En tapant : 

`[ touch nomdufichier]`
Cela aura effet de créer un ficier qui s'appelle nom _dufichier_

### 1.3.6.2  COPIER 

Pour copier un fichier ou un dossier d'un endroit à un autre, il suffit de rentrer : `[cp fichier_à_copier lieu_de_destination]` 

### 1.3.6.3
Pour déplacer (couper) un fichier ou un dossier d'un endroit à un autre, il suffit de rentrer :
 `[mv [fichier_à_déplacer]lieu_de_destination]

 **Protip** : `[mv]` est très pratiquetrès pratique pour renommer un fichier. Imaginons que tu as créé un fichier "hello.rv" au lieu de "hello.rb". Oups, malheur.Heureusement, faire `[$ mv hello.rv]` `[hello]` résoud ceci en quelques coups de clavier !

 ### 1.3.6.4 Remove
 Supprimer un fichier : `[$ rm nomdufichier]`


Il est possible d'effacer un dossier ainsi que son contenu en ajoutant la récursion en option : `[rm -r nomdufichier]`

### INSTANT DE CULTURE GE 
`[rm]`est à l'origine d'une blague vieille comme le monde. En effet, ajouter l'option `[-f]` permet de forcer la suppression d'un fichier, même s'il est important pour l'ordinateur, et finir par`[/]`ou `[*]`dit à votre ordinateur de prendre absolument tous les fichiers. Ainsi, si tu tapes `[$ rm -rf /]` ou `[rm-rf *] dans ton terminal, tu dis à ce dernier de tout prendre et de tout effacer, en forçant. Et figure toi que rm est très rapide, et donc effacera l'intégralité de ton ordinateur en quelques secondes à peine.** A ne jamais jamais jamais faire donc.

### 1.3.6.5 Vim 
Vim est un des éditeurs de texte les plus respectés au monde. Comme il passe uniquement par le terminal, il se marie extrêmement bien avec cet outil. Et comme vim utilise exclusivement le clavier, ses raccourcis permettent d'aller extrêmement vite, pour qui ose grimper la très dure courbe d'apprentissage (quelques semaines à plein temps). De ce fait, je te montrerai vim pour ta culture générale, mais te demanderai de passer par un autre éditeur de texte. 
`[$ vim nomdufiichier]`

Permet d'ouvrir vim sur le fichier nom _dufichier_ et de l'éditer. Pour quitter vim, il faut rentrer `[:q!]`.

### 1.3.7.Autres astuces  

`[CRTL]`+ `[C]` annule la fonction en couts. Pratique quand on a une boucle infinie.

La casse est très importante , idem pour les espaces.

Il y a des raccourcis pratiques , par exemple `[CRTL]` + `[U]` efface la ligne en cours.

Les touches du haut et du bas permettent de naviguer dans l'historique des commandes. Très pratique pour par exemple re-éxécuter une commande que tu viens de faire

### 1.4 . Les points importants** 

Voici les points à retenir de la source : Voici les points à retenir de la ressource :
* Pour lancer le terminal sur Linux : 
`[CTRL]`+ ` [ ALT]` + `[T]` : pour le lancer sur macOS : `[CMD]+ `[SPACE]`
, puis écrire  `[Terminal]` ( ou iTerm), Enter.

* `[man]` est le manuel des fonctions
* `[pwd"]` affiche le dossier dans lequel tu es actuellement .
* `[ls]` est une commande qui affiche les fichiers et dossiers qu'il ya dans mon dossiers actuel.
* la notion de géographie est fondamentale : le terminal n'arrivera pas à ouvrir les fichierssi'il ne se trouve pas dans le bon dossier
*`[cd]` permet de changer de dossier 
*`[touch]` permet de créer un fichier
*`[cp]` permet de copier un fichier
*`[mv]` permet de déplacerun fichier ou un dossier
*`[rm]` permet de supprimer un fichier 

### 1.5 Aller plus loins

Voici un excellent [cours express](https://www.vikingcodeschool.com/web-development-basics/a-command-line-crash-course) pour avoir quelques base, sur le terminal. Il est un peu similaire au mien, mais aborde d'autres sujets intéressants tels que que le PATH.

Viking code school ont aussi fait [cours sur le pimp de terminal](https://www.vikingcodeschool.com/web-development-basics/a-command-line-crash-course) pour avoir plein de couleurs de BGs sur le tien .

Michael Harti a fait une célèbre introduction au terminal nommée [Learn enough Command Line To Be Dangerous](https://www.learnenough.com/command-line-tutorial). Cette ressource permet d'aller assez loins en détails dans le terminal .








