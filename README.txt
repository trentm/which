which.py -- a portable GNU which replacement
============================================

Home            : http://code.google.com/p/which/
License         : MIT (see LICENSE.txt)
Platforms       : Windows, Linux, Mac OS X, Unix
Dev Status      : mature, has been heavily used in a commercial product for
                  a number of years
Requirements    : Python >= 2.3


`which.py` is a small GNU-which replacement. It has the following
features:

  * it is portable (Windows, Linux, Mac OS X, Un*x); 
  * it understands PATHEXT and "App Paths" registration on Windows (i.e. it
    will find everything that `start` does from the command shell); 
  * it can print all matches on the PATH; 
  * it can note "near misses" on the PATH (e.g. files that match but may not,
    say, have execute permissions); and 
  * it can be used as a Python module. 

