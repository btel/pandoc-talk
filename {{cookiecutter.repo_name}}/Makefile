default: {{cookiecutter.repo_name}}.pdf

{{cookiecutter.repo_name}}.pdf: {{cookiecutter.repo_name}}.md template/header.tex template/beamer.pandoc
	mkdir -p build
	pandoc -t beamer -H template/header.tex --template=template/beamer.pandoc --filter=pandoc/pandoc-svg.py --latex-engine=xelatex $< -o $@
