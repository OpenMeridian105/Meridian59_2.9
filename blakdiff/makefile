#
# makefile for blakdiff
#

TOPDIR=..
!include $(TOPDIR)\common.mak

# ----------------------------------------------------------------------
# Additional compiler flags (see common.mak)
# /TP           Compile as C++ code
# /arch:x64    Use SSE2 instructions (VS2013+ default to SSE2)
CFLAGS = $(CFLAGS) /arch:x64 /TP

# ----------------------------------------------------------------------
# Additional linker flags (see common.mak)
# /SUBSYSTEM:CONSOLE",5.01" NO-UI Windows XP (5.01)
LINKFLAGS = $(LINKFLAGS) /SUBSYSTEM:CONSOLE",5.01"

OBJS = $(OUTDIR)\blakdiff.obj

all: makedirs $(OUTDIR)\blakdiff.exe

$(OUTDIR)\blakdiff.exe : $(OBJS)
	$(LINK) $(LINKFLAGS) $(OBJS) -out:$@
	$(CP) $@ $(BLAKBINDIR)

!include $(TOPDIR)\rules.mak
