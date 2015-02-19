# PHP REST Client
[![Latest Stable Version](https://img.shields.io/packagist/v/romanpitak/php-rest-client.svg)](https://packagist.org/packages/romanpitak/php-rest-client)
[![Total Downloads](https://img.shields.io/packagist/dt/romanpitak/php-rest-client.svg)](https://packagist.org/packages/romanpitak/php-rest-client)
[![License](https://img.shields.io/packagist/l/romanpitak/php-rest-client.svg)](https://packagist.org/packages/romanpitak/php-rest-client)
[![Code Climate](https://codeclimate.com/github/romanpitak/PHP-REST-Client/badges/gpa.svg)](https://codeclimate.com/github/romanpitak/PHP-REST-Client)

(c) 2014-2015 Roman Piták, http://pitak.net <roman@pitak.net>

Representational state transfer PHP client library.

## Installation
The best way to install is to use the [Composer](https://getcomposer.org/) dependency manager.
```
php composer.phar require romanpitak/php-rest-client
```

## Basic Usage

```php
$client = new Client('http://api.example.com/v2/'); // Use the client to store general settings

$request = $client->newRequest('hello-world.json'); // Returns a Request object

$response = $request->getResponse(); // Returns a Response object

$content = $response->getParsedResponse(); // Returns the response body as a string
```
