AsciiDoc is a lightweight markup language for authoring notes, articles, documentation, books, web pages, slide decks and man pages in plain text.

It's similar to _markdown_ but much more powerful, standardized and complete but not much more complicated.

The file `source.adoc` contains some `asciidoc examples` taken from the reference guide. 

The file `asciidoc_examples.pdf` is the rendered output of the source file.

If you click on `source.adoc` here in this repo you see the live *HTML* rendering performed by Github. 

If you want to see the raw text source, click [here](https://raw.githubusercontent.com/damko/asciidoc-example/master/source.adoc)

Github supports asciidoc inside any repo and inside the Wiki but not inside Github Pages (because the jekill plugin for asciidoc is not supported, somehow)

## References:

* [complete user manual](https://asciidoctor.org/docs/user-manual/)
* [quick syntax reference](https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/)
* [getting started user guide](https://asciidoctor.org/docs/asciidoc-writers-guide/)


## How to install asciidoctor on Debian

Asciidoctor is a convenient application or rendering asciidoc files in different formats

    sudo apt install asciidoctor ruby-asciidoctor ruby-asciidoctor-pdf

## Rendering

This document can be rendered in different ways:

* as _article_ in *PDF* format with the following command:


``` bash
asciidoctor-pdf -d article source.adoc -o asciidoc_examples.pdf
```

* as _book_ in *PDF* format with the following command:


``` bash
asciidoctor-pdf -d book source.adoc -o asciidoc_examples.pdf
```

or you could add this to the header of the document and lose the `-d` option:

``` bash
:doctype: book
```

When the document is rendered in the *PDF* format the images are embedded in the document.