comfigure
=========

A comfortable way to manage ./configure options.

Usage
----------
$ ./comfigure help
comfigure 1.3 Copyright 2002 Jochen Suckfuell, License: GNU GPL
Usage: comfigure [command(s)] <configure options>

If no command is given, supplied configure options will be stored. If no
command and no configure options are given, the last used options will be used
if possible.

Commands are:
   interactive  ask each time before using stored options.
                (this is the default if the version has changed)
   new          force new entry, even if no options are given
   use_old      use old options without asking even if the stored version is
                older and there are new configure options (only applies if no
                configure options are given)
   add          add more options to the stored options
   show         show configuration for the current directory or for all named
                programs and exit
   showall      show all known programs with version and date of configuration
                and exit
   forget       forget configuration for the current directory or for all named
                programs and exit. Everything after the 'forget' command will
                be interpreted as a program name (even 'interactive', so be
                careful!).
   exec         take the following argument as executable instead of
                './configure'
   help         display this help and exit
   --help       invokes './configure --help' and exits


Sources
-----------
https://github.com/sujo/comfigure

