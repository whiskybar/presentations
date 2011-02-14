SOURCES=Presentation.pdf

all: clean $(SOURCES)

clean:
	rm -f *.pdf

%.pdf: %.rst
	rst2pdf -b1 -s slides.style $<
