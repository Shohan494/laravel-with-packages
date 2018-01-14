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

#### Laravel Decomposer to Check Dependencies

- composer require lubusin/laravel-decomposer
- need to add in (config/app.php) package service provider: Lubusin\Decomposer\DecomposerServiceProvider::class,
- need to add in web routes: Route::get('decompose','\Lubusin\Decomposer\Controllers\DecomposerController@index');

#### Laravel Log Viewer

- composer require rap2hpoutre/laravel-log-viewer
- need to add in (config/app.php) package service provider: Rap2hpoutre\LaravelLogViewer\LaravelLogViewerServiceProvider::class,
- need to add in web routes: Route::get('logs', '\Rap2hpoutre\LaravelLogViewer\LogViewerController@index');

#### Arcanedev/logviewer is installed and will be configured later

#### Laravel Tracy

- composer require recca0120/laravel-tracy
- need to add in (config/app.php) package service provider:     Recca0120\LaravelTracy\LaravelTracyServiceProvider::class,
- run this command: php artisan vendor:publish --provider="Recca0120\LaravelTracy\LaravelTracyServiceProvider"
- edit the created config file as package doc