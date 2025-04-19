# LaTeX template for 3rd and 4th year project reports in physics at Imperial College London

This repository contains a LaTeX template for writing reports for the 3rd and 4th year projects in physics at Imperial College London. The template is based on the official requirements by the department as of April 2025. It is designed to be used with Visual Studio Code and the LaTeX Workshop extension, but it should work with any LaTeX editor.

## Getting started

To get started and set things up for you, just search the repository for the keyword `TODO` and follow the instructions. The most important things to do are:
- Set up your name and student number in the `main.tex` file.
- Set up the bibliography file `bibliography.bib` with your references. You can use a citation manager like Zotero to do this. The template uses the `biblatex` package for citations.
- Set up the `assets` directory with your images. The template uses the `graphicx` package for including images.
- Set up the `main.tex` file with your content. The template uses the `input` command to include the different sections of the report. You can add or remove sections as needed.

## (Optional) Some conventions and tips to follow in LaTeX:

- The **language** used throughout the document should be British English. (Tip: Enable spell checking in VSCode and set in to `en-GB`.)
- To reference other parts of the document, **labels** should always be used. They should be of the format `\label{<type>:<section>:<name>}` where:
    - `<type>` is one of:
        - `sec` for sections (including subsections and subsubsections)
        - `fig` for figures
        - `tab` for tables
        - `eq` for equations
    - `<section>` is one of:
        - `intro` for the introduction
        - `part1` for part I
        - `part2` for part II
        - `conclusions` for the conclusion
        - `bib` for the bibliography
        - `part<i>-app<n>` for appendix `<n>` in part `<i>`
    - `<name>` is a descriptive name for the label (this should be in lowercase and use hyphens (`-`) instead of spaces or underscores). This should only be obmitted if the label is for a section.
- **Image files** should be stored in the `assets` directory. Filenames should be of the format `<section>-<name>.<extension>` where:
    - `<section>` is one of:
        - `intro` for the introduction
        - `part1` for part I
        - `part2` for part II
        - `conclusions` for the conclusion
        - `part<i>-app<n>` for appendix `<n>` in part `<i>`
    - `<name>` is a descriptive name for the image (this should be in lowercase and use hyphens (`-`) instead of spaces or underscores).
    - `<extension>` is the file extension (e.g. `png`, `jpg`, `pdf`, etc.). For matplotlib plots, the extension should be `pdf` to ensure that the plots are vector graphics.
- **Citations** should be done using the `biblatex` package. The command `\autocite{<citation-key>}` should be used. The bibliography should be stored in the `bibliography.bib` file; it should be generated using a citation manager (e.g. Zotero) and should be in BibTeX format. 
- **Commit messages** should be in the present tense and should be concise. They should be of the format `Add <section>` or `Update <section>`.
- During the process of writing, **todo notes** can be added to the document using the `\todo{<note>}` command. An overview of all todo notes is displayed after the contents section.