# Des commandes en plus dans le terminal

```
terminal
csv2ssv
dedup
mkv2mp4
ogg2mp3
wav2mp3
xls2ssv
ssv2tsv
```

## terminal

`terminal` : Met à jour `terminal`, affiche les informations d'installation et les commandes disponibles. 

## dedup

`dedup fichier1 [fichier2]` : créé un fichier avec les emails dans `fichier1` [mais pas dans `fichier2`]. 

Les doublons et les adresses invalides sont isolés dans un repertoire `fichier1_dedup` créé à coté de `fichier1`.

### Option `-d`
Dédupliquer en fin de processus avec les fichiers `$liste_rouge` définis dans `desinscrits.config`.

```
liste_rouge="chemin/vers/liste_rouge.csv"
liste_rouge2="chemin/vers/autre_liste_rouge.csv"
```


## ...


# Installation avec Git

Dans le terminal taper la première fois :
```
git clone https://github.com/BoOz/terminal.git
cd terminal
chmod +x install.sh
./install.sh
```

Suivre les indications à l'écran pour ajouter `terminal` au PATH.

# Mise à jour 
```
terminal
```

# ajout au PATH
```
# ajouter des commandes au shell (MAMP + terminal)
export PATH=$PATH:/Applications/MAMP/Library/bin:la/ou/est/terminal
```

# Dépendances

Sous MacOSX installer préalablement :
- xcode (depuis l'appstore) pour avoir Git et SVN

## Homebrew et cask
Press Command+Space and type Terminal and press enter/return key.
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null ; brew install caskroom/cask/brew-cask 2> /dev/null
```

## les commandes unix oubliées par MacOSX
`brew install coreutils`

# Autres commandes utiles

## Installer homebrew et cask
Press Command+Space and type Terminal and press enter/return key.
```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)" < /dev/null 2> /dev/null ; brew install caskroom/cask/brew-cask 2> /dev/null
```

# Apache / PHP / Mysql
./APACHE_MYSQL_PHP.md

## csv kit
```
sudo pip install csvkit
```
http://csvkit.readthedocs.io


## Conversion HTML => Rtf
```
textutil -convert rtf -inputencoding utf-8 test.txt -output NewFileName.rtf
```

## table2csv : récuperer un tableau HTML en csv
pip install -U table2csv
table2csv http://en.wikipedia.org/wiki/List_of_Super_Bowl_champions > dump.txt

## generer une cle ssh
```
ssh-keygen -b 4096
```
puis entrée à chaque prompt

## enregistrer un access ssh sur un serveur distant
```
brew install ssh-copy-id
ssh-copy-id user@server.net
```

## barre de progression
```
brew install pv
```
## config mysql
`vim .my.cnf`

