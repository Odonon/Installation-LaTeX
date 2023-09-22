# Installation LaTeX

## Sous Windows
Pour l'installation sur Windows, suivre installation_latex_windows.pdf.

## Sous Ubuntu (ou autre distro *debian based*)
### Par le gestionnaire de paquet *apt*
Pour une installation basique sur Ubuntu, je vous renvoie sur le lien suivant https://doc.ubuntu-fr.org/utilisateurs/sssammm/installer_texlive
Cette installation se fait par le gestionnaire de paquet *apt*. Le principal avantage est qu'il contient une installation **extrêmement** stable de texlive. L'inconvénient est donc que cette installation n'est pas totalement à jour (en général elle est mise à jour tous les 2 ou 3 ans). Par ailleurs, en passant par cette méthode, l'installation des éditeurs comme *Texstudio* est simplifiée. Il suffit de l'installer via le gestionnaire de paquet:
```
apt install texstudio
```

### Par l'archive de texlive
Si vous souhaiter une installation sur une distribution *debian-based* à jour et sans compromis de texlive, télécharger l'archive .tar sur ce lien :
http://mirror.ctan.org/systems/texlive/tlnet/install-tl-unx.tar.gz
Puis taper les lignes de code suivantes en les adaptant au dossier où l'archive à été télécharger:
```
cd /path/to/download/
tar -xf install-tl-unx.tar.gz
cd /path/to/extracted/tar
sudo ./install-tl
```

__ATTENTION :__ Pour installer Texstudio, il est nécessaire d'ajouter l'option `no-install-recommends` pour éviter une double installation de Texlive et donc des problèmes:
```
apt --no-install-recommends install texstudio
```

### Ajout de la variable dans le *path* (Linux uniquement)
Pour pouvoir utiliser votre installation toute neuve de texlive il est nécessaire d'ajouter le dossier d'installation à votre variable d'environnement `$PATH`. Pour se faire, plusieurs méthodes, je vous renvoie à votre meilleure recherche Google pour trouver votre bonheur.

## Installation sous ArchLinux
Pour une installation sur ArchLinux, je vous renvoie à l'AUR sur le wiki de Arch https://wiki.archlinux.org/index.php/TeX_Live | je conseille une installation manuelle, le dépôt sur pamac semble entrer en conflit avec certaines installations des éditeurs comme TeXStudio et Texmaker depuis le manager.

# Tutoriels
Pour démarrer, quelques sites avec d'excellents tutoriels ou base de données d'exemples :
- [LearLaTeX][https://www.learnlatex.org/fr/] : un tutoriel complet avec des exercices pour débutants
- [TeXample][https://texample.net/] : une base de données d'exemples de figures dessinées avec TikZ ou pgfplots
- [LaTeX Cookbook][https://latex-cookbook.net/] : un livre de recettes pour faire beaucoup de belles choses avec LaTeX
- [Forum TeXchange][https://tex.stackexchange.com/] : le graal lorsque l'on a une question ou une erreur inexpliquée

