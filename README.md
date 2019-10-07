# My Linux Settings

Get linux mint from [mint](https://www.linuxmint.com/download.php)

Make a bootable usb i.e. with Rufus [rufus](https://rufus.ie/)

Theme vimix-dark from [vimix](https://github.com/vinceliuice/vimix-gtk-themes)

Theme nordic with standard buttons from [nordic](https://www.cinnamon-look.org/p/1267246/)

Paper icon theme from [paper](https://github.com/snwh/paper-icon-theme)

Configure non-system disks to automount.

Configure timeshift don't include documents and files.

Apps from APT:
*  redshift
*  calibre
*  gpick
*  libreoffice
*  inkscape
*  pychess
*  qBittorent
*  TeXStudio
*  Texlive-full
*  Rhytmbox
*  Spotify
*  VLC

Get NVIDIA proprietary drivers. Add the ppa to get the newest one. Don't install the binary ones, just the metapackage.
Still need to figure out how to actually make it run on startup but `nvidia-settings --assign GPULogoBrightness=0` turn off the gpu led's.

# Atom and packages needed for Markdown, etc.

One Dark theme and syntax works best for mutliple languages.

Packages:
* Hydrogen
* atom-csv-markdown
* atom-language-r
* document-outline
* language-markdown
* markdown-pdf
* markdown-table-editor
* markdown-writer
* markdown-preview-enhanced(disable the original markdown-preview)
* language-matlab
* pigment

# R, RStudio and packages

Get RStudio from [stable](https://www.rstudio.com/products/rstudio/download/#download) or a preview from [preview](https://www.rstudio.com/products/rstudio/download/preview/)

# RStudio custom theme

get it here [atom_theme_custom](https://github.com/ExabytE1337/Linux_settings/blob/master/atom.rstheme)
and this one too [nord one dark](https://github.com/ExabytE1337/Linux_settings/blob/master/nord_one.rstheme)

# RMarkdown custom theme

Combine the file markdown.css, atom_one_dark.css to one css that will be used inside the document.
Use highlight: zenburn to get the code highlight working for now. We will have to dig a bit deeper to adjust the colors of functions and words the same as used in the atom_one_dark.css.

**Easy to incorporate into RMarkdown just use YAML**

```r
---
title: "Sample title"
output:
  html_document:
    df_print: paged
    css: one_dark_simple.css
---
```

## Uninstall RStudio - to reinstall it ofcourse

sudo apt-get remove rstudio

Get the newest R-language from
[cran](https://cran.r-project.org/)
for mint 19.1 it was by adding
``` deb https://cloud.r-project.org/bin/linux/ubuntu bionic-cran35/``` to your `/etc/apt/sources.list` file.
Maybe you will need to run

```
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E084DAB9
sudo apt-get update sudo apt-get install r-base
sudo apt-get install r-base-dev
``` 

Install tidyverse by first installing
```sudo apt install libcurl4-openssl-dev libssl-dev libxml2-dev```.

Add the atom.rstheme to RStudio. Preferably to Rstudio/resources/themes.
This will import the One Dark theme. Use the one that is in this repository. I changed the .ace_operator to make it distinguishable from other functions.

# CLI based software

Install neofetch by running ```sudo apt install neofetch```. Source is on [neofetch](https://github.com/dylanaraps/neofetch/wiki/Installation).

Install cmatrix by running ```sudo apt-get install cmatrix```.
Use ctrl+c to exit matrix.

# Python, Anaconda and spyder
