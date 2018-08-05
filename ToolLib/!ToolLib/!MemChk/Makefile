# This makefile made by Makatic2


CCExtra=-zpc1 -DMemCheck_MEMCHECK -JMemCheck:ANSI.,:mem -fw -g
LibName=ToolLibMem


ObjectFiles	=		\
			o.allocate	\
			o.applicatio	\
			o.backtrace	\
			o.box	\
			o.ci_string	\
			o.debug_io	\
			o.error	\
			o.exception	\
			o.fast_trig	\
			o.list	\
			o.message	\
			o.nevent	\
			o.nev_messag	\
			o.nev_suppor	\
			o.nev_toolbo	\
			o.nev_wimp	\
			o.saver	\
			o.save_buffe	\
			o.set	\
			o.shifting	\
			o.shifting_s	\
			o.tbx	\
			o.text_plot	\
			o.backtr_sup	\


ProjectName		=	!MemChk

Target = ^.o.$(LibName)

ASMFlags  = $(ASMExtra) -Stamp -NoCache -CloseExec -Quit -throwback
CCFlags   = $(CCExtra) -D__swi -fussy -fah -depend !Depend -throwback -I,@.^,C:
CPPFlags  = $(CPPExtra) -depend !Depend -throwback -I,@.^,C:
LinkFlags = $(LinkExtra)
LibFileflags = -c -o

ASM  = objasm $(ASMFlags)
CC   = cc -c $(CCFlags)
CPP  = Makatic._C++ c++ -c $(CPPFlags)
LINK = Link -aif -c++ $(LinkFlags)
LIBFILE = libfile -c



# Don't alter anything below this...


VPATH = @.^

.SUFFIXES: .o .s .c .c++

$(Target): $(ObjectFiles)
           $(LibFile) -o $@ $(ObjectFiles)

.s.o:
           $(ASM) -from $< -to $@

.c.o:
           $(CC) -o $@ $<

.c++.o:
           $(CPP) -o $@ $<


# Dynamic dependencies:
o.ci_string:	^.c.ci_string
o.ci_string:	^.h.ci_string
o.ci_string:	C:h.stddef
o.ci_string:	C:h.assert
o.ci_string:	C:h.ctype
o.text_plot:	^.c.text_plot
o.text_plot:	^.h.text_plot
o.text_plot:	C:h.os
o.text_plot:	C:h.types
o.text_plot:	C:h.assert
o.text_plot:	C:h.string
o.text_plot:	C:h.colourtrans
o.text_plot:	C:h.osspriteop
o.text_plot:	C:h.font
o.text_plot:	C:h.wimp
o.text_plot:	C:h.wimpreadsysinfo
o.allocate:	^.c.allocate
o.allocate:	^.h.allocate
o.allocate:	C:h.stdlib
o.allocate:	C:h.stdlib
o.allocate:	C:h.assert
o.allocate:	^.h.exception
o.allocate:	C:h.setjmp
o.allocate:	C:h.assert
o.allocate:	C:h.os
o.allocate:	C:h.types
o.box:	^.c.box
o.box:	^.h.box
o.box:	C:h.os
o.box:	C:h.types
o.box:	C:h.assert
o.box:	C:h.macros
o.error:	^.c.error
o.error:	^.h.error
o.error:	^.h.exception
o.error:	C:h.setjmp
o.error:	C:h.assert
o.error:	C:h.os
o.error:	C:h.types
o.error:	C:h.assert
o.error:	C:h.stdio
o.error:	C:h.stdlib
o.error:	C:h.string
o.error:	C:h.macros
o.error:	C:h.toolbox
o.error:	C:h.wimp
o.error:	C:h.osspriteop
o.error:	C:h.font
o.error:	C:h.messagetrans
o.error:	C:h.wimp
o.error:	^.h.allocate
o.error:	C:h.stdlib
o.error:	^.h.message
o.error:	^.h.tbx
o.error:	C:h.stddef
o.list:	^.c.list
o.list:	^.h.list
o.list:	C:h.stddef
o.list:	^.h.bool
o.list:	C:h.types
o.list:	C:h.assert
o.list:	^.h.allocate
o.list:	C:h.stdlib
o.list:	C:h.stdio
o.message:	^.c.message
o.message:	^.h.message
o.message:	C:h.assert
o.message:	C:h.string
o.message:	C:h.stdlib
o.message:	C:h.stdio
o.message:	C:h.messagetrans
o.message:	C:h.types
o.message:	C:h.os
o.message:	C:h.toolbox
o.message:	C:h.wimp
o.message:	C:h.osspriteop
o.message:	C:h.font
o.message:	^.h.exception
o.message:	C:h.setjmp
o.message:	C:h.assert
o.message:	^.h.allocate
o.message:	C:h.stdlib
o.nevent:	^.c.nevent
o.nevent:	^.h.nevent
o.nevent:	C:h.toolbox
o.nevent:	C:h.types
o.nevent:	C:h.os
o.nevent:	C:h.wimp
o.nevent:	C:h.osspriteop
o.nevent:	C:h.font
o.nevent:	C:h.messagetrans
o.nevent:	C:h.assert
o.nevent:	C:h.stdio
o.nevent:	^.h.nev_support
o.nev_messag:	^.c.nev_messag
o.nev_messag:	^.h.nev_message
o.nev_messag:	^.h.nevent
o.nev_messag:	C:h.toolbox
o.nev_messag:	C:h.types
o.nev_messag:	C:h.os
o.nev_messag:	C:h.wimp
o.nev_messag:	C:h.osspriteop
o.nev_messag:	C:h.font
o.nev_messag:	C:h.messagetrans
o.nev_messag:	C:h.assert
o.nev_messag:	C:h.stdio
o.nev_messag:	C:h.stdlib
o.nev_messag:	^.h.allocate
o.nev_messag:	C:h.stdlib
o.nev_messag:	^.h.list
o.nev_messag:	C:h.stddef
o.nev_messag:	^.h.bool
o.nev_messag:	^.h.nev_support
o.nev_messag:	^.h.set
o.nev_messag:	^.h.bool
o.nev_messag:	C:h.stddef
o.nev_suppor:	^.c.nev_suppor
o.nev_suppor:	^.h.nev_support
o.nev_suppor:	C:h.toolbox
o.nev_suppor:	C:h.types
o.nev_suppor:	C:h.os
o.nev_suppor:	C:h.wimp
o.nev_suppor:	C:h.osspriteop
o.nev_suppor:	C:h.font
o.nev_suppor:	C:h.messagetrans
o.nev_suppor:	C:h.assert
o.nev_toolbo:	^.c.nev_toolbo
o.nev_toolbo:	^.h.nev_toolbox
o.nev_toolbo:	^.h.nevent
o.nev_toolbo:	C:h.toolbox
o.nev_toolbo:	C:h.types
o.nev_toolbo:	C:h.os
o.nev_toolbo:	C:h.wimp
o.nev_toolbo:	C:h.osspriteop
o.nev_toolbo:	C:h.font
o.nev_toolbo:	C:h.messagetrans
o.nev_toolbo:	C:h.assert
o.nev_toolbo:	C:h.stdio
o.nev_toolbo:	C:h.stdlib
o.nev_toolbo:	^.h.allocate
o.nev_toolbo:	C:h.stdlib
o.nev_toolbo:	^.h.list
o.nev_toolbo:	C:h.stddef
o.nev_toolbo:	^.h.bool
o.nev_toolbo:	^.h.nev_support
o.nev_toolbo:	C:h.string
o.nev_toolbo:	^.h.set
o.nev_toolbo:	^.h.bool
o.nev_toolbo:	C:h.stddef
o.nev_wimp:	^.c.nev_wimp
o.nev_wimp:	^.h.nev_wimp
o.nev_wimp:	^.h.nevent
o.nev_wimp:	C:h.toolbox
o.nev_wimp:	C:h.types
o.nev_wimp:	C:h.os
o.nev_wimp:	C:h.wimp
o.nev_wimp:	C:h.osspriteop
o.nev_wimp:	C:h.font
o.nev_wimp:	C:h.messagetrans
o.nev_wimp:	C:h.assert
o.nev_wimp:	C:h.stdio
o.nev_wimp:	^.h.list
o.nev_wimp:	C:h.stddef
o.nev_wimp:	^.h.bool
o.nev_wimp:	^.h.allocate
o.nev_wimp:	C:h.stdlib
o.nev_wimp:	^.h.nev_support
o.saver:	^.c.saver
o.saver:	^.h.saver
o.saver:	C:h.toolbox
o.saver:	C:h.types
o.saver:	C:h.os
o.saver:	C:h.wimp
o.saver:	C:h.osspriteop
o.saver:	C:h.font
o.saver:	C:h.messagetrans
o.saver:	C:h.assert
o.saver:	C:h.saveas
o.saver:	C:h.window
o.saver:	C:h.keyboardshortcut
o.saver:	C:h.gadget
o.saver:	^.h.exception
o.saver:	C:h.setjmp
o.saver:	C:h.assert
o.saver:	C:h.hourglass
o.saver:	^.h.nev_toolbox
o.saver:	^.h.nevent
o.saver:	^.h.save_buffer
o.saver:	C:h.stddef
o.save_buffe:	^.c.save_buffe
o.save_buffe:	^.h.save_buffer
o.save_buffe:	C:h.stddef
o.save_buffe:	C:h.toolbox
o.save_buffe:	C:h.types
o.save_buffe:	C:h.os
o.save_buffe:	C:h.wimp
o.save_buffe:	C:h.osspriteop
o.save_buffe:	C:h.font
o.save_buffe:	C:h.messagetrans
o.save_buffe:	C:h.assert
o.save_buffe:	C:h.stdio
o.save_buffe:	C:h.string
o.save_buffe:	C:h.limits
o.save_buffe:	C:h.saveas
o.save_buffe:	C:h.window
o.save_buffe:	C:h.keyboardshortcut
o.save_buffe:	C:h.gadget
o.save_buffe:	C:h.osfile
o.save_buffe:	C:h.fileswitch
o.save_buffe:	C:h.osfind
o.save_buffe:	C:h.osgbpb
o.save_buffe:	^.h.nevent
o.save_buffe:	^.h.allocate
o.save_buffe:	C:h.stdlib
o.save_buffe:	^.h.error
o.save_buffe:	^.h.exception
o.save_buffe:	C:h.setjmp
o.save_buffe:	C:h.assert
o.set:	^.c.set
o.set:	^.h.set
o.set:	^.h.bool
o.set:	C:h.types
o.set:	C:h.stddef
o.set:	C:h.assert
o.set:	C:h.string
o.set:	C:h.stdlib
o.set:	^.h.allocate
o.set:	C:h.stdlib
o.set:	^.h.list
o.set:	C:h.stddef
o.set:	^.h.bool
o.set:	^.h.exception
o.set:	C:h.setjmp
o.set:	C:h.assert
o.set:	C:h.os
o.set:	C:h.stdio
o.shifting_s:	^.c.shifting_s
o.shifting_s:	^.h.shifting_send
o.shifting_s:	C:h.stddef
o.shifting_s:	^.h.exception
o.shifting_s:	C:h.setjmp
o.shifting_s:	C:h.assert
o.shifting_s:	C:h.os
o.shifting_s:	C:h.types
o.shifting_s:	^.h.save_buffer
o.shifting_s:	C:h.stddef
o.shifting_s:	C:h.toolbox
o.shifting_s:	C:h.wimp
o.shifting_s:	C:h.osspriteop
o.shifting_s:	C:h.font
o.shifting_s:	C:h.messagetrans
o.shifting_s:	^.h.shifting
o.shifting_s:	C:h.stddef
o.shifting_s:	^.h.allocate
o.shifting_s:	C:h.stdlib
o.tbx:	^.c.tbx
o.tbx:	^.h.tbx
o.tbx:	C:h.toolbox
o.tbx:	C:h.types
o.tbx:	C:h.os
o.tbx:	C:h.wimp
o.tbx:	C:h.osspriteop
o.tbx:	C:h.font
o.tbx:	C:h.messagetrans
o.tbx:	C:h.stddef
o.tbx:	C:h.assert
o.tbx:	C:h.stdio
o.tbx:	C:h.displayfield
o.tbx:	C:h.gadget
o.tbx:	C:h.macros
o.tbx:	C:h.radiobutton
o.tbx:	C:h.stringset
o.tbx:	C:h.writablefield
o.tbx:	^.h.allocate
o.tbx:	C:h.stdlib
o.applicatio:	^.c.applicatio
o.applicatio:	^.h.application
o.applicatio:	^.h.bool
o.applicatio:	C:h.types
o.applicatio:	C:h.assert
o.applicatio:	C:h.stdio
o.applicatio:	C:h.stdlib
o.applicatio:	C:h.toolbox
o.applicatio:	C:h.os
o.applicatio:	C:h.wimp
o.applicatio:	C:h.osspriteop
o.applicatio:	C:h.font
o.applicatio:	C:h.messagetrans
o.applicatio:	^.h.error
o.applicatio:	^.h.exception
o.applicatio:	C:h.setjmp
o.applicatio:	C:h.assert
o.applicatio:	^.h.nevent
o.applicatio:	^.h.nev_toolbox
o.applicatio:	^.h.nevent
o.applicatio:	^.h.nev_message
o.applicatio:	^.h.nevent
o.applicatio:	MemCheck:h.MemCheck
o.applicatio:	C:h.stddef
o.applicatio:	C:h.stdio
o.backtrace:	^.c.backtrace
o.backtrace:	^.h.backtrace
o.backtrace:	C:h.assert
o.backtrace:	C:h.stdio
o.backtrace:	^.h.backtr_sup
o.backtrace:	C:h.kernel
o.backtrace:	^.h.debug_io
o.backtrace:	MemCheck:h.MemCheck
o.backtrace:	C:h.stddef
o.backtrace:	C:h.stdio
o.debug_io:	^.c.debug_io
o.debug_io:	^.h.debug_io
o.debug_io:	C:h.stdio
o.debug_io:	C:h.stdlib
o.debug_io:	C:h.osargs
o.debug_io:	C:h.types
o.debug_io:	C:h.os
o.debug_io:	C:h.fileswitch
o.debug_io:	^.h.bool
o.exception:	^.c.exception
o.exception:	^.h.exception
o.exception:	C:h.setjmp
o.exception:	C:h.assert
o.exception:	C:h.os
o.exception:	C:h.types
o.exception:	C:h.assert
o.exception:	C:h.signal
o.exception:	C:h.stdlib
o.exception:	C:h.string
o.exception:	C:h.stdio
o.exception:	C:h.kernel
o.exception:	^.h.backtrace
o.exception:	^.h.debug_io
o.fast_trig:	^.c.fast_trig
o.fast_trig:	^.h.fast_trig
o.fast_trig:	C:h.assert
o.fast_trig:	C:h.math
o.shifting:	^.c.shifting
o.shifting:	^.h.shifting
o.shifting:	C:h.stddef
o.shifting:	C:h.messagetrans
o.shifting:	C:h.types
o.shifting:	C:h.os
o.shifting:	^.h.allocate
o.shifting:	C:h.stdlib
o.shifting:	C:h.assert
o.shifting:	C:h.flex
o.shifting:	C:h.kernel
o.shifting:	C:h.toolbox
o.shifting:	C:h.wimp
o.shifting:	C:h.osspriteop
o.shifting:	C:h.font
o.shifting:	^.h.exception
o.shifting:	C:h.setjmp
o.shifting:	C:h.assert
o.shifting:	^.h.tbx
o.shifting:	C:h.stddef
o.shifting:	MemCheck:h.MemCheck
o.shifting:	C:h.stddef
o.shifting:	C:h.stdio
