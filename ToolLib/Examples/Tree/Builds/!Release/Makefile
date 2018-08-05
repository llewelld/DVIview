# This makefile made by Makatic2


CCExtra=-DNDEBUG
ExtraLibs=ToolLib:o.ToolLib


ObjectFiles	=		\
			o.diagram_sa	\
			o.line_plott	\
			o.line_store	\
			o.main	\
			o.tree	\
			o.treeparams	\
			o.treewindow	\


ProjectName		=	!Release

Libraries = OSLib:o.OSLib C:o.flexlib C:o.stubs

Target = ^.^.!Tree.!RunImage

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
o.line_plott:	^.c.line_plott
o.line_plott:	^.h.line_plotter
o.line_plott:	^.h.line_processor
o.line_plott:	C:h.os
o.line_plott:	C:h.types
o.line_plott:	C:h.colourtrans
o.line_plott:	C:h.osspriteop
o.line_plott:	C:h.font
o.diagram_sa:	^.c.diagram_sa
o.diagram_sa:	^.h.diagram_save
o.diagram_sa:	C:h.drawfile
o.diagram_sa:	C:h.types
o.diagram_sa:	C:h.os
o.diagram_sa:	C:h.osspriteop
o.diagram_sa:	C:h.draw
o.diagram_sa:	C:h.font
o.diagram_sa:	C:h.wimp
o.diagram_sa:	C:h.jpeg
o.diagram_sa:	C:h.macros
o.diagram_sa:	C:h.box
o.diagram_sa:	^.h.line_storer
o.diagram_sa:	^.h.line_processor
o.diagram_sa:	C:h.save_buffer
o.diagram_sa:	C:h.toolbox
o.diagram_sa:	C:h.messagetrans
o.line_store:	^.c.line_store
o.line_store:	^.h.line_storer
o.line_store:	^.h.line_processor
o.line_store:	C:h.shifting
o.line_store:	C:h.messagetrans
o.line_store:	C:h.types
o.line_store:	C:h.os
o.line_store:	C:h.allocate
o.main:	^.c.main
o.main:	C:h.application
o.main:	C:h.bool
o.main:	C:h.types
o.main:	C:h.fast_trig
o.main:	C:h.nev_wimp
o.main:	C:h.nevent
o.main:	C:h.toolbox
o.main:	C:h.os
o.main:	C:h.wimp
o.main:	C:h.osspriteop
o.main:	C:h.font
o.main:	C:h.messagetrans
o.main:	C:h.shifting
o.main:	C:h.allocate
o.main:	^.h.treewindow
o.main:	^.h.treeparams
o.tree:	^.c.tree
o.tree:	^.h.tree
o.tree:	^.h.line_processor
o.tree:	C:h.fast_trig
o.treeparams:	^.c.treeparams
o.treeparams:	^.h.treeparams
o.treeparams:	C:h.hourglass
o.treeparams:	C:h.types
o.treeparams:	C:h.os
o.treeparams:	C:h.numberrange
o.treeparams:	C:h.toolbox
o.treeparams:	C:h.wimp
o.treeparams:	C:h.osspriteop
o.treeparams:	C:h.font
o.treeparams:	C:h.messagetrans
o.treeparams:	C:h.gadget
o.treeparams:	C:h.toolbox
o.treeparams:	C:h.error
o.treeparams:	C:h.exception
o.treeparams:	C:h.exception
o.treeparams:	C:h.nev_toolbox
o.treeparams:	C:h.nevent
o.treeparams:	^.h.line_storer
o.treeparams:	^.h.line_processor
o.treeparams:	^.h.tree
o.treeparams:	^.h.line_processor
o.treeparams:	^.h.treewindow
o.treewindow:	^.c.treewindow
o.treewindow:	^.h.treewindow
o.treewindow:	C:h.toolbox
o.treewindow:	C:h.types
o.treewindow:	C:h.os
o.treewindow:	C:h.wimp
o.treewindow:	C:h.osspriteop
o.treewindow:	C:h.font
o.treewindow:	C:h.messagetrans
o.treewindow:	C:h.wimp
o.treewindow:	C:h.window
o.treewindow:	C:h.keyboardshortcut
o.treewindow:	C:h.gadget
o.treewindow:	C:h.exception
o.treewindow:	C:h.nev_wimp
o.treewindow:	C:h.nevent
o.treewindow:	C:h.saver
o.treewindow:	^.h.diagram_save
o.treewindow:	^.h.line_plotter
o.treewindow:	^.h.line_processor
o.treewindow:	^.h.line_storer
o.treewindow:	^.h.line_processor
