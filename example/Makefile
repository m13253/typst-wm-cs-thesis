.PHONY: all clean

all: example.pdf example.svg

clean:
	$(RM) example.pdf example.svg

%.pdf: %.typ %.bib
	typst compile --root .. --font-path ../fonts $< $@

%.svg: %.typ %.bib
	typst compile --root .. --font-path ../fonts --pages 1 $< $@
