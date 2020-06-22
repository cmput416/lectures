all:
	pdflatex paper < /dev/null
	bibtex -min-crossrefs 99 paper < /dev/null
	pdflatex paper < /dev/null
	grep Citation *.log; true
	grep Reference *.log; true
	grep Label.*multiply *.log; true
#	pandoc coverletter.txt -o coverletter.pdf

clean:
	rubber --clean -d paper
