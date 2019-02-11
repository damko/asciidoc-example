AsciiDoc is a lightweight markup language for authoring notes, articles, documentation, books, web pages, slide decks and man pages in plain text.

It's similar to _markdown_ but much more powerful, standardized and complete but not much more complicated.

The file `source.adoc` contains some `asciidoc examples` taken from the reference guide. 

The file `asciidoc_examples.pdf` is the rendeerd output of the source file.

## References:

* https://asciidoctor.org/docs/user-manual/[complete user manual]
* https://asciidoctor.org/docs/asciidoc-syntax-quick-reference/[quick syntax reference]
* https://asciidoctor.org/docs/asciidoc-writers-guide/[getting started user guide]


## How to install asciidoctor on Debian

Asciidoctor is a convenient application or rendering asciidoc files in different formats

    sudo apt install asciidoctor ruby-asciidoctor

## Rendering

This document can be rendered in different ways:

. as _article_ in *PDF* format with the following command:
+
----
asciidoctor-pdf -d article source.adoc -o asciidoc_examples.pdf
----

. as _book_ in *PDF* format with the following command:
+
----
asciidoctor-pdf -d book source.adoc -o asciidoc_examples.pdf
----

or you could add this to the header of the document and lose the `-d` option:

----
:doctype: book
----
