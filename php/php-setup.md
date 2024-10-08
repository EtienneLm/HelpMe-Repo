# Installing PHP on Windows

This guide will walk you through the steps to install PHP on a Windows machine.

## Prerequisites

Before you start, make sure you have the following:
- A Windows operating system (Windows 10 or later recommended)
- Administrative access to your machine

## Steps to Install PHP

### Step 1: Download PHP

1. Go to the [PHP Downloads page](https://windows.php.net/download/).
2. Choose the appropriate version (for example, **PHP 8.x**).
3. Select the **Thread Safe** version for your system architecture (x64 for 64-bit or x86 for 32-bit).
4. Download the ZIP file (e.g., `php-8.x.x-Win32-vs16-x64.zip`).

### Step 2: Extract the ZIP File

1. Create a new directory for PHP (e.g., `C:\php`).
2. Extract the contents of the downloaded ZIP file into this directory.

### Step 3: Configure PHP

1. Navigate to the PHP directory (e.g., `C:\php`).
2. Rename the file `php.ini-development` to `php.ini`.
3. Open `php.ini` in a text editor (e.g., Notepad).
4. Configure your settings (optional). Common changes include:
   - Set the `extension_dir` to point to the `ext` directory:
     ```ini
     extension_dir = "ext"
     ```
   - Uncomment extensions you need (remove the `;` at the beginning of the line). For example, to enable the `mysqli` extension, find and uncomment:
     ```ini
     extension=mysqli
     ```

### Step 4: Add PHP to the System Path

1. Right-click on **This PC** or **Computer** on your desktop or in File Explorer and select **Properties**.
2. Click on **Advanced system settings**.
3. Click on the **Environment Variables** button.
4. In the **System variables** section, find the `Path` variable and select it, then click **Edit**.
5. Click **New** and add the path to the PHP directory (e.g., `C:\php`).
6. Click **OK** to close all dialogs.

### Step 5: Verify Installation

1. Open a new Command Prompt window (to ensure the new PATH is recognized).
2. Type the following command and press Enter:
   ```
   php --version
   ```
