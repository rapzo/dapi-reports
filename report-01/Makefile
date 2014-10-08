#
# Version:   Wed Sep 10 10:47:40 2014
# Written by JCL
#

## Basename for result
TARGET=report-01

latexmk:
	latexmk -pdf -bibtex -recorder -pvc $(TARGET).tex

## Extensions
EXTS=aux toc idx ind ilg log out lof lot lol bbl blg brf tdo ffs wtf bbl brb

##clean
clean:
	for EXT in ${EXTS}; do \
	  find `pwd` -name \*\.$${EXT} -exec rm -v \{\} \; ; done

### misc
.SUFFIXES: .tex .aux .toc .lof .lot .log .dvi .dvi2 .ps .ps2 .pdf .bib .bbl
