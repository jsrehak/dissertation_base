# Dissertation Base

This is a template directory for writing and compiling a dissertation
using the required UC Berkeley dissertation class. The main reason for
the automation is to enable you to build only one chapter of the
thesis at a time (for easier reviewing by committee members). Chapters
should be placed in the `chp` folder (if they are elsewhere the
Makefile won't find them) and an `\include{chp/new_chapter}` statement
added to `thesis.tex`. Now using `make new_chapter` will only make the
specified chapter, or `make thesis` will make the whole thesis.

## Dependencies
- LaTeX ([TeX Live](https://www.tug.org/texlive/) recommended)
- `make`
- `biber`
- `qpdf`: PDF manipulation software (comes installed with Ubuntu)

Note: `biber` is not installed by default in Ubuntu, you need to
install it using:
```
sudo apt-get install texlive-bibtex-extra biber
```
