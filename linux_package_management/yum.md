## 🟥 YUM (Yellowdog Updater Modified)

yum is a package manager used in older Red Hat and CentOS systems.

It automatically handles dependency resolution during installation, updates, and removal of packages.

### Install and Remove Packages

- sudo yum install nginx
- sudo yum remove nginx

### Update or Upgrade Packages

- sudo yum update package_name
- sudo yum upgrade package_name

### View Available Options

- yum --help

###  Check Available Updates

- sudo yum check-update

### View Package History

Shows package activities with date and time.

- sudo yum history

### Undo or Redo Transactions

- sudo yum history undo <ID>
- sudo yum history redo <ID>
