# University of Aveiro Thesis

## Document PDF

O documento em pdf está na pasta /build



## Usage

Optional: In debian and ubuntu you can install all dependencies automatically:

```
make setup
```

Build a development version of the document:

```
make [build]
```

Continuously build the development version of the document:

```
make preview
```

This option is great when paired with a document viewer (such as Okular) which
automatically reloads the document on file change. This means you can keep
writing and on save the updated document is compiled and displayed!

Build versions of the document for publishing:

```
make print
make ebook
```

Run linters (for now only [proselint](http://proselint.com/)) against a TeX
file (e.g. chapter 1):

```
make lint [texfile=chapter1.tex]
```

If you do not specify the `texfile` to lint, then all TeX files in `chapters/`
will be linted.

Clean the build directory:

```
make clean[all]
```

`clean` will leave the output products (the PDFs) in place, while `cleanall`
will remove these too. If your document is not compiling for some reason and
you think you've already solved the problem in the LaTeX sources, maybe try a
`cleanall` before insisting. Sometimes the underlying build programs (namely
`latexmk`) get stuck in inconsistent temporary files.

## Authors

Tomás Oliveira e Silva created the [original
template](http://sweet.ua.pt/tos/TeX/ua_thesis.tgz) which was later picked up
by João Paulo Barraca who [improved and maintained it for
years](http://code.ua.pt//projects/latex-ua/repository).


