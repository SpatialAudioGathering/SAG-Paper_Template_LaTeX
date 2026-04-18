# SAG Paper Template LaTeX

This repository includes the LaTeX template for paper and short papers presented at SAG - Spatial Audio Gathering conference. The LaTeX class suppoting the template and the default content were created from scratch by Enrico Dorigatti specifically for SAG, and do not rely on existing code.

The template is the same for long and short papers, and is organised as a one-column document, specifically aimed at improving readability.

For consistency reasons, only a LaTeX template is provided, in place of the usual Word + LaTeX combination. However, the template can be opened and edited in OverLeaf, in place of a local LaTeX instannation, making the entire process straightforward.

## Text in the template

The template comes already filled with:

- title
- abstract
- list of mock authors
- main text: it explains how to use the template and introduces LaTeX to the newcomers, explaining and demonstrating the main commands. Expert LaTeX users can remove it and start to fill it immediately with their data. However, LaTeX newcomers are strongly encouraged to familiarise with the main commands and the best practices
- elements such as lists, tables, and pictures. The `images` folder contains a `placeholder.pdf` which is used as a sample image. Do not remove the folder unless you're sure you will not use images in your document. It is nevertheless suggested to simply remove the sample image from the text
- references: the `bibliography.bib` file contains some mock entries which are used to demonstrate how to reference sources

Again, LaTeX newcomers are strongly encouraged to familiarise with the main commands and their use through the text filling the template by default.

## Composition of the package

Within the .zip package containing the template, you'll find:
- an `images` folder, where you can add your own images–inside, there's a `placeholder.pdf` file used as a sample image
- a `bibliography.bib` containing some mock bibliographic entries in the BibTeX format. You can get rid of those, and you must use that file to add the entries of the sources you cite
- a `SAG_SubmissionTemplate.tex` file. This is the main document, where you have to write your own content
- a `sag.sty` file. This is the class supporting the correct functioning of the template, *DO NOT TOUCH IT!*

## Anonymity

Please note that the `sag.sty` class supporting this template accepts an optional argument when recalled. When you recall it, you can either:
- recall it through `\usepackage{sag}`: this loads the default class to compile the document as-is. Use this option for he Camera-Ready version of your contribution (non-anonymous)
- recall it through `\usepackage[anonymous]{sag}`: the optional argument _anonymous_ in square brackets tells the class to hide real names, institutions, and other personal data of the authors both in the first page and the headers. Use this options if your have to anonymise your contribution, such as when submitting it for peer-review
