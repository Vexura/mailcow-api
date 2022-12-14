Mailcow PHP API Client
=======================
This **PHP 7.2+** library allows you to communicate with the VPNResellers-API.

[![Latest Stable Version](http://poser.pugx.org/vexura/mailcow-api/v)](https://packagist.org/packages/vexura/mailcow-api) [![Total Downloads](http://poser.pugx.org/vexura/mailcow-api/downloads)](https://packagist.org/packages/vexura/mailcow-api) [![Latest Unstable Version](http://poser.pugx.org/vexura/mailcow-api/v/unstable)](https://packagist.org/packages/vexura/mailcow-api) [![License](http://poser.pugx.org/vexura/mailcow-api/license)](https://packagist.org/packages/vexura/mailcow-api) [![PHP Version Require](http://poser.pugx.org/vexura/mailcow-api/require/php)](https://packagist.org/packages/vexura/mailcow-api)
## Getting Started

Recommended installation is using **Composer**!

In the root of your project execute the following:
```sh
$ composer require vexura/mailcow-api
```

Or add this to your `composer.json` file:
```json
{
    "require": {
        "vexura/mailcow-api": "^1.0"
    }
}
```

Then perform the installation:
```sh
$ composer install --no-dev
```

### Examples

Creating the MailCowAPI main object and get all Domains:
```php
<?php
// Require the autoloader
require_once 'vendor/autoload.php';
// Use the library namespace
use Vexura\MailCowAPI;
// Then simply pass your API-Token when creating the API client object.
$client = new MailCowAPI('API-Token');
// Then you are able to perform a request
var_dump($client->domains()->getDomains());
?>
```