# OctoberCMS Build 306 - Starter Kit

## Included
* Demo theme from OctoberCMS
* [Blank Bootstrap 3 theme](http://octobercms.com/theme/krisawzm-blank-bootstrap) with Font Awesome, jQuery and built using LESS
* .env.example file for environment configuration

##Requirements

	PHP >= 5.4.0
	MCrypt PHP Extension

Installation instructions for the mcrypt extension are available [here](http://php.net/manual/en/mcrypt.installation.php).

##How to Install
### Step 1: Get the code
#### Option 1: Git Clone

```bash
$ git clone https://github.com/surahmans/OctoberCMS-Starter-Kit.git octobercms
```

#### Option 2: Download the repository

    https://github.com/surahmans/OctoberCMS-Starter-Kit/archive/master.zip

### Step 2: Use Composer to install dependencies
#### Option 1: Composer is not installed globally

```bash
$ cd octobercms
$ curl -s https://getcomposer.org/installer | php
$ php composer.phar install
```

#### Option 2: Composer is installed globally

```bash
$ cd octobercms
$ composer install
```

### Step 3: Configure Environments
copy the .env.example file to .env 
```bash
cp .env.example .env
```
Edit your .env file like below
```bash
APP_DEBUG=true
APP_KEY=SomeRandomString
APP_URL=http://localhost

DB_HOST=localhost
DB_DATABASE=homestead
DB_USERNAME=homestead
DB_PASSWORD=secret

CACHE_DRIVER=file
SESSION_DRIVER=file
QUEUE_DRIVER=sync
```

Generate the app key
```
php artisan key:generate
```

### Step 4: Populate Database tables
Run this command will build the database tables
```bash
php artisan october:up
```

### Step 5: Start Page
```bash
php artisan serve
```
Open in your browser, http://localhost:8000

### Step 6: Backend page
You can access the backend url at http://localhost:8000/backend
```
username: admin
password: admin
```

## License

This is free software distributed under the terms of the MIT license

## Additional information

Inspired by and based on [Laravel-4-Bootstrap-Starter-Site](https://github.com/andrewelkins/Laravel-4-Bootstrap-Starter-Site)

Any questions, feel free to [contact me](http://twitter.com/surahmans).
