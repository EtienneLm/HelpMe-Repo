# Installing Composer

This guide will walk you through the steps to install Composer, the dependency manager for PHP.

## Prerequisites

Make sure you have the following installed on your machine:
- PHP (version 7.2.5 or higher)
- A command line interface (CLI) or terminal

## Steps to Install Composer

### Step 1: Download the Composer Installer
Open your terminal and run the following command to download the Composer installer script:

```
php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
```

### Step 2: Verify the Installer SHA-384
It’s a good practice to verify the installer’s SHA-384 to ensure its integrity. Run the following command to get the latest installer SHA-384 from the Composer website:
```
HASH="$(php -r "echo hash_file('SHA384', 'composer-setup.php');")"
```
Then compare the output against the latest SHA-384 hash provided on the Composer website. If it matches, proceed to the next step.

### Step 3: Install Composer Globally
```
php composer-setup.php --install-dir=/usr/local/bin --filename=composer
```

### Step 4: Remove the Installer
After installation, remove the installer script:
```
php -r "unlink('composer-setup.php');"
```

### Step 5: Verify Installation
To verify that Composer was installed correctly, run:
```
composer --version
You should see the version number of Composer displayed in the terminal.
```

### Step 6: Update Composer (Optional)
To update Composer to the latest version, use the following command:
```
composer self-update
```
