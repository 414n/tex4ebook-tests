.PHONY: clean distclean all default PDF epub tikz tikz-clean tex4ebook tex4ebook2 epub-check

default: all

all: tex4ebook 

clean:
	latexmk -C

tex4ebook: clean
	tex4ebook -t -c conv2html.cfg -e my_filters.mk4 test.tex

PDF: clean
	latexmk -xelatex test.tex