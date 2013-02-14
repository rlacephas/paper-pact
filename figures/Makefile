
FIGURES = rerange \
	foo-10 \
	foo-1000 \
	cp-overview \
	pathnorm \
	valprof \
	denormalize \
	motivate \
	smoothing

FIGS = $(FIGURES:=.fig)
PDFS = $(FIGURES:=.pdf)
EPSS = $(FIGURES:=.eps)

.SUFFIXES : .fig .eps .pdf

#smoothing.eps: smoothing.fig
#	fig2mpdf -e -H header.tex $<

.fig.eps:
	fig2mpdf -l -e -H header.tex $<

.eps.pdf:
	epspdf $<

all: pdf eps

pdf:	$(PDFS)

eps: $(EPSS)

clean:
	rm *~ *cls

list:
	@echo "FIGURES = $(FIGURES)"
	@echo "PDFS = $(PDFS)"
	@echo "EPSS = $(EPSS)"