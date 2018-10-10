DOC	= paper

paper:	
	latex $(DOC)
	latex $(DOC)
	bibtex $(DOC)
	latex $(DOC)
	dvips -Ppdf $(DOC).dvi
	ps2pdf14 $(DOC).ps

bundle:
	tar czf $(DOC).tar.gz $(DOC).tex $(DOC).bib $(DOC)_f*.eps $(DOC).pdf

clean:
	/bin/rm *.bbl *.aux *.blg *.dvi *.log *.ps *.pdf *.out

