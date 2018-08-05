--------------------
N.B. If you don't use OSLib then you'll need to edit 'bool.h' slightly
details are given in that file.

--------------------
This small library contains a list and a queue abstract data type.
There are two versions of the library:

ADTLib:o.ADTLib   is the "production" version of the library
ADTLib:o.ADTLibD  is the "debugging" version of the library

The debugging version contains debugging code that checks that you
are using the library correctly and tells you what's up if you mis-use it.
You should, however, link against the production version for the release
version of your code. I'd advise using !ProjMan (available on CAUGers
disc 1:2 or from the CAUG sofware library) because it supports debug
libraries.

In the 'c' directory you'll also find test harnesses that check the
data types and the debugging code.

If you are interested in adding data types to this library (e.g. trees,
stacks, tables, different implementations of lists) then please contact me.

Paul Field
346 Chadwell Heath Lane
Chadwell Heath
Romford
Essex
RM6 4YH
UK

Phone: (+44 or 0) 181 598 9676
email: paulf@dcs.qmw.ac.uk
       caugers@accu.org
