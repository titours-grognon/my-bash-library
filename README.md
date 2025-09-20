# 🎉 **MY-BASH-LIBRARY** 🎉

- [🎉 **MY-BASH-LIBRARY** 🎉](#-my-bash-library-)
  - [Objectifs 🚩](#objectifs-)
  - [Personnalisation du shell *Bash*](#personnalisation-du-shell-bash)

## Objectifs 🚩

- personnaliser le comportement du shell *Bash* du terminal
- base d'exécution d'un script *Bash*
- ensemble de « librairies » associé

## Personnalisation du shell *Bash*

Copier le répertoire `.bash-files` à la racine du répertoire personnel :

```cmd
cp .bash-files ~/.
```

Ajouter la condition suivante au fichier `~/.bashrc` :

```cmd
if [ -f ~/.bash-files/module ]
then
  source ~/.bash-files/module
  echo -en "$(__style FG_GREEN BOLD)--- Custom configuration loaded ---\n$(__style)"
fi
```

> Note :
>
> Il est possible de modifier le comportement de la navigation dans le terminal via le fichier `~/.inputrc`.
>
> Pour aller plus loin :
>
> - [Readline EN](https://www.gnu.org/software/bash/manual/html_node/Readline-Init-File.html)
> - [Linux From Stratch EN](https://linuxfromscratch.org/lfs/view/stable/chapter09/inputrc.html)
> - [Linux From Stratch FR](http://fr.linuxfromscratch.org/view/lfs-12.4-fr/chapter09/inputrc.html)
