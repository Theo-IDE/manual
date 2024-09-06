# User Manual
This repository contains the source code of the user manual for the Theo-IDE and it's libraries. This file contains 
instructions on how to obtain the manual as a pdf document.

## Prerequisites

This user manual was written using  [ConTeXt LMTX](https://wiki.contextgarden.net/Installation) `>= 2023.04.01 09:52`. 
The fonts we used are:

- STIX Two Text
- STIX Two Math
- Inter
- JetBrains Mono

These fonts need to be installed on your system, and the environment variable `OSFONTDIR` needs to point to the folder
containing your fonts. On linux you should add `export OSFONTDIR=$HOME/.local/share/fonts:/usr/share/fonts`
to your `.bashrc` configuration. The STIX fonts are included in ConTeXt.

Verify that you installed the fonts correctly with:
```bash
mtxrun --generate
mtxrun --script font --reload
```

## Compiling
Having installed ConTeXt and the required fonts, you will be able to compile a pdf document using the following command:
```bash
$ context prd_user_manual.tex
```
