DOC = memoria.tex
OUT = memoria.pdf
BIB = bibliografia.bib
SRC = memoria.tex portada.tex introduccion.tex planificacion.tex

all: $(OUT)

$(OUT): $(SRC) $(BIB)
	pdflatex $(DOC)
	bibtex $(basename $(DOC))
	pdflatex $(DOC)
	pdflatex $(DOC)

clean:
	rm -f *.aux *.bbl *.blg *.log *.toc *.out *.lof *.lot *.synctex.gz *.pdf
