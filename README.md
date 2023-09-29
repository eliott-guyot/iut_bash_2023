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
  - rm -r 'chemin vers le dossier'
   - --recursive  -> efface tous les dossiers et fichiers enfants du chemin  spécifié
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
### chmod 
- chmod permet de donner des perm. c'est à dire: ugo:+ou/:rwx
(u=user,g=groupe,o=other,r=read,w=write,x=execute)
 ca s'ecrit chmod ... nomDuFichier
### droit
- --------- se traduit par 0 en octal en fonction de ce qui est marqué( si ca commence par un - c que c'est un fichier, si d c'est u dossier, l pour un lien) 
- les 3 premier - correspondent à user, groupe, autres
- en generale pour un fichier txte normal les droit normaux sont -rw-r(w)-r--
### nano
- permet de modifier le contenu d'un fichier
### man
- man + commande(donne le mannuel de la commande)

### cp
- cp permet de copier un ou des fichiers vers un endroit donné(ca s'ecrit: pc nomdufichier endroitdepose)
- ./ affiche le contenue d'un fichier
### utiliser mv
- #!/bin/bash (ouvre un interpreteur)
- mv peut deplacer un fichier mv /home/toto/truc.txt /temp/
- mv peut deplacer un repertoire mv /home/toto/docs/  /temp/
- mv peut renomer un fichier mv /home/toto/truc.txt /home/toto/machin.txt 
### utiliser cp
- cp copie un fichier dans un autre repertoire
cp /home/toto/truc.net /temp/
- cp copie un fichier dans un meme repertoire
cp /home/toto/truc.txt /home/toto/truc.back
- copier dans le meme repertoire
 cp truc.txt machin.txt
- copier plusieurs fichier
 cp fichier1 fichie2 ficher3  /tmp/
- echo $(variable) nous donne le contenu de la var
- quand on a un espace dans une reponse/nom il faut mettre des "" pour ne pas que ca soit vu comme un arg
### echo$fichier
- lance le fichier
### ./
represente la ou on est
### nano affectation
nomdevar=$(qqc)
### nano affichage
echo "texte"+ (si jamais $nomdevar)

### remplir premiere ligne nano (shebang)
#!/bin/bash
pour savoir ou est l'interpreteur mettre dans le term "which bash"
### fichier
- appleler ses fichier scrpit avec .sh a la fin
- lui ajouter des droits d'execution(chmod)(chmod (u/g/o+r/w/x) nomdufichier)
- pour executer le script :  ./nomdufichier.sh
(./ représente la ou on est)
### control+shift
selectionne plusieurs lignes
