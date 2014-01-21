
all:
	pdflatex main.tex
	bibtex main.aux
	pdflatex main.tex
	pdflatex main.tex

clean:
	rm -rf *.aux
	rm -rf *.bbl
	rm -rf *.blg
	rm -rf *.log
	rm -rf *.spl
	rm -rf *.pdf
