Tree  (c) Paul Field
~~~~~~~~~~~~~~~~~~~~
Tree is a program demonstrating how to use OSLib and the Toolbox to
write a simple Wimp application. It also demonstrates how to handle errors
by using exceptions (in C).


Compiling
~~~~~~~~~
To compile you will need to have Julian Smith's Makatic installed.

The source code and 'build applications' are in the Builds directory.

There are three ways to compile the program (three "builds"): double-click
on !Debug to compile the debug version of the program; double-click
on !Release to compile the production version; double-click on
!MemCheck to build the memory checking version (you will need
Julian Smith's/Warm Silence Software's C Tools for this).

The WimpSlot set up in !Run will need to be increased to run the debug
or memory-checking versions.

Note that debug information is sent to the file pipe:$.debug.


General notes
~~~~~~~~~~~~~
Tree is not designed to be a "multi-document" (in this case multi-tree)
program; there is a single parameter window and a single tree display window.
This makes the program fairly simple and thus a good example for beginners
investigating Toolbox programming.

!GFXView is intended as a more advanced example which demonstrates, amongst
other things, how to implement a multi-document application.

Note that !Tree does demonstrate some advanced features such as file saving
(using ToolLib's 'saver' and 'save_buffer' facilities) and Draw file
construction.


Tree's files
~~~~~~~~~~~~

diagram_save   This saves lines as a Draw file using ToolLib's saver and
               save_buffer facilities.

line_plotter   This is a particular sort of line_processor (see below) that
               processes lines by plotting them on the screen.
             
line_processor This is an abstract definition of a system that processes lines.
               It enable the tree calculating function (see below) to generate
               lines without committing to a use for those lines (e.g. putting
               them on the screen, or putting them in a Draw file).
               In C++ this would be an abstract base class but note that this
               C implementation only allows one instantiation of each
               line_processor type (e.g. you can't have two line_storers).
               GFXView's 'picture' overcomes this limitation but the code
               is more complicated.
               
line_storer    This is a particular sort of line_processor that processes
               lines by storing them. Additional functions are provided for
               accessing the stored lines. Note that the 'shifting' memory
               manager is used.
               
main           This is the code for initialising and quitting your program.
               It shows how to use ToolLib's application framework.

tree           This is the main tree drawing code. Note how it is independent
               of any operating system calls or uses for the lines it generates.
               This is important because this code may need to be used in a
               PC program (this tree program actually has a serious use,
               believe it or not).

treeparams     This handles the tree parameters window. It demonstrates how
               to manage a dialogue box and read values from it.

treewindow     This handles the tree display window. It demonstrates how to use
               a redraw loop to draw the contents of a window.

              
Help!
~~~~~
!Tree was developed for my brother who is planning to use
computer-generated trees in a learning paradigm for his psychology Ph.D.
However, it will hopefully act as an example of a reasonably
well-written Toolbox application using OSLib. If there's anything you don't
understand please let me know so I can improve the program. If you have
any sensible criticisms of the code (stylistic, organisational or whatever)
please also let me know.


Contact details
~~~~~~~~~~~~~~~
Paul Field
Editor of CAUGers
346 Chadwell Heath Lane
Chadwell Heath
Romford
Essex
RM6 4YH
UK

phone:   uk:   0 181 598 9676
     non-uk: +44 181 598 9676

email: paul.field@dial.pipex.com