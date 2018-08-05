GFXView (c) Paul Field
~~~~~~~~~~~~~~~~~~~~~~
GFXView is a program demonstrating how to use OSLib and the Toolbox to
write a simple Wimp application. It also demonstrates how to handle errors
by using exceptions (in C).

The program will display sprites, Draw files and JPEGs which are
double-clicked or dropped onto its icon on the icon bar.

Note that JPEGs are only supported if you have the SpriteExtend
module v0.99 or later (this is present in RISC OS 3.6).
The program will not attempt to load JPEGs with earlier versions
of SpriteExtend.


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
GFXView is a reasonably complicated example that demonstrates the
implementation of a multi-document application and also shows how to load
files and render various graphics formats.

For a simpler example see !Tree which is only single-document (and so has
simpler 'viewer' code). Note that !Tree does have some advanced features
such as file saving (using ToolLib's facilities) and Draw file construction.


GFXView's files
~~~~~~~~~~~~~~~

main        This is the code for initialising and quitting your program.
            It shows how to use ToolLib's application framework.
            
picture     Code which provides a uniform 'picture' interface for differing
            format such as Sprite, Draw or JPEG files. This is one way of
            implementing a C++ abstract base class in C (see CAUGers 3:1
            p9-14 which shows this arrangement as a class diagram).
            
draw_pic    Code for handling draw file 'pictures'. In C++ this would be
            a class derived from picture.            
            
sprite_pic  Code for handling sprite 'pictures'. In C++ this would be
            a class derived from picture.

jpeg_pic    Code for handling jpeg 'pictures'. In C++ this would be
            a class derived from picture.
            
viewer      The code for handling a window containing a sprite (including
            handling the 'scale' dialogue box). Demonstrates:
              Loading files
              Handling multiple 'documents'
              How to manage a window that needs to be redrawn by the application
              Using debug code to validate data structures in event handlers
              
Help!
~~~~~
GFXView's main aim is to give you an example of a reasonably
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