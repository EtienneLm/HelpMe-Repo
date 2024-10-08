# Creating a Laravel Project with Composer

This guide will walk you through the steps to create a new Laravel project using Composer.

## Prerequisites

Before you begin, make sure you have the following installed on your machine:

- **PHP** (version 8.0 or higher)
- **Composer** (dependency manager for PHP)
- **A web server** (such as Apache or Nginx)
- **Node.js** and **npm** (for front-end dependencies, optional)

## Steps to Create a Laravel Project

### Step 1: Install Composer

If you haven't installed Composer yet, follow these steps:

1. Download the Composer installer from the [official Composer website](https://getcomposer.org/download/).
2. Follow the installation instructions for your operating system.

### Step 2: Open a Terminal or Command Prompt

- On **Windows**, you can use Command Prompt or PowerShell.
- On **macOS** or **Linux**, open the Terminal.

### Step 3: Navigate to Your Project Directory

Use the `cd` command to navigate to the directory where you want to create your Laravel project:

```
cd /path/to/your/directory
```

### Step 4: Create a New Laravel Project
```
composer create-project --prefer-dist laravel/laravel project-name
```

Step 5: Navigate into Your Project Directory
```
cd project-name
```

Step 6: Set Up Environment File
```
cp .env.example .env
```

Step 7: Generate Application Key
```
php artisan key:generate
```

Step 8: Configure Your Database
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_user
DB_PASSWORD=your_database_password
```

Step 9: Run Migrations (Optional)
```
php artisan migrate
```

Step 10: Serve Your Application
```
php artisan serve
```


