DOC	= P11-3

paper:
	latex $(DOC)
	latex $(DOC)
	bibtex $(DOC)
	latex $(DOC)
	dvipdf $(DOC).dvi

bundle:
	tar czf $(DOC).tar.gz $(DOC).tex $(DOC).bib $(DOC)_f*.eps $(DOC).pdf

clean:
	/bin/rm *.bbl *.aux *.blg *.dvi *.log *.ps *.pdf *.out
