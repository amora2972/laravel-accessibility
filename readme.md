#### Under Development

## Laravel Accessibility

This package helps with a variety of common accessibility problems.
The package adds a number of helpful accessibility features with a minimum amount of setup or expert knowledge.

## Notice
This repo was taken from oh4d / laravel-accessibility, and modified to work with laravel v8.0

## Installation

Require this package with composer.

```shell
composer require oh4d/laravel-accessibility dev-dev
```

Laravel 5.5 uses Package Auto-Discovery, so doesn't require you to manually add the ServiceProvider.

The Accessibility will be enabled by default, to change that update your .env file.
See more options in `config/accessibility.php`
```text
ACCESSIBILITY_ENABLED=true
``` 

### Laravel 5.5+:

If you don't use auto-discovery, add the ServiceProvider to the providers array in `config/app.php`

```php
Oh4d\Accessibility\ServiceProvider::class
```

Copy the package config and translation files to your local with the publish command:

```shell
php artisan vendor:publish --provider="Oh4d\Accessibility\ServiceProvider"
```