# Slides for Research Software Engineering Methods Talk

## Building the slides
### Depencencies
#### LaTeX
This talk is written in LaTeX, so to build the slides from source, you will need a LaTeX distribution. I've tested with `pdflatex` on Ubuntu 18.04. It should also build using other distributions and on other operating systems, but I have not tested this myself.

For Ubuntu, install the TexLive base:
```sh
sudo apt-get install texlive-latex-base
```

Optionally, install more fonts:
```sh
sudo apt-get install texlive-fonts-recommended
sudo apt-get install texlive-fonts-extra
```

And extra packages:
```sh
sudo apt-get install texlive-latex-extra
```

#### Beamer
The `Beamer` documentclass is used for formatting a presentation in LaTeX, most distributions should support this.

#### Slide theme - Metropolis
Instructions for building the slide theme are here: https://github.com/matze/mtheme

### Build Instructions
#### Clone this repo
In the folder location where you would like to build the presentation pdf, run:
```sh
git clone https://github.com/davidwilby/ResearchSoftwareMethods
cd ResearchSoftwareMethodsTalk
pdflatex presentation.tex
```
This should build the presentation to `./presentation.pdf`
