# Creating a Laravel Project with Composer

This guide will walk you through the steps to create a new Laravel project using Composer.

## Make sure you have the following installed on your machine:

- **PHP** (version 8.0 or higher)
- **Composer** (dependency manager for PHP) [Official Composer website](https://getcomposer.org/download/).
- **A web server** (such as Apache or Nginx)
- **Node.js** and **npm** (for front-end dependencies, optional)

## Steps to Create a Laravel Project

### Step 1: Navigate to Your Project Directory

Use the `cd` command to navigate to the directory where you want to create your Laravel project:

```
cd /path/to/your/directory
```

### Step 2: Create a New Laravel Project
```
composer create-project --prefer-dist laravel/laravel project-name
```

### Step 3: Navigate into Your Project Directory
```
cd project-name
```

### Step 4: Set Up Environment File
```
cp .env.example .env
```

### Step 5: Generate Application Key
```
php artisan key:generate
```

### Step 6: Configure Your Database
```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database_name
DB_USERNAME=your_database_user
DB_PASSWORD=your_database_password
```

### Step 7: Run Migrations (Optional)
```
php artisan migrate
```

### Step 8: Serve Your Application
```
php artisan serve
```


