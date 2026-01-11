# ds-uzh-aedl-LaTeX
This is a personal (non-official) LaTeX template that can serve as your starting point for writing papers and theses at the Deutsches Seminar (DS) of the University of Zurich (UZH).

It is configured to follow the [rules and guidelines of the Ältere deutsche Literaturwissenschaft](https://www.ds.uzh.ch/de/studium/master/info_masterstudium/merkblaetter.html) as close as possible.

This LaTeX template has been created from and adapts the [template for BA and MA theses](https://www.cl.uzh.ch/en/studies/studies-BA-MA/wegleitung.html) at the Institute of Computational Linguistics of the UZH.

## Getting Started

To get started with this template, download the code as a ZIP file from the GitHub repository.

**Using Overleaf**: Upload the ZIP file directly to Overleaf and begin editing your document in the browser.

**Working locally**: Extract the ZIP file and work locally using the editor and TeX distribution of choice. This template uses `biblatex` with the `biber` backend for bibliography management.

The compilation sequence is:
```bash
pdflatex thesis.tex  # First pass: creates citation markers
biber thesis         # Processes bibliography from thesis.bib
pdflatex thesis.tex  # Second pass: incorporates bibliography
pdflatex thesis.tex  # Third pass: finalizes references and page numbers
```

Most modern LaTeX editors (VS Code with LaTeX Workshop, TeXShop, etc.) handle this automatically. If you see `[?]` for citations, ensure biber is run as part of your build process.
