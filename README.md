# Research Software Engineering Methods Talk

![pdf](https://github.com/davidwilby/ResearchSoftwareMethods/actions/workflows/build_presentation_pdf.yml/badge.svg)

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
#### Locally
In the folder location where you would like to build the presentation pdf, run:
```sh
git clone https://github.com/davidwilby/ResearchSoftwareMethods
cd ResearchSoftwareMethods
pdflatex presentation.tex
```
This should build the presentation to `./presentation.pdf`

#### Automated on GitHub
Tagged commits are automatically built and associated with a release; the built pdf is attached to the release as an asset.
You can see the workflow for doing this in [`.github/workflows/`](/.github/workflows)

## Contributing
Contributions and improvements are very welcome! Please fork this repo and make a pull request against the `main` branch.
Please ensure that your document compiles successfully with the instructions above.
