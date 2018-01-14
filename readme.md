## Laravel Packages Trial
- OS - Ubuntu 16.04

##### Install Laravel 5.5 First and change your directory to your project folder

#### Homestead Per Laravel Project

- composer require laravel/homestead --dev
- php vendor/bin/homestead make
- sudo gedit /etc/hosts
- edit the hosts file with adding this line: 192.168.10.10  homestead.test
- vagrant up

##### You will find Laravel running on your url at: http://homestead.test

#### Laravel Extended File Generator

- composer require laracasts/generators --dev

Now we can make:

- Migrations With Schema
- Pivot Tables
- Database Seeders

#### Laravel Api Doc Generator

- composer require mpociot/laravel-apidoc-generator