#UNAME := $(shell uname -o)

#default:    paper.tex
#	@echo "cd img ; make ; cd .. ; latex paper ; bibtex paper ; latex paper ; latex paper ; dvips -P pdf -t letter -Pdownload35 -o paper.ps paper.dvi ; ps2pdf -dPDFSETTINGS=/prepress -dSubsetFonts=true -dEmbedAllFonts=true -dMaxSubsetPct=100 -dCompatibilityLevel=1.3 paper.ps paper.pdf" | at now > /dev/null 2>&1

all:	paper.tex
#ifeq ($(UNAME),Cygwin)
#	@echo "Not available in Cygwin"
#else
#	@echo "cd img ; make ; cd .. ; latex paper ; bibtex paper ; latex paper ; latex paper ; dvips -P pdf -t letter -Pdownload35 -o paper.ps paper.dvi ; ps2pdf -dPDFSETTINGS=/prepress -dSubsetFonts=true -dEmbedAllFonts=true -dMaxSubsetPct=100 -dCompatibilityLevel=1.3 paper.ps paper.pdf" | at now > /dev/null 2>&1
	cd img ; make
	# latex paper
	# bibtex paper
	latex paper
	latex paper
	dvips -P pdf -t letter -Pdownload35 -o paper.ps paper.dvi
	ps2pdf -dPDFSETTINGS=/prepress -dSubsetFonts=true -dEmbedAllFonts=true -dMaxSubsetPct=100 -dCompatibilityLevel=1.3 paper.ps paper.pdf
#endif
clean:
	cd img ; make clean
	./latex-clean.sh
