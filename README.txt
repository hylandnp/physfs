
PhysicsFS; a portable, flexible file i/o abstraction:

  http://icculus.org/physfs/
  
This modified version based off of another custom fork:

  https://github.com/samueldr/physfs

Please see the docs directory for documentation, licensing, and information.

####################################################################################

TODOs:
  1) Modify CMake files to support some extended build configuration.
  2) Publish modified 'openReadMulti' & 'closeMulti' functions (that allow access to all versions of overlapping files).

ALSO:
  1) Maybe look into fixing build issue for 7z support (on Windows) and ISO9660 (on Linux). Should uncheck their CMake options by default for the moment.
