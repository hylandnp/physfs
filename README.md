# PhysFS

"PhysicsFS"; a portable, flexible file i/o abstraction:

  http://icculus.org/physfs/
  
 This modified version based off of another custom fork:

  https://github.com/samueldr/physfs

Please see the docs directory for documentation, licensing, and information.

## Added Features

This fork adds the ability to open overlapping (i.e. different versions of the same file name/path in the search path) file handles, for cases where it is preferable to merge the data contained within, rather than overwriting/replacing earlier versions in the search path.

```c
// New functions added:
PHYSFS_openReadMulti(const char* filename)
PHYSFS_closeMulti(PHYSFS_File** handles)
```

## TODOs

1. Modify CMake files to support some extended build configuration.
2. Maybe look into fixing build issue for 7z support (on Windows) and ISO9660 (on Linux). Unchecked in CMake for the moment.
