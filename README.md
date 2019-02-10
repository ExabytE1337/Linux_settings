# My Linux Settings
Get linux mint from https://www.linuxmint.com/download.php

Make a bootable usb i.e. with Rufus https://rufus.ie/

Theme vimix-dark from https://github.com/vinceliuice/vimix-gtk-themes

Paper icon theme from https://github.com/snwh/paper-icon-theme

Configure non-system disks to automount.

Configure timeshift.

Apps from APT:
* atom
* redshift
* calibre
* gpick
* libreoffice
* inkscape
* pychess
* qBittorent
* TeXStudio
* Rhytmbox
* Spotify
* VLC

Get NVIDIA proprietary drivers.

# Atom and packages needed for Markdown, etc.
One Dark theme and syntax works best for mutliple languages.

Packages:
* Hydrogen
* atom-csv-markdown
* atom-language-r
* document-outline
* language-markdown
* language-matlab
* markdown-pdf
* markdown-scroll-sync
* markdown-table-editor
* markdown-writer

Themes: - right now they don't work for markdown
* dracula-syntax
* dracula-ui


# R, RStudio and packages
Get RStudio from https://www.rstudio.com/products/rstudio/download/#download

Get the newest R-language from
https://cran.r-project.org/
for mint 19.1 it was by adding
``` deb https://cloud.r-project.org/bin/linux/ubuntu bionic-cran35/``` to your /etc/apt/sources.list file.
Maybe you will need to run
```sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9``` I don't remember.
Then run ```sudo apt-get update sudo apt-get install r-base``` and ```sudo apt-get install r-base-dev``` .

Install tidyverse by first installing
```sudo apt install libcurl4-openssl-dev libssl-dev libxml2-dev```.

# CLI based software

Install neofetch by running ```sudo apt install neofetch```. Source is on https://github.com/dylanaraps/neofetch/wiki/Installation.

Install cmatrix by running ```sudo apt-get install cmatrix```.
Use ctrl+c to exit matrix.

# Python, Anaconda and spyder
