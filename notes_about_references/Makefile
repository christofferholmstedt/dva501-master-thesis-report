
all:
	pdflatex main.tex
	makeindex main.nlo -s nomencl.ist -o main.nls
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
	rm -rf *.lof
	rm -rf *.lot
	rm -rf *.out
	rm -rf *.toc
	rm -rf *.nls
	rm -rf *.nlo
	rm -rf *.ilg
