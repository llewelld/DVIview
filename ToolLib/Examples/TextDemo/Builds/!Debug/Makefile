# This makefile made by Makatic2


ExtraLibs=ToolLib:o.ToolLibDbg


ObjectFiles	=		\
			o.main	\


ProjectName		=	!Debug

Libraries = OSLib:o.OSLib C:o.stubs

Target = ^.^.!Text.!RunImage

ASMFlags  = $(ASMExtra) -Stamp -NoCache -CloseExec -Quit -throwback
CCFlags   = $(CCExtra) -D__swi -fussy -fah -depend !Depend -throwback -I,@.^,C:
CPPFlags  = $(CPPExtra) -depend !Depend -throwback -I,@.^,C:
LinkFlags = $(LinkExtra)

ASM  = objasm $(ASMFlags)
CC   = cc -c $(CCFlags)
CPP  = Makatic._C++ c++ -c $(CPPFlags)
LINK = Link -aif -c++ $(LinkFlags)



# Don't alter anything below this...


VPATH = @.^

.SUFFIXES: .o .s .c .c++

$(Target): $(ObjectFiles) $(ExtraLibs) $(Libraries)
           $(LINK) -o $@ $(ObjectFiles) $(ExtraLibs) $(Libraries)
           Settype $@ ff8

.s.o:
           $(ASM) -from $< -to $@

.c.o:
           $(CC) -o $@ $<

.c++.o:
           $(CPP) -o $@ $<


# Dynamic dependencies:
o.main:	^.c.main
o.main:	C:h.colourtrans
o.main:	C:h.types
o.main:	C:h.os
o.main:	C:h.osspriteop
o.main:	C:h.font
o.main:	C:h.window
o.main:	C:h.toolbox
o.main:	C:h.wimp
o.main:	C:h.messagetrans
o.main:	C:h.keyboardshortcut
o.main:	C:h.gadget
o.main:	C:h.applicatio
o.main:	C:h.bool
o.main:	C:h.exception
o.main:	C:h.nev_wimp
o.main:	C:h.nevent
o.main:	C:h.text_plot
