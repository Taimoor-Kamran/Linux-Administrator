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
