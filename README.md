![](https://img.shields.io/badge/licence-MIT-green?style=flat-square)
![](https://img.shields.io/badge/language-LaTeX2e-blue?style=flat-square)

# Minimal-CV (forked from [minimal-cv](https://github.com/FMatti/Minimal-CV/tree/main))
Minimal template for typesetting a curriculum vitae (CV) in LaTeX.

## Introduction
This is my fork of [minimal-cv](https://github.com/FMatti/Minimal-CV/tree/main) made by [FMatti](https://github.com/FMatti).

## Features
Some of the main features that characterize this template are the
- coherent and consistent design language
- programmatically generated vector icons and flags
- tunable color scheme
- extendability for personal use

Added Features with this fork:
- font awesome support
- SVG support
- enhanced tables management
- greek letters support 

### SVG

To enable SVG support, on VS code you have to enable shell escape. Visit [this link](https://github.com/James-Yu/LaTeX-Workshop/wiki/FAQ#how-to-pass--shell-escape-to-latexmk) 

- go to `settings` 
- search `latex-workshop.latex.tools`
- edit the json adding `-shell-escape` in the `arg` section:
    ```json
    ...
    "args": [
                "-shell-escape",
                "-synctex=1",
                "-interaction=nonstopmode",
                "-file-line-error",
                "-pdf",
                "-outdir=%OUTDIR%",
                "%DOC%"
            ],
    ...
    ```

### Icons
[FMatti](https://github.com/FMatti) designed a set of vector illustrations that can be used as icons to guide the eye of the reader towards the relevant information.
![icons](https://user-images.githubusercontent.com/79205741/177930763-1178f46a-04bb-4347-9a1e-90a9e47f435a.svg).

My adaptation can use images from [Font Awesome](https://fontawesome.com/).

### Flags
A small set of flags can be used to make your language competences visible at a glance.
![flags](https://user-images.githubusercontent.com/79205741/177930857-f0c5ae05-6d3a-4d51-9f67-2ad911b33a7c.svg)

### Color schemes
Custom color schemes can be quite easily added to the default design to personalize the CV.
| Default | Blue | Green | Red |
:-------------------------:|:-------------------------:|:-------------------------:|:-------------------------:
![minimal-cv-black](https://github.com/FMatti/Minimal-CV/assets/79205741/2270e68f-8f2a-4e4f-9f6a-1e82de8c57ad) | ![minimal-cv-blue](https://github.com/FMatti/Minimal-CV/assets/79205741/5c48a543-455c-4a5a-b0a9-640c94fb53ff) | ![minimal-cv-green](https://github.com/FMatti/Minimal-CV/assets/79205741/ce27e5c8-3c7c-4225-badc-e617dee9909e) | ![minimal-cv-red](https://github.com/FMatti/Minimal-CV/assets/79205741/6806cf3c-dde8-4755-90a5-1f09d44a7681)

## Usage
To build a pdf version of the CV simply run the following commands:

    git clone https://github.com/FMatti/Minimal-CV.git
    cd Minimal-CV
    pdflatex Minimal-CV.tex
