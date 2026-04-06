## DPKG = UBUNTU/DEBIAN Package Manager

dpkg is a low-level package management tool used in Debian and Ubuntu systems.
It installs, removes, and provides information about .deb packages but does not resolve dependencies automatically.

### how to install a package

dpkg -i package-file.deb

Installs a .deb package manually.

## how to remove a package

dpkg -r package_name

Removes the package but keeps configuration files.

## remove package completely (with config files)

dpkg -P package_name

Deletes package including configuration files.

## upgrade or reinstall a package

dpkg -i package-file.deb

Installs newer version if already installed.

## list all installed packages

dpkg -l

Shows all installed packages on the system.

## check if a package is installed

dpkg -l | grep package_name

Search installed package.

## show package information

dpkg -s package_name

Displays package details and status.

## list files installed by a package

dpkg -L package_name

Shows all files installed by the package.

## find which package owns a file

dpkg -S /path/to/file

Identifies package related to a file.

## view dpkg logs

less /var/log/dpkg.log

Shows package installation and removal history.

## fix broken dependencies (using apt)

apt install -f

Fixes dependency issues after dpkg installation.