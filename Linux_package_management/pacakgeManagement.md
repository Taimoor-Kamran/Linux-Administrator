# Pacakge Management In Linux

Package management in Linux is the process of installing, updating, upgrading, configuring, and removing software using package managers. Different Linux distributions use different package management systems.

## Linux Distribution 

### Debian-Based Distributions

- Ubuntu
- Debian
- Linux Mint

### Package Tools

- apt
- dpkg

## Red Hat-Based Distributions

### Red Hat Enterprise Linux (RHEL)

- CentOS
- Rocky Linux
- AlmaLinux
- Fedora

### Package Tools

- yum
- dnf
- rpm

# Package Managers Overview

|Distribution   |High-Level Tool   |Low-Level Tool|
|---------------|------------------|--------------|
|Ubuntu/Debian	| apt              |	dpkg      |
|RHEL/CentOS	|yum / dnf         |	rpm       |


- High-level tools → handle dependencies automatically.
- Low-level tools → manage packages directly.

## APT (Advanced Package Tool) — Main Package Manager

APT is the default package manager for Debian-based systems like Debian, Ubuntu, and Linux Mint. It installs, updates, upgrades, and removes packages while automatically handling dependencies from online repositories.

### Linux Package Management Commands (WSL Ubuntu)

## Update & Upgrade

### Command Description 

- sudo apt update

Refreshes the package list from repositories (doesn't install anything).

- sudo apt upgrade

Upgrades all installed packages to their latest versions

- sudo apt full-upgrade

Like upgrade, but also removes conflicting packages if needed

- sudo apt dist-upgrade

Handles changing dependencies with new package versions

## Install & Remove

### Command Description

- sudo apt install package-name

Installs a package

- sudo apt install package1 package2

Installs multiple packages at once

- sudo apt remove package-name

Removes a package but keeps its config files

- sudo apt purge package-name

Removes a package along with its config files

- sudo apt autoremove

Removes unused dependency packages automatically

## Search & Info

### Command Description 

- apt & search keyword

Searches for packages by keyword

- apt show package-name

Shows detailed info about a package

- apt list --installed

Lists all installed packages

- apt list --upgradable

Lists packages that have available updates

- dpkg -l

Lists all installed packages (low-level)

- dpkg -l | grep name

Filters installed packages by name

## Clean Up

### Command Description

- sudo apt clean

Clears the local cache of downloaded .deb files.

- sudo apt autoclean

Removes only outdated cached packages

DPKG — Low-Level Package Tool

### Command Description

- sudo dpkg -i file.deb

Installs a .deb package file manually.

- sudo dpkg -r package-name

Removes a package

- sudo dpkg -P package-name

Purges a package and its config files.

- dpkg -s package-name

Shows status/info of an installed package

- dpkg -L package-name

Lists all files installed by a package.

- dpkg -S <file>

Finds which package owns a specific file

## SNAP — Universal Package Manager

### Command Description

- sudo snap install <package>

Installs a snap package

- sudo snap remove <package>

Removes a snap package

- snap list

Lists all installed snap packages

- sudo snap refresh

Updates all snap packages

- snap find <keyword>

Searches for snap packages