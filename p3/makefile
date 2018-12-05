binaries = $(wildcard *.pdf) $(wildcard *.log) $(wildcard *.aux) $(wildcard *.nav) $(wildcard *.out) $(wildcard *.toc) $(wildcard *.vrb) $(wildcard *.snm) $(wildcard *.pyg)

deps = style logos images

tex = $(wildcard *.tex)

pres.pdf: $(deps) $(tex)
	pdflatex -synctex=1 -interaction=nonstopmode --shell-escape $(tex)

.PHONY: clean 

clean: 
	rm -rf $(binaries) *.sty $(deps) 

style: $(wildcard ../include/*.sty)
	cp ../include/*.sty ./

logos: $(wildcard ../include/logos/*)
	cp -r ../include/$@ $@

images: $(wildcard ../include/images/*)
	cp -r ../include/$@ $@
