.PHONY: clean

manuscript.tex: manuscript.md
	pandoc manuscript.md -o manuscript.tex

manuscript-plos.pdf: manuscript-plos.tex
	latex manuscript-plos
	bibtex manuscript-plos
	latex manuscript-plos
	latex manuscript-plos
	dvipdf manuscript-plos
clean:
	rm -f *~
	rm -f manuscript-plos.aux
	rm -f manuscript-plos.bbl
	rm -f manuscript-plos.blg
	rm -f manuscript-plos.dvi
	rm -f manuscript-plos.log
	rm -f manuscript-plos.out
	rm -f manuscript-plos.tex.pdf
	rm -f manuscript.tex

