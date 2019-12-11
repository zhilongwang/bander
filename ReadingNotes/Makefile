
default: pdf

PAPER = week3
JUNK = *.ps *.dvi *.log *.out *.aux *.backup *~ *.blg *.bbl *.toc

# Define the tools we are going to use

# Rules for various parts of the target
pdf: $(PAPER).tex
	pdflatex $(PAPER).tex
	bibtex  $(PAPER)
	pdflatex $(PAPER).tex
	pdflatex $(PAPER).tex
	rm -f $(JUNK)

clean:
	rm -f $(JUNK) $(PAPER).pdf
