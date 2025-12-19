# Default target
all: 04-classification/04-classification.csv 05-resampling/05-resampling.csv

# 04 Classification
04-classification/04-classification.csv: 04-classification.tex 04-classification.pdf
	latex2anki 04-classification.tex

04-classification.pdf: 04-classification.tex
	latexmk -pdf $

# 05 Resampling
05-resampling/05-resampling.csv: 05-resampling.tex 05-resampling.pdf
	latex2anki 05-resampling.tex

05-resampling.pdf: 05-resampling.tex
	latexmk -pdf $

# Clean up auxiliary LaTeX files
clean:
	rm -f *.aux *.fls *.log *.fdb_latexmk *.paux *.gz
