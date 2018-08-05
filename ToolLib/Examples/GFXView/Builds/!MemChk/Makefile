# This makefile made by Makatic2


CCExtra=-zpc1 -DMemCheck_MEMCHECK -JMemCheck:ANSI.,:mem -fw -g
LinkExtra=-d
ExtraLibs=ToolLib:o.ToolLibMem MemCheck:o.MC


ObjectFiles	=		\
			o.draw_pic	\
			o.jpeg_pic	\
			o.main	\
			o.picture	\
			o.sprite_pic	\
			o.viewer	\


ProjectName		=	!MemChk

Libraries = C:o.stubs C:o.flexlib OSLib:o.OSLib

Target = ^.^.!GFXView.!RunImage

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
o.picture:	^.c.picture
o.picture:	^.h.picture
o.picture:	C:h.os
o.picture:	C:h.types
o.picture:	C:h.osfile
o.picture:	C:h.fileswitch
o.picture:	C:h.jpeg
o.picture:	C:h.allocate
o.picture:	C:h.stdlib
o.picture:	C:h.exception
o.picture:	C:h.setjmp
o.picture:	C:h.assert
o.picture:	^.h.draw_pic
o.picture:	^.h.sprite_pic
o.picture:	^.h.jpeg_pic
o.sprite_pic:	^.c.sprite_pic
o.sprite_pic:	^.h.sprite_pic
o.sprite_pic:	C:h.os
o.sprite_pic:	C:h.types
o.sprite_pic:	C:h.assert
o.sprite_pic:	C:h.colourtrans
o.sprite_pic:	C:h.osspriteop
o.sprite_pic:	C:h.font
o.sprite_pic:	C:h.osspriteop
o.sprite_pic:	C:h.osfile
o.sprite_pic:	C:h.fileswitch
o.sprite_pic:	C:h.wimp
o.sprite_pic:	C:h.wimpreadsysinfo
o.sprite_pic:	C:h.allocate
o.sprite_pic:	C:h.stdlib
o.sprite_pic:	C:h.exception
o.sprite_pic:	C:h.setjmp
o.sprite_pic:	C:h.assert
o.sprite_pic:	C:h.shifting
o.sprite_pic:	C:h.stddef
o.sprite_pic:	C:h.messagetrans
o.sprite_pic:	C:h.allocate
o.draw_pic:	^.c.draw_pic
o.draw_pic:	^.h.draw_pic
o.draw_pic:	C:h.os
o.draw_pic:	C:h.types
o.draw_pic:	C:h.assert
o.draw_pic:	C:h.drawfile
o.draw_pic:	C:h.osspriteop
o.draw_pic:	C:h.draw
o.draw_pic:	C:h.font
o.draw_pic:	C:h.wimp
o.draw_pic:	C:h.jpeg
o.draw_pic:	C:h.osfile
o.draw_pic:	C:h.fileswitch
o.draw_pic:	C:h.allocate
o.draw_pic:	C:h.stdlib
o.draw_pic:	C:h.exception
o.draw_pic:	C:h.setjmp
o.draw_pic:	C:h.assert
o.draw_pic:	C:h.shifting
o.draw_pic:	C:h.stddef
o.draw_pic:	C:h.messagetrans
o.draw_pic:	C:h.allocate
o.jpeg_pic:	^.c.jpeg_pic
o.jpeg_pic:	^.h.jpeg_pic
o.jpeg_pic:	C:h.os
o.jpeg_pic:	C:h.types
o.jpeg_pic:	C:h.assert
o.jpeg_pic:	C:h.stdlib
o.jpeg_pic:	C:h.jpeg
o.jpeg_pic:	C:h.osfile
o.jpeg_pic:	C:h.fileswitch
o.jpeg_pic:	C:h.wimpreadsysinfo
o.jpeg_pic:	C:h.wimp
o.jpeg_pic:	C:h.osspriteop
o.jpeg_pic:	C:h.font
o.jpeg_pic:	C:h.allocate
o.jpeg_pic:	C:h.stdlib
o.jpeg_pic:	C:h.exception
o.jpeg_pic:	C:h.setjmp
o.jpeg_pic:	C:h.assert
o.jpeg_pic:	C:h.shifting
o.jpeg_pic:	C:h.stddef
o.jpeg_pic:	C:h.messagetrans
o.jpeg_pic:	C:h.allocate
o.main:	^.c.main
o.main:	C:h.application
o.main:	C:h.bool
o.main:	C:h.types
o.main:	C:h.nev_wimp
o.main:	C:h.nevent
o.main:	C:h.toolbox
o.main:	C:h.os
o.main:	C:h.wimp
o.main:	C:h.osspriteop
o.main:	C:h.font
o.main:	C:h.messagetrans
o.main:	C:h.shifting
o.main:	C:h.stddef
o.main:	C:h.allocate
o.main:	C:h.stdlib
o.main:	^.h.viewer
o.viewer:	^.c.viewer
o.viewer:	^.h.viewer
o.viewer:	C:h.assert
o.viewer:	C:h.scale
o.viewer:	C:h.types
o.viewer:	C:h.toolbox
o.viewer:	C:h.os
o.viewer:	C:h.wimp
o.viewer:	C:h.osspriteop
o.viewer:	C:h.font
o.viewer:	C:h.messagetrans
o.viewer:	C:h.window
o.viewer:	C:h.keyboardshortcut
o.viewer:	C:h.gadget
o.viewer:	C:h.window
o.viewer:	C:h.allocate
o.viewer:	C:h.stdlib
o.viewer:	C:h.exception
o.viewer:	C:h.setjmp
o.viewer:	C:h.assert
o.viewer:	C:h.nev_message
o.viewer:	C:h.nevent
o.viewer:	C:h.nev_toolbox
o.viewer:	C:h.nevent
o.viewer:	C:h.nev_wimp
o.viewer:	C:h.nevent
o.viewer:	^.h.picture
