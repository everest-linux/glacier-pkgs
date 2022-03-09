# glacier-pkgs
Collection of packages used by the Glacier package manager.

To submit a package, the following requirements must be met:
  - An information file named "{package_name}-pkginfo.json", which must contain the package's name, version, description, source tree size, executable size, and any dependencies that Glacier will install, and the name of the license (if it utilizes a license that is not GPL 3.0)
  - A script named INSTALL.sh describing what steps must be taken to install the package
  - A script named UPDATE.sh describing what steps must be taken to update the package
  - A script named REMOVE.sh describing what steps must be taken to remove the package
  - The executable
  - (optional) a copy of the license (if it utilizes a license that is not GPL 3.0)
