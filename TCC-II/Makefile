# $Id: Makefile,v 1.1 2003/04/10 23:12:59 gweber Exp $

all: TCC-II.ps TCC-II.pdf

TCC-II.dvi : TCC-II.tex
	latex TCC-II
	bibtex TCC-II
	latex TCC-II
	latex TCC-II
	
TCC-II.ps: TCC-II.dvi
	dvips -t a4 -o TCC-II.ps tese
	
TCC-II.pdf: TCC-II.dvi
	pdflatex TCC-II

clean:
	rm -f *.aux *.log *.blg *.bbl *.dvi *.ps *.pdf *.toc *.lot *.lof *~
