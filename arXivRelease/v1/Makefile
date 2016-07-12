ALL: finalPaper.pdf

%.pdf: %.tex Makefile
	pdflatex $(<:.tex=) && bibtex $(<:.tex=) && pdflatex $(<:.tex=) && pdflatex $(<:.tex=)
	rm -f $(<:.tex=Notes.bib)
#	pdflatex $< && bibtex $(<:.tex=.aux) && pdflatex $< && pdflatex $<


clean:
	rm -f *.aux *.bbl *.blg *.log  *.nav *.out *.snm *.toc

sclean: clean
	rm -f finalPaper.pdf
