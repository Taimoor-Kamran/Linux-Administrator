# 📦 Package Management in Linux

# Introduction

Package management in Linux is the process of installing, updating, upgrading, configuring, and removing software using package managers. Different Linux distributions use different package management systems.

## 🐧 Linux Distributions

### Debian-Based Distributions

1. Ubuntu
2. Debian
3. Linux Mint

### Package Tools

1. apt
2. dpkg

## Red Hat-Based Distributions

1. Red Hat Enterprise Linux (RHEL)
2. CentOS
3. Rocky Linux
4. AlmaLinux
5. Fedora

### Package Tools

1. yum
2. dnf
3. rpm

## 🔧 Package Managers Overview

 Distribution     | High-Level Tool | Low-Level Tool
 |----------------|-----------------|--------------|
 Ubuntu/Debian    | apt	            | dpkg
 |----------------|-----------------|--------------|
 RHEL/CentOS      | yum / dnf	    | rpm
 |----------------|-----------------|--------------|

- High-level tools → handle dependencies automatically.
- Low-level tools → manage packages directly.

[YUM Package Manager](yum.md)

## 📦 RPM (Red Hat Package Manager)

rpm is a low-level package management tool.

It allows installation, removal, and querying of packages directly.

⚠️ Limitation:
RPM does NOT resolve dependencies automatically.

### Install an RPM Package

- sudo rpm -i package-file.rpm

### Upgrade a Package

- sudo rpm -U package-file.rpm

### Install with Progress Output

- sudo rpm -ivh package-file.rpm

Options:

v → verbose output
h → shows progress bar

### Remove a Package

- sudo rpm -e package_name

### Query Installed Packages

rpm -qa

### Package Information

rpm -qi package_name

### View Configuration Files

rpm -qc package_name

## 🟦 DNF (Dandified YUM)

dnf is the modern replacement for yum used in newer Red Hat-based systems.

### List Packages

- sudo dnf list available
- sudo dnf list installed

### Install / Remove Packages

- sudo dnf install package_name
- sudo dnf remove package_name

### Update System
- sudo dnf update
- sudo dnf upgrade

### Search Packages

- sudo dnf search package_name

### Package Information

- sudo dnf info package_name

## 🟩 APT (Advanced Package Tool) — Ubuntu/Debian

apt is the primary package manager for Debian-based systems.

### Update Repository Information

- sudo apt update

Downloads the latest package list from repositories.

### Install Package

- sudo apt install package_name

### Remove Package

- sudo apt remove package_name

### Remove Unused Dependencies

- sudo apt autoremove

### Upgrade Installed Packages

- sudo apt upgrade

### Search for Packages

- apt search apache

or

- apt-cache search apache