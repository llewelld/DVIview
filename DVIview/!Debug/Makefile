# This makefile made by Makatic2


CCExtra=-DPRINT_VERBOSE
ExtraLibs=ToolLib:o.ToolLibDbg


ObjectFiles	=		\
			o.bstream_er	\
			o.byte_strea	\
			o.choices	\
			o.command_pr	\
			o.document	\
			o.draw_utils	\
			o.dvifile	\
			o.dviops	\
			o.file	\
			o.file_error	\
			o.font_file	\
			o.font_set	\
			o.font_summa	\
			o.font_table	\
			o.log	\
			o.magnifier	\
			o.main	\
			o.mask	\
			o.optionfile	\
			o.page	\
			o.page_diag	\
			o.papersize	\
			o.picture	\
			o.pic_draw	\
			o.pic_jpeg	\
			o.pic_sprite	\
			o.print_core	\
			o.print_job	\
			o.real_font	\
			o.render_lis	\
			o.special	\
			o.substitute	\
			o.sys_font_l	\
			o.tex_font	\
			o.tfm	\
			o.units	\
			o.var_stack	\
			o.viewer	\
			o.virtual_fo	\
			o.vprint	\
			o.vprint_dbx	\
			o.vp_area	\
			o.vp_font	\
			o.vp_iter	\
			o.vp_side	\
			o.vp_status	\


ProjectName		=	!Debug

Libraries = C:o.flexlib C:o.stubs OSLib:o.OSLib

Target = ^.!DVIview.!RunImage

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
o.units:	^.c.units
o.units:	^.h.units
o.units:	C:h.os
o.units:	C:h.types
o.print_job:	^.c.print_job
o.print_job:	^.h.print_job
o.print_job:	C:h.pdriver
o.print_job:	C:h.types
o.print_job:	C:h.os
o.print_job:	C:h.draw
o.print_job:	C:h.font
o.print_job:	C:h.messagetrans
o.print_job:	C:h.jpeg
o.print_job:	C:h.osfind
o.print_job:	C:h.fileswitch
o.print_job:	C:h.exception
o.vprint:	^.c.vprint
o.vprint:	^.h.vprint
o.vprint:	^.h.vp_choices
o.vprint:	C:h.bool
o.vprint:	C:h.types
o.vprint:	^.h.print_doc
o.vprint:	C:h.bool
o.vprint:	^.h.print_declarer
o.vprint:	C:h.os
o.vprint:	C:h.exception
o.vprint:	^.h.print_core
o.vprint:	^.h.print_iterator
o.vprint:	C:h.bool
o.vprint:	^.h.print_side
o.vprint:	^.h.print_rep
o.vprint:	^.h.vp_iter
o.vprint:	^.h.print_doc
o.vprint:	^.h.print_iter
o.vprint:	^.h.vp_choices
o.vprint:	^.h.vp_status
o.vprint:	^.h.print_rep
o.var_stack:	^.c.var_stack
o.var_stack:	^.h.var_stack
o.var_stack:	C:h.allocate
o.var_stack:	C:h.bool
o.var_stack:	C:h.types
o.bstream_er:	^.c.bstream_er
o.bstream_er:	^.h.bstream_error
o.bstream_er:	^.h.byte_stream
o.bstream_er:	^.h.file_error
o.bstream_er:	^.h.file
o.bstream_er:	C:h.bool
o.bstream_er:	C:h.types
o.byte_strea:	^.c.byte_strea
o.byte_strea:	^.h.byte_stream
o.byte_strea:	C:h.allocate
o.byte_strea:	C:h.exception
o.byte_strea:	C:h.os
o.byte_strea:	C:h.types
o.byte_strea:	^.h.file
o.byte_strea:	C:h.bool
o.dviops:	^.c.dviops
o.dviops:	^.h.dviops
o.dviops:	^.h.byte_stream
o.dviops:	C:h.allocate
o.dviops:	C:h.exception
o.dviops:	C:h.os
o.dviops:	C:h.types
o.choices:	^.c.choices
o.choices:	^.h.choices
o.choices:	C:h.numberrange
o.choices:	C:h.types
o.choices:	C:h.toolbox
o.choices:	C:h.os
o.choices:	C:h.wimp
o.choices:	C:h.osspriteop
o.choices:	C:h.font
o.choices:	C:h.messagetrans
o.choices:	C:h.gadget
o.choices:	C:h.nev_toolbox
o.choices:	C:h.nevent
o.choices:	^.h.optionfile
o.choices:	C:h.bool
o.choices:	^.h.units
o.command_pr:	^.c.command_pr
o.command_pr:	^.h.command_processor
o.command_pr:	^.h.byte_stream
o.command_pr:	^.h.font_table
o.command_pr:	C:h.bool
o.command_pr:	C:h.types
o.command_pr:	^.h.font_set
o.command_pr:	C:h.font
o.command_pr:	C:h.os
o.command_pr:	C:h.set
o.command_pr:	C:h.bool
o.command_pr:	^.h.tex_font
o.command_pr:	^.h.dviops
o.command_pr:	^.h.byte_stream
o.command_pr:	^.h.font_set
o.command_pr:	^.h.renderer
o.command_pr:	^.h.real_font
o.command_pr:	C:h.bool
o.command_pr:	C:h.exception
o.command_pr:	^.h.var_stack
o.draw_utils:	^.c.draw_utils
o.draw_utils:	^.h.draw_utils
o.draw_utils:	C:h.drawfile
o.draw_utils:	C:h.types
o.draw_utils:	C:h.os
o.draw_utils:	C:h.osspriteop
o.draw_utils:	C:h.draw
o.draw_utils:	C:h.font
o.draw_utils:	C:h.wimp
o.draw_utils:	C:h.jpeg
o.draw_utils:	^.h.font_set
o.draw_utils:	C:h.font
o.draw_utils:	C:h.set
o.draw_utils:	C:h.bool
o.draw_utils:	C:h.macros
o.draw_utils:	C:h.exception
o.draw_utils:	C:h.save_buffer
o.draw_utils:	C:h.toolbox
o.draw_utils:	C:h.messagetrans
o.draw_utils:	C:h.shifting
o.draw_utils:	C:h.allocate
o.dvifile:	^.c.dvifile
o.dvifile:	^.h.dvifile
o.dvifile:	^.h.page
o.dvifile:	^.h.font_table
o.dvifile:	C:h.bool
o.dvifile:	C:h.types
o.dvifile:	^.h.font_set
o.dvifile:	C:h.font
o.dvifile:	C:h.os
o.dvifile:	C:h.set
o.dvifile:	C:h.bool
o.dvifile:	^.h.tex_font
o.dvifile:	^.h.dviops
o.dvifile:	^.h.byte_stream
o.dvifile:	^.h.font_set
o.dvifile:	^.h.renderer
o.dvifile:	^.h.real_font
o.dvifile:	C:h.bool
o.dvifile:	^.h.font_set
o.dvifile:	^.h.units
o.dvifile:	C:h.allocate
o.dvifile:	C:h.exception
o.dvifile:	C:h.hourglass
o.dvifile:	^.h.byte_stream
o.dvifile:	^.h.bstream_error
o.dvifile:	^.h.byte_stream
o.file:	^.c.file
o.file:	^.h.file
o.file:	C:h.bool
o.file:	C:h.types
o.file:	C:h.macros
o.file:	C:h.osargs
o.file:	C:h.os
o.file:	C:h.fileswitch
o.file:	C:h.osfind
o.file:	C:h.osfile
o.file:	C:h.osgbpb
o.file:	C:h.allocate
o.file:	C:h.exception
o.file:	C:h.message
o.file_error:	^.c.file_error
o.file_error:	^.h.file_error
o.file_error:	^.h.file
o.file_error:	C:h.bool
o.file_error:	C:h.types
o.file_error:	C:h.macros
o.file_error:	C:h.exception
o.file_error:	C:h.os
o.file_error:	C:h.message
o.font_file:	^.c.font_file
o.font_file:	^.h.font_file
o.font_file:	C:h.os
o.font_file:	C:h.types
o.font_file:	C:h.exception
o.font_file:	C:h.message
o.font_set:	^.c.font_set
o.font_set:	^.h.font_set
o.font_set:	C:h.font
o.font_set:	C:h.types
o.font_set:	C:h.os
o.font_set:	C:h.set
o.font_set:	C:h.bool
o.font_summa:	^.c.font_summa
o.font_summa:	^.h.font_summary
o.font_summa:	C:h.bool
o.font_summa:	C:h.types
o.font_summa:	C:h.allocate
o.font_summa:	C:h.ci_string
o.font_summa:	C:h.exception
o.font_summa:	C:h.os
o.font_summa:	C:h.list
o.font_summa:	C:h.bool
o.font_summa:	C:h.message
o.font_table:	^.c.font_table
o.font_table:	^.h.font_table
o.font_table:	C:h.bool
o.font_table:	C:h.types
o.font_table:	^.h.font_set
o.font_table:	C:h.font
o.font_table:	C:h.os
o.font_table:	C:h.set
o.font_table:	C:h.bool
o.font_table:	^.h.tex_font
o.font_table:	^.h.dviops
o.font_table:	^.h.byte_stream
o.font_table:	^.h.font_set
o.font_table:	^.h.renderer
o.font_table:	^.h.real_font
o.font_table:	C:h.bool
o.font_table:	C:h.allocate
o.font_table:	C:h.exception
o.font_table:	C:h.list
o.font_table:	C:h.bool
o.log:	^.c.log
o.log:	^.h.log
o.log:	C:h.macros
o.log:	C:h.colourtrans
o.log:	C:h.types
o.log:	C:h.os
o.log:	C:h.osspriteop
o.log:	C:h.font
o.log:	C:h.window
o.log:	C:h.toolbox
o.log:	C:h.wimp
o.log:	C:h.messagetrans
o.log:	C:h.keyboardshortcut
o.log:	C:h.gadget
o.log:	C:h.allocate
o.log:	C:h.exception
o.log:	C:h.nev_wimp
o.log:	C:h.nevent
o.log:	C:h.nev_toolbox
o.log:	C:h.nevent
o.log:	C:h.set
o.log:	C:h.bool
o.log:	C:h.tbx
o.log:	C:h.text_plot
o.magnifier:	^.c.magnifier
o.magnifier:	^.h.magnifier
o.magnifier:	^.h.page
o.magnifier:	^.h.font_table
o.magnifier:	C:h.bool
o.magnifier:	C:h.types
o.magnifier:	^.h.font_set
o.magnifier:	C:h.font
o.magnifier:	C:h.os
o.magnifier:	C:h.set
o.magnifier:	C:h.bool
o.magnifier:	^.h.tex_font
o.magnifier:	^.h.dviops
o.magnifier:	^.h.byte_stream
o.magnifier:	^.h.font_set
o.magnifier:	^.h.renderer
o.magnifier:	^.h.real_font
o.magnifier:	C:h.bool
o.magnifier:	^.h.font_set
o.magnifier:	C:h.scale
o.magnifier:	C:h.toolbox
o.magnifier:	C:h.wimp
o.magnifier:	C:h.osspriteop
o.magnifier:	C:h.messagetrans
o.magnifier:	C:h.window
o.magnifier:	C:h.keyboardshortcut
o.magnifier:	C:h.gadget
o.magnifier:	C:h.window
o.magnifier:	C:h.exception
o.magnifier:	C:h.nev_toolbox
o.magnifier:	C:h.nevent
o.magnifier:	C:h.nev_wimp
o.magnifier:	C:h.nevent
o.magnifier:	C:h.tbx
o.magnifier:	^.h.optionfile
o.magnifier:	C:h.bool
o.magnifier:	^.h.units
o.mask:	^.c.mask
o.mask:	^.h.mask
o.mask:	C:h.os
o.mask:	C:h.types
o.mask:	C:h.drawfile
o.mask:	C:h.osspriteop
o.mask:	C:h.draw
o.mask:	C:h.font
o.mask:	C:h.wimp
o.mask:	C:h.jpeg
o.mask:	C:h.allocate
o.mask:	C:h.box
o.mask:	C:h.exception
o.mask:	C:h.list
o.mask:	C:h.bool
o.mask:	C:h.save_buffer
o.mask:	C:h.toolbox
o.mask:	C:h.messagetrans
o.optionfile:	^.c.optionfile
o.optionfile:	^.h.optionfile
o.optionfile:	C:h.bool
o.optionfile:	C:h.types
o.optionfile:	C:h.message
o.optionfile:	C:h.error
o.optionfile:	C:h.exception
o.optionfile:	C:h.os
o.optionfile:	^.h.file_error
o.optionfile:	^.h.file
o.optionfile:	C:h.bool
o.papersize:	^.c.papersize
o.papersize:	^.h.papersize
o.papersize:	C:h.bool
o.papersize:	C:h.types
o.papersize:	C:h.exception
o.papersize:	C:h.os
o.papersize:	C:h.list
o.papersize:	C:h.bool
o.papersize:	C:h.nev_toolbox
o.papersize:	C:h.nevent
o.papersize:	C:h.toolbox
o.papersize:	C:h.wimp
o.papersize:	C:h.osspriteop
o.papersize:	C:h.font
o.papersize:	C:h.messagetrans
o.papersize:	C:h.tbx
o.papersize:	C:h.menu
o.papersize:	C:h.numberrange
o.papersize:	C:h.gadget
o.papersize:	C:h.writablefield
o.papersize:	^.h.optionfile
o.papersize:	C:h.bool
o.papersize:	^.h.units
o.picture:	^.c.picture
o.picture:	^.h.picture
o.picture:	C:h.os
o.picture:	C:h.types
o.picture:	^.h.font_set
o.picture:	C:h.font
o.picture:	C:h.set
o.picture:	C:h.bool
o.picture:	C:h.jpeg
o.picture:	C:h.osfile
o.picture:	C:h.fileswitch
o.picture:	C:h.allocate
o.picture:	C:h.box
o.picture:	C:h.exception
o.picture:	C:h.list
o.picture:	C:h.bool
o.picture:	C:h.message
o.picture:	^.h.pic_draw
o.picture:	^.h.font_set
o.picture:	^.h.pic_sprite
o.picture:	^.h.pic_jpeg
o.picture:	^.h.units
o.pic_draw:	^.c.pic_draw
o.pic_draw:	^.h.pic_draw
o.pic_draw:	C:h.os
o.pic_draw:	C:h.types
o.pic_draw:	^.h.font_set
o.pic_draw:	C:h.font
o.pic_draw:	C:h.set
o.pic_draw:	C:h.bool
o.pic_draw:	C:h.drawfile
o.pic_draw:	C:h.osspriteop
o.pic_draw:	C:h.draw
o.pic_draw:	C:h.wimp
o.pic_draw:	C:h.jpeg
o.pic_draw:	C:h.osargs
o.pic_draw:	C:h.fileswitch
o.pic_draw:	C:h.osgbpb
o.pic_draw:	C:h.osfile
o.pic_draw:	C:h.osfind
o.pic_draw:	C:h.allocate
o.pic_draw:	C:h.exception
o.pic_draw:	C:h.shifting
o.pic_draw:	C:h.messagetrans
o.pic_draw:	C:h.allocate
o.pic_draw:	^.h.draw_utils
o.pic_draw:	C:h.drawfile
o.pic_draw:	^.h.font_set
o.pic_jpeg:	^.c.pic_jpeg
o.pic_jpeg:	^.h.pic_jpeg
o.pic_jpeg:	C:h.os
o.pic_jpeg:	C:h.types
o.pic_jpeg:	C:h.drawfile
o.pic_jpeg:	C:h.osspriteop
o.pic_jpeg:	C:h.draw
o.pic_jpeg:	C:h.font
o.pic_jpeg:	C:h.wimp
o.pic_jpeg:	C:h.jpeg
o.pic_jpeg:	C:h.jpeg
o.pic_jpeg:	C:h.macros
o.pic_jpeg:	C:h.osfile
o.pic_jpeg:	C:h.fileswitch
o.pic_jpeg:	C:h.wimpreadsysinfo
o.pic_jpeg:	C:h.allocate
o.pic_jpeg:	C:h.exception
o.pic_jpeg:	C:h.message
o.pic_jpeg:	C:h.save_buffer
o.pic_jpeg:	C:h.toolbox
o.pic_jpeg:	C:h.messagetrans
o.pic_jpeg:	C:h.shifting
o.pic_jpeg:	C:h.allocate
o.pic_jpeg:	C:h.shifting_send
o.pic_jpeg:	^.h.units
o.pic_sprite:	^.c.pic_sprite
o.pic_sprite:	^.h.pic_sprite
o.pic_sprite:	C:h.os
o.pic_sprite:	C:h.types
o.pic_sprite:	C:h.colourtrans
o.pic_sprite:	C:h.osspriteop
o.pic_sprite:	C:h.font
o.pic_sprite:	C:h.drawfile
o.pic_sprite:	C:h.draw
o.pic_sprite:	C:h.wimp
o.pic_sprite:	C:h.jpeg
o.pic_sprite:	C:h.osspriteop
o.pic_sprite:	C:h.osfile
o.pic_sprite:	C:h.fileswitch
o.pic_sprite:	C:h.wimp
o.pic_sprite:	C:h.wimpreadsysinfo
o.pic_sprite:	C:h.allocate
o.pic_sprite:	C:h.exception
o.pic_sprite:	C:h.save_buffer
o.pic_sprite:	C:h.toolbox
o.pic_sprite:	C:h.messagetrans
o.pic_sprite:	C:h.shifting
o.pic_sprite:	C:h.allocate
o.pic_sprite:	C:h.shifting_send
o.pic_sprite:	^.h.units
o.real_font:	^.c.real_font
o.real_font:	^.h.real_font
o.real_font:	C:h.bool
o.real_font:	C:h.types
o.real_font:	C:h.allocate
o.real_font:	C:h.ci_string
o.real_font:	C:h.error
o.real_font:	C:h.exception
o.real_font:	C:h.os
o.real_font:	C:h.exception
o.real_font:	^.h.log
o.real_font:	C:h.message
o.real_font:	^.h.substitute
o.real_font:	^.h.tfm
o.real_font:	C:h.bool
o.render_lis:	^.c.render_lis
o.render_lis:	^.h.render_list
o.render_lis:	C:h.bool
o.render_lis:	C:h.types
o.render_lis:	C:h.allocate
o.render_lis:	C:h.ci_string
o.render_lis:	C:h.exception
o.render_lis:	C:h.os
o.render_lis:	C:h.list
o.render_lis:	C:h.bool
o.render_lis:	C:h.message
o.special:	^.c.special
o.special:	^.h.special
o.special:	C:h.list
o.special:	C:h.bool
o.special:	C:h.types
o.special:	^.h.font_set
o.special:	C:h.font
o.special:	C:h.os
o.special:	C:h.set
o.special:	C:h.bool
o.special:	C:h.allocate
o.special:	C:h.exception
o.special:	^.h.log
o.special:	C:h.message
o.special:	^.h.picture
o.special:	^.h.font_set
o.substitute:	^.c.substitute
o.substitute:	^.h.substitute
o.substitute:	C:h.ci_string
o.substitute:	C:h.message
o.substitute:	^.h.font_summary
o.substitute:	C:h.bool
o.substitute:	C:h.types
o.substitute:	^.h.log
o.substitute:	^.h.render_list
o.substitute:	C:h.bool
o.substitute:	^.h.sys_font_list
o.substitute:	C:h.list
o.substitute:	C:h.bool
o.sys_font_l:	^.c.sys_font_l
o.sys_font_l:	^.h.sys_font_list
o.sys_font_l:	C:h.list
o.sys_font_l:	C:h.bool
o.sys_font_l:	C:h.types
o.sys_font_l:	C:h.font
o.sys_font_l:	C:h.os
o.sys_font_l:	C:h.ci_string
o.sys_font_l:	C:h.exception
o.tex_font:	^.c.tex_font
o.tex_font:	^.h.tex_font
o.tex_font:	^.h.dviops
o.tex_font:	^.h.byte_stream
o.tex_font:	^.h.font_set
o.tex_font:	C:h.font
o.tex_font:	C:h.types
o.tex_font:	C:h.os
o.tex_font:	C:h.set
o.tex_font:	C:h.bool
o.tex_font:	^.h.renderer
o.tex_font:	^.h.real_font
o.tex_font:	C:h.bool
o.tex_font:	C:h.allocate
o.tex_font:	C:h.ci_string
o.tex_font:	C:h.error
o.tex_font:	C:h.exception
o.tex_font:	C:h.exception
o.tex_font:	C:h.list
o.tex_font:	C:h.bool
o.tex_font:	^.h.log
o.tex_font:	C:h.message
o.tex_font:	^.h.file
o.tex_font:	C:h.bool
o.tex_font:	^.h.font_file
o.tex_font:	^.h.substitute
o.tex_font:	^.h.tfm
o.tex_font:	C:h.bool
o.tex_font:	^.h.virtual_font
o.tex_font:	^.h.font_set
o.tfm:	^.c.tfm
o.tfm:	^.h.tfm
o.tfm:	C:h.bool
o.tfm:	C:h.types
o.tfm:	C:h.allocate
o.tfm:	C:h.ci_string
o.tfm:	C:h.exception
o.tfm:	C:h.os
o.tfm:	C:h.list
o.tfm:	C:h.bool
o.tfm:	C:h.message
o.tfm:	^.h.file
o.tfm:	C:h.bool
o.tfm:	^.h.file_error
o.tfm:	^.h.file
o.tfm:	^.h.font_file
o.viewer:	^.c.viewer
o.viewer:	^.h.viewer
o.viewer:	^.h.document
o.viewer:	^.h.viewer
o.viewer:	^.h.dvifile
o.viewer:	^.h.page
o.viewer:	^.h.font_table
o.viewer:	C:h.bool
o.viewer:	C:h.types
o.viewer:	^.h.font_set
o.viewer:	C:h.font
o.viewer:	C:h.os
o.viewer:	C:h.set
o.viewer:	C:h.bool
o.viewer:	^.h.tex_font
o.viewer:	^.h.dviops
o.viewer:	^.h.byte_stream
o.viewer:	^.h.font_set
o.viewer:	^.h.renderer
o.viewer:	^.h.real_font
o.viewer:	C:h.bool
o.viewer:	^.h.font_set
o.viewer:	^.h.units
o.viewer:	^.h.print_doc
o.viewer:	C:h.bool
o.viewer:	^.h.print_declarer
o.viewer:	C:h.bool
o.viewer:	C:h.displayfield
o.viewer:	C:h.toolbox
o.viewer:	C:h.wimp
o.viewer:	C:h.osspriteop
o.viewer:	C:h.messagetrans
o.viewer:	C:h.gadget
o.viewer:	C:h.numberrange
o.viewer:	C:h.macros
o.viewer:	C:h.menu
o.viewer:	C:h.saveas
o.viewer:	C:h.window
o.viewer:	C:h.keyboardshortcut
o.viewer:	C:h.scale
o.viewer:	C:h.window
o.viewer:	C:h.exception
o.viewer:	C:h.list
o.viewer:	C:h.bool
o.viewer:	C:h.message
o.viewer:	C:h.nev_wimp
o.viewer:	C:h.nevent
o.viewer:	C:h.nev_toolbox
o.viewer:	C:h.nevent
o.viewer:	C:h.save_buffer
o.viewer:	C:h.tbx
o.viewer:	^.h.choices
o.viewer:	^.h.magnifier
o.viewer:	^.h.page
o.viewer:	^.h.optionfile
o.viewer:	C:h.bool
o.viewer:	^.h.vprint_dbx
o.viewer:	^.h.vp_choices
o.viewer:	C:h.bool
o.viewer:	^.h.print_doc
o.virtual_fo:	^.c.virtual_fo
o.virtual_fo:	^.h.virtual_font
o.virtual_fo:	^.h.font_set
o.virtual_fo:	C:h.font
o.virtual_fo:	C:h.types
o.virtual_fo:	C:h.os
o.virtual_fo:	C:h.set
o.virtual_fo:	C:h.bool
o.virtual_fo:	C:h.allocate
o.virtual_fo:	C:h.exception
o.virtual_fo:	C:h.list
o.virtual_fo:	C:h.bool
o.virtual_fo:	C:h.message
o.virtual_fo:	^.h.command_processor
o.virtual_fo:	^.h.byte_stream
o.virtual_fo:	^.h.font_table
o.virtual_fo:	C:h.bool
o.virtual_fo:	^.h.font_set
o.virtual_fo:	^.h.tex_font
o.virtual_fo:	^.h.dviops
o.virtual_fo:	^.h.byte_stream
o.virtual_fo:	^.h.font_set
o.virtual_fo:	^.h.renderer
o.virtual_fo:	^.h.real_font
o.virtual_fo:	C:h.bool
o.virtual_fo:	^.h.file_error
o.virtual_fo:	^.h.file
o.virtual_fo:	C:h.bool
o.virtual_fo:	^.h.font_file
o.vprint_dbx:	^.c.vprint_dbx
o.vprint_dbx:	^.h.vprint_dbx
o.vprint_dbx:	^.h.vp_choices
o.vprint_dbx:	C:h.bool
o.vprint_dbx:	C:h.types
o.vprint_dbx:	^.h.print_doc
o.vprint_dbx:	C:h.bool
o.vprint_dbx:	^.h.print_declarer
o.vprint_dbx:	C:h.os
o.vprint_dbx:	C:h.macros
o.vprint_dbx:	C:h.numberrange
o.vprint_dbx:	C:h.toolbox
o.vprint_dbx:	C:h.wimp
o.vprint_dbx:	C:h.osspriteop
o.vprint_dbx:	C:h.font
o.vprint_dbx:	C:h.messagetrans
o.vprint_dbx:	C:h.gadget
o.vprint_dbx:	C:h.optionbutton
o.vprint_dbx:	C:h.pdriver
o.vprint_dbx:	C:h.draw
o.vprint_dbx:	C:h.jpeg
o.vprint_dbx:	C:h.radiobutton
o.vprint_dbx:	C:h.window
o.vprint_dbx:	C:h.keyboardshortcut
o.vprint_dbx:	C:h.exception
o.vprint_dbx:	C:h.message
o.vprint_dbx:	C:h.nev_toolbox
o.vprint_dbx:	C:h.nevent
o.vprint_dbx:	C:h.tbx
o.vprint_dbx:	^.h.vprint
o.vprint_dbx:	^.h.vp_choices
o.vprint_dbx:	^.h.print_doc
o.vp_font:	^.c.vp_font
o.vp_font:	^.h.vp_font
o.vp_font:	^.h.print_declarer
o.vp_font:	C:h.os
o.vp_font:	C:h.types
o.vp_font:	C:h.pdriver
o.vp_font:	C:h.draw
o.vp_font:	C:h.font
o.vp_font:	C:h.messagetrans
o.vp_font:	C:h.jpeg
o.vp_font:	^.h.font_set
o.vp_font:	C:h.font
o.vp_font:	C:h.set
o.vp_font:	C:h.bool
o.vp_iter:	^.c.vp_iter
o.vp_iter:	^.h.vp_iter
o.vp_iter:	^.h.print_doc
o.vp_iter:	C:h.bool
o.vp_iter:	C:h.types
o.vp_iter:	^.h.print_declarer
o.vp_iter:	C:h.os
o.vp_iter:	^.h.print_iter
o.vp_iter:	C:h.bool
o.vp_iter:	^.h.print_side
o.vp_iter:	^.h.vp_choices
o.vp_iter:	C:h.bool
o.vp_iter:	C:h.macros
o.vp_iter:	C:h.pdriver
o.vp_iter:	C:h.draw
o.vp_iter:	C:h.font
o.vp_iter:	C:h.messagetrans
o.vp_iter:	C:h.jpeg
o.vp_iter:	C:h.error
o.vp_iter:	C:h.exception
o.vp_iter:	C:h.exception
o.vp_iter:	C:h.message
o.vp_iter:	C:h.nevent
o.vp_iter:	C:h.toolbox
o.vp_iter:	C:h.wimp
o.vp_iter:	C:h.osspriteop
o.vp_iter:	C:h.hourglass
o.vp_iter:	^.h.vp_font
o.vp_iter:	^.h.print_declarer
o.vp_iter:	^.h.vp_side
o.vp_iter:	^.h.print_side
o.vp_iter:	^.h.print_doc
o.vp_iter:	^.h.vp_area
o.vp_iter:	^.h.print_declarer
o.vp_status:	^.c.vp_status
o.vp_status:	^.h.vp_status
o.vp_status:	^.h.print_rep
o.vp_status:	C:h.displayfield
o.vp_status:	C:h.types
o.vp_status:	C:h.toolbox
o.vp_status:	C:h.os
o.vp_status:	C:h.wimp
o.vp_status:	C:h.osspriteop
o.vp_status:	C:h.font
o.vp_status:	C:h.messagetrans
o.vp_status:	C:h.gadget
o.vp_status:	C:h.message
o.vp_status:	C:h.nevent
o.vp_status:	C:h.tbx
o.main:	^.c.main
o.main:	C:h.hourglass
o.main:	C:h.types
o.main:	C:h.os
o.main:	C:h.application
o.main:	C:h.bool
o.main:	C:h.nev_message
o.main:	C:h.nevent
o.main:	C:h.toolbox
o.main:	C:h.wimp
o.main:	C:h.osspriteop
o.main:	C:h.font
o.main:	C:h.messagetrans
o.main:	C:h.nev_wimp
o.main:	C:h.nevent
o.main:	C:h.shifting
o.main:	C:h.allocate
o.main:	^.h.choices
o.main:	^.h.document
o.main:	^.h.viewer
o.main:	^.h.document
o.main:	C:h.bool
o.main:	^.h.dvifile
o.main:	^.h.page
o.main:	^.h.font_table
o.main:	C:h.bool
o.main:	^.h.font_set
o.main:	C:h.font
o.main:	C:h.set
o.main:	C:h.bool
o.main:	^.h.tex_font
o.main:	^.h.dviops
o.main:	^.h.byte_stream
o.main:	^.h.font_set
o.main:	^.h.renderer
o.main:	^.h.real_font
o.main:	C:h.bool
o.main:	^.h.font_set
o.main:	^.h.units
o.main:	^.h.print_doc
o.main:	C:h.bool
o.main:	^.h.print_declarer
o.main:	^.h.font_summary
o.main:	C:h.bool
o.main:	^.h.log
o.main:	^.h.optionfile
o.main:	C:h.bool
o.main:	^.h.papersize
o.main:	C:h.bool
o.main:	^.h.render_list
o.main:	C:h.bool
o.main:	^.h.sys_font_list
o.main:	C:h.list
o.main:	C:h.bool
o.main:	MemCheck:h.MemCheck
o.main:	HierProf:h.HierProf
o.vp_area:	^.c.vp_area
o.vp_area:	^.h.vp_area
o.vp_area:	^.h.print_declarer
o.vp_area:	C:h.os
o.vp_area:	C:h.types
o.vp_area:	C:h.pdriver
o.vp_area:	C:h.draw
o.vp_area:	C:h.font
o.vp_area:	C:h.messagetrans
o.vp_area:	C:h.jpeg
o.vp_area:	C:h.allocate
o.vp_area:	C:h.box
o.vp_area:	C:h.debug_io
o.vp_side:	^.c.vp_side
o.vp_side:	^.h.vp_side
o.vp_side:	^.h.print_side
o.vp_side:	C:h.os
o.vp_side:	C:h.types
o.vp_side:	^.h.print_doc
o.vp_side:	C:h.bool
o.vp_side:	^.h.print_declarer
o.vp_side:	^.h.vp_area
o.vp_side:	^.h.print_declarer
o.vp_side:	C:h.debug_io
o.vp_side:	C:h.exception
o.page_diag:	^.c.page_diag
o.page_diag:	^.h.page_diag
o.page_diag:	^.h.font_set
o.page_diag:	C:h.font
o.page_diag:	C:h.types
o.page_diag:	C:h.os
o.page_diag:	C:h.set
o.page_diag:	C:h.bool
o.page_diag:	^.h.real_font
o.page_diag:	C:h.bool
o.page_diag:	C:h.debug_io
o.page_diag:	C:h.drawfile
o.page_diag:	C:h.osspriteop
o.page_diag:	C:h.draw
o.page_diag:	C:h.wimp
o.page_diag:	C:h.jpeg
o.page_diag:	C:h.macros
o.page_diag:	C:h.box
o.page_diag:	C:h.exception
o.page_diag:	C:h.shifting
o.page_diag:	C:h.messagetrans
o.page_diag:	C:h.allocate
o.page_diag:	^.h.draw_utils
o.page_diag:	C:h.drawfile
o.page_diag:	^.h.font_set
o.document:	^.c.document
o.document:	^.h.document
o.document:	^.h.viewer
o.document:	^.h.document
o.document:	C:h.bool
o.document:	C:h.types
o.document:	^.h.dvifile
o.document:	^.h.page
o.document:	^.h.font_table
o.document:	C:h.bool
o.document:	^.h.font_set
o.document:	C:h.font
o.document:	C:h.os
o.document:	C:h.set
o.document:	C:h.bool
o.document:	^.h.tex_font
o.document:	^.h.dviops
o.document:	^.h.byte_stream
o.document:	^.h.font_set
o.document:	^.h.renderer
o.document:	^.h.real_font
o.document:	C:h.bool
o.document:	^.h.font_set
o.document:	^.h.units
o.document:	^.h.print_doc
o.document:	C:h.bool
o.document:	^.h.print_declarer
o.document:	C:h.fileinfo
o.document:	C:h.toolbox
o.document:	C:h.wimp
o.document:	C:h.osspriteop
o.document:	C:h.messagetrans
o.document:	C:h.window
o.document:	C:h.keyboardshortcut
o.document:	C:h.gadget
o.document:	C:h.hourglass
o.document:	C:h.menu
o.document:	C:h.numberrange
o.document:	C:h.saveas
o.document:	C:h.osfile
o.document:	C:h.fileswitch
o.document:	C:h.allocate
o.document:	C:h.box
o.document:	C:h.debug_io
o.document:	C:h.exception
o.document:	C:h.list
o.document:	C:h.bool
o.document:	C:h.message
o.document:	C:h.nev_toolbox
o.document:	C:h.nevent
o.document:	C:h.save_buffer
o.document:	^.h.choices
o.document:	^.h.papersize
o.document:	C:h.bool
o.document:	^.h.print_doc
o.page:	^.c.page
o.page:	^.h.page
o.page:	^.h.font_table
o.page:	C:h.bool
o.page:	C:h.types
o.page:	^.h.font_set
o.page:	C:h.font
o.page:	C:h.os
o.page:	C:h.set
o.page:	C:h.bool
o.page:	^.h.tex_font
o.page:	^.h.dviops
o.page:	^.h.byte_stream
o.page:	^.h.font_set
o.page:	^.h.renderer
o.page:	^.h.real_font
o.page:	C:h.bool
o.page:	^.h.font_set
o.page:	C:h.macros
o.page:	C:h.allocate
o.page:	C:h.box
o.page:	C:h.debug_io
o.page:	C:h.error
o.page:	C:h.exception
o.page:	C:h.exception
o.page:	C:h.list
o.page:	C:h.bool
o.page:	^.h.log
o.page:	C:h.message
o.page:	C:h.save_buffer
o.page:	C:h.toolbox
o.page:	C:h.wimp
o.page:	C:h.osspriteop
o.page:	C:h.messagetrans
o.page:	^.h.command_processor
o.page:	^.h.byte_stream
o.page:	^.h.font_table
o.page:	^.h.draw_utils
o.page:	C:h.drawfile
o.page:	C:h.draw
o.page:	C:h.jpeg
o.page:	^.h.font_set
o.page:	^.h.mask
o.page:	^.h.picture
o.page:	^.h.font_set
o.page:	^.h.page_diag
o.page:	^.h.font_set
o.page:	^.h.real_font
o.page:	^.h.special
o.page:	C:h.list
o.page:	^.h.font_set
o.page:	^.h.units
o.print_core:	^.c.print_core
o.print_core:	^.h.print_core
o.print_core:	^.h.print_iterator
o.print_core:	C:h.bool
o.print_core:	C:h.types
o.print_core:	^.h.print_side
o.print_core:	C:h.os
o.print_core:	^.h.print_rep
o.print_core:	C:h.hourglass
o.print_core:	C:h.pdriver
o.print_core:	C:h.draw
o.print_core:	C:h.font
o.print_core:	C:h.messagetrans
o.print_core:	C:h.jpeg
o.print_core:	C:h.debug_io
o.print_core:	C:h.exception
o.print_core:	^.h.print_job
