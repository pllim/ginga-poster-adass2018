#
# Photography Book Makefile
# Eric Jeschke  2009-07-04
#
# Pass environment variables to sub-make's
#.EXPORT_ALL_VARIABLES

FIGUREs = figures/*

all: poster

poster: poster.pdf

poster.pdf: poster.tex $(FIGUREs)
	xelatex poster.tex 
	#pdflatex poster.tex 

bib:	poster.bib
	bibtex poster

sweep:
	-/bin/rm *~ *.out *.aux *.log *.bbl *.blg \#*\#

clean: sweep
	-/bin/rm *.pdf 

# END
