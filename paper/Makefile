FILE=paper/training_deep_boltzmann_machines



all: $(FILE).pdf
.PHONY: all

.PHONY: clean
clean:
	rm -f *.aux *.blg *.out *.bbl *.log *.pdf

$(FILE).pdf: $(FILE).tex paper/dbm.bib
	pdflatex $(FILE)
	pdflatex $(FILE)
	bibtex $(FILE)
	pdflatex $(FILE)
	pdflatex $(FILE)
	bibtex $(FILE)
	pdflatex $(FILE)
	pdflatex $(FILE)

