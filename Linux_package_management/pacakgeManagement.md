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

## APT (Advanced Package Tool) — Ubuntu/Debian

APT = Advanced Package Tool

APT is the default package manager for Debian-based systems like Debian, Ubuntu, and Linux Mint. It installs, updates, upgrades, and removes packages while automatically handling dependencies from online repositories.

# basic commands

apt install package_name

# Install a package.

apt update

# Update package repository list.

apt upgrade

# Upgrade installed packages.

apt remove package_name

# Remove a package.

apt search package_name

Search for a package.