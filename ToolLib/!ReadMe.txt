ToolLib v1.13 - 14/6/1996 (c) Paul Field
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
ToolLib is a library of functions for OSLib/Toolbox programmers. Although
fairly small at the moment, it has some powerful features such as exception
handling and interfaces to the Toolbox SaveAs system that make Type 3 saving
(i.e. in-memory or file) a complete doddle.

You'll find a fair amount of documentation in the library header files
and the example applications demonstrate how to use the major features of
the library.


Facilities provided by ToolLib
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

allocate     This is a simple wrapper for the malloc() functions which
             throws exceptions when memory allocation fails.
            
application  This is an application framework which sets up the facilities
             a toolbox application will need (e.g. toolbox initialisation,
             Quit message/event handlers, error handlers) and performs
             the event polling loop.
            
backtrace    Generates a stack backtrace on stderr (useful for
             debugging - especially exceptions).

box          Various routines for dealing with os_box (e.g. clipping,
             detecting overlaps).

ci_string    Routines for case-insensitive comparison of strings

error        This is a system for reporting errors (mainly exceptions).

exception    This is a system for handling errors using an exception system
             similar to C++. It's not as powerful as C++'s exceptions but
             it's far better (easier to use, reliable) than passing error
             codes around (or not checking for errors at all).
            
fast_trig    Routines for performing trigonomic functions very quickly.

list         A list data type.

message      An interface to MessageTrans which enables you to look up
             messages from the Messages files.
            
nevent       An event handling system, similar to Acorn's event library
             but with more advanced facilities and debugging checks.

nev_message  Allows you to register handlers for Wimp messages.

nev_toolbox  Allows you to register handlers for Toolbox events.

nev_wimp     Allows you to register handlers for Wimp events.

saver        In combination with save_buffer this completely handles type 3
             data transfer from a saveas object.

save_buffer  Provides a uniform interface for data transfer either to a file
             or another application (using type 3 transfer).

set          A set data type.

shifting     An alternative to flex which throws exceptions on error and
             provides a 'better' interface (including debug checks).

shifting_send Allows data from shifting blocks to be sent to the save buffer.
            
tbx          General toolbox utilities (currently just one function to return
             the task name).

text_plot    Functions for plotting text using the desktop font (using
             Wimp_TextOp in RISC OS 3.5+ and an alternative method in
             earlier OS versions).

Further details of each system is given in the system's header file.
A detailed introduction to the exception handling system appears
in CAUGers 3:2.


Compiling an application
~~~~~~~~~~~~~~~~~~~~~~~~
You will need to link your application against the following libraries:

  ToolLib:o.ToolLib  (or ToolLib:o.ToolLibDbg for the debug version)
  C:o.flexlib        (only necessary if you use the shifting system)
  C:o.stubs
  OSLib:o.OSLib

Have a look at the example applications and their MakeFiles for a starting
point.


The debug version
~~~~~~~~~~~~~~~~~
The library ToolLib:o.ToolLibDbg is a debug version of the ToolLib library.
It performs a large number of integrity checks (using assert()), for example
on function arguments, and also produces a stack backtrace on stderr whenever
an exception occurs (so it's easy to find out where things went wrong).

When using the debug version of ToolLib you are advised to redirect the
standard error stream as described in CAUGers 1:3 and 1:4.
All of the example programs redirect the error stream to pipe:$.debug - 
look at their initialisation code to see how.


The memory-checking version
~~~~~~~~~~~~~~~~~~~~~~~~~~~
The library ToolLib:o.ToolLibMem is a memory-checking version of the
ToolLib library for use with Julian Smith's MemCheck system.
The library will automatically initialise the system and make these
calls:
   MemCheck_SetStoreMallocFunctions(1);
   MemCheck_InterceptSCLStringFunctions();

The shifting system will automatically register its memory blocks with the
MemCheck system.


The profiling version
~~~~~~~~~~~~~~~~~~~~~
The library ToolLib:o.ToolLibPrf is for use with Julian Smith's
HierProf profiling system. If you use ToolLib's application.h
then profiling will be automatically initialised and output
automatically generated when the program terminates.


The future
~~~~~~~~~~
As I continue to develop applications I will extend this library.
If you develop useful routines based on OSLib and/or using exceptions please
send them to me so I can include them in the library.


Help!
~~~~~
If there's anything you don't understand please let me know so I can improve
the library and its documentation. If you have any sensible criticisms of the
code (stylistic, organisational or whatever) please also let me know.


History
~~~~~~~
v1.10 - added abstract data types: list and set

v1.11 - added shifting_send
        changed to use Makatic for building
        added memory-checking build
        added profiling build
        changed action_QUIT to 0x82a91 to match Toolbox quit objects' quit message

v1.12 - new nevent system
        changes to list and set ADTs (to use list_ptr and set_ptr)
        added ci_string
        exception now catches SIGABRT (catches assert() failures)
        changes to error and message: error now reports strings and
           so messages doesn't need to look up messages for error blocks.
        added error_report_information()
        added message_lookup_in_list()
           

v1.13 - added text_plot




Known problems/limitations
~~~~~~~~~~~~~~~~~~~~~~~~~~
There is currently no way to deal with user_message_acknowledge in the 
nevent system

Invlidation of list_ptrs by certain list calls is not currently checked
by the list system.

List test harness doesn't test list_ptr violations

Set is based on lists and so uses a linear search algorithm: using a
(appoximately) balanced tree data structure (e.g. AVL trees,
red-black trees) would be better.



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
