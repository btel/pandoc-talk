default: slides.pdf

slides.pdf: slides.md template/header.tex template/beamer.pandoc
	pandoc -t beamer -H template/header.tex --template=template/beamer.pandoc --filter=pandoc/pandoc-svg.py --latex-engine=xelatex $< -o $@
