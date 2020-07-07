# pcr-toolkit

The PCR utility and related tools supports routines written in PL/I to be nucxloaded
into CMS storage and then invoked as either CMS commands, Rexx functions and sub-
routines, or CMS "immediate" commands. Multiple PL/I routines can be loaded and
managed at once, all sharing common data structures.

PCR is similar to the CMS **NUCXLOAD** and **NUCXDROP** commands, but is designed
to work with PL/I modules, and allows them to share data structures and retain allocated
data structures between invocations. Modules are given a logical name of which they are
invoked, in addition to a nucleus name (_nucxname_) with which they are loaded. The logical name can be
invoked either as a Rexx function or subroutine, as a normal CMS command through
the command line, as a CMS immediate command, or as a subcommand environment
handler.

PCR makes creating these types of routines much easier as they can be now written in
PL/I instead of Assembler.
