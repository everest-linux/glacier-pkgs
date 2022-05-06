# glacier-pkgs

Collection of packages used by the Glacier package manager.

There are 2 different packaging methods.

The first, which is used if your program is relatively simple (only one or 2 executables installed), is relatively simple.

The second, which is used for more complex programs (a lot of executables installed and a lot of programs made), compiles said programs from source.

Regardless of which method you choose, all archives must have the following files:

- An information file named "{package_name}-pkginfo.json", which must contain the package's name, version, description, source tree size, executable size, and any dependencies that Glacier will install, and the name of the license (if it utilizes a license that is not GPL 3.0)
- A script named INSTALL.sh describing what steps must be taken to install the package
- A script named UPDATE.sh describing what steps must be taken to update the package
- A script named REMOVE.sh describing what steps must be taken to remove the package
- The executable (or a makefile and configure script if the program will be compiled from source)
- (optional) a copy of the license (if it utilizes a license that is not GPL 3.0)

In the world repository, there should only be system software
In the galaxy repository, there should be GPL only software
In the universe repository, there can only be open source software (any license)
In the multiverse repository, there should only be proprietary software
