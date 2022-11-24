TOPDIR=..\..\..
!include $(TOPDIR)\common.mak

SOURCEDIR = .
OUTDIR = .

.SUFFIXES: .bbg

BGFS = neeleme.bgf neelemeX.bgf iunholyt.bgf xeoneru.bgf xeoneruX.bgf \
       pear.bgf peartree.bgf orange.bgf orangetree.bgf cookie.bgf \
       mmdrat.bgf mfdrat.bgf arrowgold.bgf corncob.bgf cornbasket.bgf \
       mashtaters.bgf stuffing.bgf turkey.bgf ham.bgf hamslices.bgf  \
       rouladen.bgf pumpslice.bgf pumppie.bgf pecanslice.bgf pecanpie.bgf \
       indianhat.bgf indianhatF.bgf pilgrimhat.bgf pilgrimhatF.bgf 

!include $(RESOURCEDIR)\copy.mak

{$(SOURCEDIR)}.bbg.bgf:
   $(MAKEBGF) -o $(OUTDIR)\$*.bgf @$*.bbg

clean:

