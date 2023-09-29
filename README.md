# iut_bash_2023
## titre2
### titre 3
un test en **gras** et en *italique*

- item 1
- item 2
  - sous titre
  - sous item
 
    
1. pizza
2. eau
3. glace
ls montre tous les fichier
cd =change directory
cd ..  revient d'un en arriere
## 1.2
### cd : change directory
- `cd <nom_dossier>` : permet de se déplacer dans un dossier enfant
- `cd` : permet de se déplacer dans son home, repéré par le ~
- `cd ..` : permet de remonter dans le dossier parent
### ls :list
-  `ls ` : permet d'afficher la liste des dossiers et fichiers du dossier actuel

## 1.3
- `cat <nom_fichier>` permet de lire le contenue d'un fichier
`print('salut')`
- <kbd> tab </kbd> : autocomplétion du début d'une commande

## 1.4 chemin relatif et absolue
  double tab montre les fichiers d'un dossier
`../` : permet d'aller dans le dossier parent 

    ce que sont les dossiers / et ..
    ce qu'est un chemin (absolu ou relatif)
    ce qu'est le répertoire courant,
    des exemples de commandes et d'arguments
    comment lister les fichiers présents dans le dossier courant en utilisant la commande ls sans argument.
    comment lister les fichiers présents dans un dossier en utilisant la commande ls suivi d'un chemin relatif ou absolu vers un dossier.
    comment te déplacer en donnant comme argument à la commande cd soit un chemin relatif soit un chemin absolu.
    comment voir le contenu d'un fichier avec la commande cat suivi d'un chemin relatif ou absolu vers un fichier.

## 1.5 mkdir
echo repete ce qu'on lui donne, ondoit separer les arguments par un espace
mkdir créé un fichier
les mots commençant par _ sont des options et le autres de arguments
Le double tiret : les options ainsi signalées le sont en version longue.

[liens vers le killercoda](https://killercoda.com/emelin)

jghgjghj
  ## séance2
  nano 'chemin' ->vers un fichier
  ouvre un editeur de fichier
  commande ^s -> sauvegarder
           ^x -> supprime
  
  mkdir "repertoire"
  créer un dossier
  mkdir -r /usr/machin/truc/bidule
  -r recursive  mkdir test1 test2 test3 test4 : creer 4 dossiers

  touch 'chemin vers un fichier'
  Permet de mettre à jour l'heure et la date d'un fichier
  si l'emplacement est inexistant de alors ca va creer un fichier vide

  rm 'chemin vers un plan'
  supprime un fichier
  **rm -r efface tout l'ordi**
   rm -r 'chemin vers le dossier'
   --recursive  -> efface tous les dossiers et fichiers enfants du chemin spécifié

   du 'chemin vers un dossier'
   =disk usage -> permet de connaitre la taille d'un repertoire

   rm -r tavail/
   __    _______
   option   argument


   du -s 'dossier'
      ___
      summarize
      (somme)
fait la somme de l'espace disque utilisé du -h 'dossier'

-- humain-readable
affihe la taille avec une unité plus facile à lire
taille de votre home

du -h /home/toto
- du -h ~
taille du fichier

bit ->0 ou 1
octet ->8 bits
Ko (kilo octet) 1000 octets
Mo
Go
To

  
### killercoda séance 3
- mv permet de deplacer un fichier(La commande mv permet également de renommer un fichier. Par exemple : mv john.snow commandant renommera john.snow en commandant .)   
- chmod permet de donner des perm. c'est à dire: ugo:+ou/:rwx
(u=user,g=groupe,o=other,r=read,w=write,x=execute)


- --------- se traduit par 0 en octal en fonction de ce qui est marqué( si ca commence par un - c que c'est un fichier, si d c'est u dossier, l pour un lien) 
