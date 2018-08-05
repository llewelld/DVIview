An overview of the example programs
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
All programs are provided with a !ReadMe file which gives details of the
program's structure and operation. This section gives an overview of the
examples and what you can learn from them.


Text
-----
If you're a beginner, start with this program. It shows how to:
 * Initialise an application using ToolLib
 * Handle a single window whose contents must be redrawn by the application
 * Use Toolib's text_plot facilities


Click
-----
If you understand !Text, move on to this application. It shows how to:
 * Initialise an application using ToolLib
 * Handle errors using an exception-handling mechanism
 * Handle a single window whose contents must be redrawn by the application
 * Handle mouse clicks in the window
 * Use a data structure to store the contents of the window (in contrast to
   a non-Wimp program where you just plot on the screen)


Tree
----
This is a more complicated example but, like Click, is still
"single-document". It shows how to:
 * Initialise an application using ToolLib
 * Handle errors using an exception-handling mechanism
 * Handle a single window whose contents must be redrawn by the application
 * Handle a dialogue box containing gadgets
 * Save a Draw file
 * Save using type 3 (i.e. in-memory or file) data transfer using ToolLib's
   facilities
 * Abstract an algorithm (i.e. a tree building algorithm) from implementation
   details (i.e. what to do with the lines - plot them, save them, put them
   in a Draw file etc...)
   

GFXView
-------
This is a multi-document example. It shows how to:
 * Initialise an application using ToolLib
 * Handle errors using an exception-handling mechanism
 * Handle multiple 'documents' each of which appears in a separate window
 * Handle scaling and a scale dialogue box
 * Load and render Sprites (including 'deep' sprites on RISC OS 3.5 upwards)
 * Load and render Draw files
 * Load and render JPEGs (on RISC OS 3.6)
 * Organise a program well:
     - The 'viewer' is separated from the data it views
     - The different graphics formats are abstracted by 'picture' which
       presents a uniform interface hiding the implementation details of
       a particular graphics format. This makes the viewer code simpler and
       it's very easy to add new graphics formats.
     - Each graphics format is separated into a separate file
   This organisation separates code in to groups of related code which should
   make the program easier to understand and maintain. Note that the picture
   abstraction would be an abstract base class in C++ with draw_pic,
   sprite_pic and jpeg_pic derived from it.


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